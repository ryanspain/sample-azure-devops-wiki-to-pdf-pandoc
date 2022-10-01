# Generate PDF from Azure DevOps wiki

This sample shows how you can take your Azure DevOps wiki repository files, and use them to generate a PDF document using Pandoc. The example uses a Docker image to remove the need to install the various Pandoc dependencies.

## Run locally

1. Install Docker
2. Install the `wikiexport` dotnet tool

    ```powershell
    dotnet tool install dotnet-wikiexport -g
    ```

3. Clone your wiki into the `/src` folder
4. Combine your wiki into a single file

    ```powershell
    wikiexport -s ./src -t ./out --title "Sample wiki" --titleFormat "{title}"
    ```

    - `-s` denotes the source folder
    - `-t` denotes the target folder
    - `--title` is the title of the combined wiki
    - `--titleFormat` lets us simplify the title format

5. Add the helper aliased PowerShell function

    ```powershell
    function Run-Pandock 
    {
        $input = $args[0]
        $output = $args[1]
        docker run --rm --volume "$(pwd):/data" pandoc/latex --pdf-engine=xelatex $input -o $output
    }
    Set-Alias -Name pandock -Value Run-Pandock
    ```

6. Generate the the PDF from the wiki combined wiki

    ```powershell
    pandock "./out/Sample wiki.md" "./dist/Sample wiki.pdf"
    ```
