# Content and UI Pattern Library

User Interface Design patterns are recurring solutions that solve common design problems. 
Content Patterns are standard reference points for the experienced user interface designer.

Content Patterns provide a common language between designers. 
They allow for debate over alternatives, where merely mentioning the name of a 
content pattern implicitly carries much more meaning than just the name.

## Why bother?

Currently with Joomla!, extension developers (and the core as well) put hard coded HTML and JS into their view,
and additionally put their own styling preferences into it.
Since we in Joomla!4 want to establish a Channel Independency Border, that cannot be allowed anymore.

## Solution

The solution is to provide a kind of 'Domain Language', a collection of building blocks
(so called atoms, molecules, organisms in Atomic Design), developers can use instead.
The advantage is, that we get a much better separation of concerns:
 
  - The developer defines the output independent from the output media, on kind of a semantic level.
  - The Renderer creates the structure (HTML) and functionality (JS) from it.
  - The template adds styling to the structure.
  
The Content and UI Pattern Library is ment to support on all three stages.
It

  - defines the building blocks, that the developer can address, and which data they need,
  - determines which methods all Renderers must provide, and
  - lets a template designer create a template, that works for upcoming extensions as well,
    because (s)he just styles the building blocks (in different contexts, since fx. a LinkList may be styled differently, depending on its position on the page).

## Table of Content

- [Input Control Patterns](input-control/input-control.md)
- [Structural Patterns](structural/structural.md)
- [Design Patterns](design/design.md)
- [Behavioural Patterns](behavioural/behavioural.md)
- [Resources](resources.md)

## Contribution

> :exclamation: This library is work in progress. Actually, it is in a very early stage, and needs your help.

To contribute, 

  - Fork this repository, add your pattern(s), modify existing patterns, add resources ...
  - For the Content Patterns please use the [template](template.md), so the pattern descriptions all follow the same structure.
  - Resize screenshots to 50% of the original size, and crop away as much as possible.
  - Name the screenshots according to the pattern, suffixed by number, and place them in the `img` directory of the pattern group.
    Example: `structural/img/paragraph-1.png`, `structural/img/paragraph-2.png`, `structural/img/paragraph-3.png` for images showing the Paragraph pattern. 
  - Send a Pull Request
  
## License

![by](img/pict-by.png)
![nc](img/pict-nc.png)
![sa](img/pict-sa.png)

The content of the **Content and UI Pattern Library** is published under the
**Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License** [CC-by-nc-sa](http://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
