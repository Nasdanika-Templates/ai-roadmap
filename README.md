# Roadmap Site

This is a template repository for roadmap web sites generated from [Drawio](https://www.drawio.com/) diagrams with [GitHub Actions](https://docs.github.com/en/actions) and [Nasdanika CLI Drawio Command](https://docs.nasdanika.org/nsd-cli/nsd/drawio/index.html).

It is created from the [Drawio site template](https://nasdanika-templates.github.io/drawio-site/) - see that template for the general information about Draw.io sites. 
The below documentation focuses on the roadmapping aspect.

The AI roadmap diagram is based on the roadmap slide from the [AI Leadership Track: Gen AI, Agentic AI for Business Leaders](https://www.udemy.com/course/executive-briefing-generative-ai-and-large-language-models-llm/) Udemy course.

[TOC levels=6]

## Overview

This site has the following "implied" domain model: **Roadmap** (table) consists of **Phases** (columns) and **Actors/Stakeholders** (rows) with **Deliverables** in cells. 
All elements can have tooltips, documentation and status tags.
Visibility of elements can be toggled by the clicking on the status nodes in the legend.

The diagram is not [mapped](https://docs.nasdanika.org/core/mapping/index.html) to a semantic model and, therefore:
* There is no cross-referencing
* There are extra nodes in the navigation tree because the tree structure follows the containment structure of the diagram

This is a simple approach which allows:

* Manage roadmap as code - version control, collaboration 
* Document roadmap elements
* Build a hierarchy - deliverables can have their own roadmaps if needed
* Toggle element visibility to focus on specific deliverable statues, e.g. "Off Track" or "Blocked"

Semantic mapping is the next step, which brings more structure and power. 
The roadmap model is work in progress and a link to it will be added to this site once it is ready.

## Adding phases or stakeholders

* Use the table "Arrange" tab to add a new row or column
* Select an existing cell. In the Style tab click on the edit drop-down and select "Edit Style...". Select style text and copy it to the clipboard.
* Select new cells - all or one by one. In the Style tab click on the edit drop-down and select "Edit Style...". Select the existing style text and press "Ctrl-V" to paste the copied style of the existing cell from the clipboard. Altenatively, add ``;fontColor=none;noLabel=1;childLayout=stackLayout;horizontalStack=0;stackSpacing=5;stackBorder=5;`` to the end of the existing style string.
* For new cells set the label to the phase name - copy/paste from the header cells.

## Changing status

* Change color
* Open tags view and change the status tag

