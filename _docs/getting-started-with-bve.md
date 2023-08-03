
---
title: Getting Started with BVE
tags: 
 - Process
 - Assessment
description: Getting started with Business Value Engineering
---


# Getting Started with Business Value Engineering

<style>
.indented img {
  border: 1px solid black; 
  width: 700px;
  height: 700px;
}
</style>

## 🔭 What is Business Value Engineering?
_Quantifying Value With BVE, Authors: Matthew Gunter_
_Last Edited: Feb 26th, 2023_

**Business Value Engineering (BVE)** provides a framework for guiding and validating improvement efforts across an organization. Data from various sources are combined to clarify the impacts of improvements.

These can be any of the following types of improvements:

### Types of Change:

**Process changes (e.g. reduce steps, add automation)**

**Product Features (e.g. provide add’l parallelism, bidirectional control, or visibility)**

**New Practices (e.g. adopt new standards, improve decision-making)**

During a Business Value Assessment, relevant information is collected to create an analytical model of the existing process that clarifies how things work today. The process’ “inputs” are quantified primarily in terms of Cost 💵, Delay ⏱, and Risk 🦺 metrics. These quantifications are aggregated by time-period (sprint, month, year), and by relevant “Units of Work” (PR, Release, Remediation, etc.), and grouped for relevant stakeholders (VP of Dev, VP of Ops, CISO)

### Comparing Before and After
To calculate the improvement potential, a before vs after comparison is created with one or more proposed changes. For each change, the expected impact on **Cost 💵, Delay ⏱, or Risk 🦺** is modeled discretely for a time-period, step, or unit of work.  Projecting from these small improvements, the aggregate impact can be summarized and communicated via one of several value-viewpoints.

**Value-Viewpoints**
- Efficiency Viewpoint: Evaluate the improvement for the Processes (via value stream mapping, etc.) for each “unit of work” that will be affected by the change(s).
- Productivity Viewpoint: Evaluate the improvement for individual participants (via interviews and “Week in the Life” surveys) for those that will be affected by the change(s).
- Structural Viewpoint: Understand and clarify how the improvements structurally improve what the organization can do in terms of increasing the options for being responsive or by for coordinating parallel efforts. This can be thought of as “structural leverage” (e.g. Ability to adapt)
Decision-Quality Viewpoint (Not Shown): Measures the benefits of the anticipated changes on improving Optionality, Predictable Execution, and Decision-Quality over time.

<span class="indented">
  <img src="/bve-knowledge-center/assets/img/business-value-viewpoints.png"> 
</span>
* * * *

### Account-Team-Guidance


On the right side of any page, you'll notice links to edit the page, or
open an issue. This ensures that any time you have a question or want to 
suggest or request a change, you can do so immediately and link directly
to the section of interest. The sections on the page also have permalinks so
you can link directly to them.

### Customer-Guidance

The entire site, including posts and documentation, is indexed and then available
for search at the top or side of the page. Give it a try! The content is rendered
into window data that is used by lunr.js to generate the search results.
If you want to exclude any file from search, add this to its front end matter:
