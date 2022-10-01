---
title: Sample wiki
author: 
date: 1 October 2022
toc: yes
---
# Main

# Paragraphs and line breaks
Add lines between your text with the **Enter** key.
Your text gets better spaced and makes it easier to read.

# Blockquotes
> Single line quote
>> Nested quote
>> multiple line
>> quote

# Horizontal rules
above

----

below

# Emphasis (bold, italics, strikethrough)
Use _emphasis_ in comments to express **strong** opinions and point out ~~corrections~~ 

**_Bold, italicized text_**  

**~~Bold, strike-through text~~**

# Code highlighting
```
sudo npm install vsoagent-installer -g  
```

To install the Microsoft Cross Platform Build & Release Agent, run the following: `$ sudo npm install vsoagent-installer -g`.

```powershell
Get-Item
```

```js
const count = records.length;
```

```csharp
Console.WriteLine("Hello, World!");
```

# Tables
| Heading 1 | Heading 2 | Heading 3 |  
|-----------|:-----------:|-----------:|  
| Cell A1 | Cell A2 | Cell A3 |  
| Cell B1 | Cell B2 | Cell B3<br/>second line of text |

# Lists
## Ordered or numbered lists

1. First item.
1. Second item.
1. Third item.

## Bulleted lists

- Item 1
- Item 2
- Item 3

## Nested lists

1. First item.
   - Item 1
   - Item 2
   - Item 3
1. Second item.
   - Nested item 1
      - Further nested item 1
      - Further nested item 2
      - Further nested item 3
   - Nested item 2
   - Nested item 3

# Links
[Link text](/url)

# Anchor links
## First heading

No content. See the [Third heading](#third-heading).

## Second heading

No content. See the [Third heading](#third-heading).

## Third heading

Some content.

# Images
## First image

TBC

## Last image

TBC

# Checklist or task list
- [ ] A  
- [ ] B  
- [ ] C  
- [x] A  
- [x] B  
- [x] C  

# Emoji
:white_check_mark:

:negative_squared_cross_mark:

# Mathematical notation and characters
[[_TOC_]]

## General

$
\alpha, \beta, \gamma, \delta, \epsilon, \zeta, \eta, \theta, \kappa, \lambda, \mu, \nu, \omicron, \pi, \rho, \sigma, \tau, \upsilon, \phi, ...
$  


$\Gamma,  \Delta,  \Theta, \Lambda, \Xi, \Pi, \Sigma, \Upsilon, \Phi, \Psi, \Omega$

## Algebraic notation

Area of a circle is $\pi r^2$

And, the area of a triangle is:

$$
A_{triangle}=\frac{1}{2}({b}\cdot{h})
$$

## Sums and Integrals

$$
\sum_{i=1}^{10} t_i
$$


$$
\int_0^\infty \mathrm{e}^{-x}\,\mathrm{d}x
$$

# Mermaid diagrams
## Sequence diagram

::: mermaid
sequenceDiagram
    Christie->>Josh: Hello Josh, how are you?
    Josh-->>Christie: Great!
    Christie->>Josh: See you later!
:::

## Gantt chart

::: mermaid
gantt
    title A Gantt chart
    dateFormat YYYY-MM-DD
    excludes 2022-03-16,2022-03-18,2022-03-19
    section Section

    A task          :a1, 2022-03-07, 7d
    Another task    :after a1 , 5d
:::

## Flowchart

:::mermaid
graph LR;
    A[Hard edge] -->|Link text| B(Round edge) --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
:::

# Collapsible section
## A collapsible section with markdown

<details>
  <summary>Click to expand!</summary>

  ### Heading

  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

# HTML
<p>This text needs to <del>strikethrough</del> <ins>since it is redundant</ins>!</p>
<p><tt>This text is teletype text.</tt></p>
<font color="blue">Colored text</font>
<center>This text is center-aligned.</center>
<p>This text contains <sup>superscript</sup> text.</p>
<p>This text contains <sub>subscript</sub> text.</p>
<p>The project status is <span style="color:green;font-weight:bold">GREEN</span> even though the bug count / developer may be in <span style="color:red;font-weight:bold">red.</span> - Capability of span
<p><small>Disclaimer: Wiki also supports showing small text</small></p>
<p><big>Bigger text</big></p>

# Embed videos
::: video
<iframe width="560" height="315" src="https://www.youtube.com/embed/OtqFyBA6Dbk" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
:::

# Sub page 1 title
Sub page 1 content

## Sub page 1 heading

Sub page 1 content

## Sub page 2 content
Sub page 2 content

### Sub page 2 heading

Sub page 2 content

### Sub page 3.1 content
Sub page 3.1 content

#### Sub page 3.1 heading

Sub page 3.1 content

### Sub page 3.2 content
Sub page 3.2 content

#### Sub page 3.2 heading

Sub page 3.2 content

