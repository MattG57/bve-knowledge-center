---
title: Prioritizing Lifecycle Costs in Automation Assets
tags: 
 - Automation
 - Explainer
description: Organizations at different stages of their automation journey face different challenges and exploit different strategies to move automation forward and therefore continuously improve the relative value they derive from Developer Talent and Effort.
---

# Prioritizing Lifecycle Costs in Automation Assets

Authors: Last Edited: May 2nd 2023  
Matthew Gunter

## Overview

Organizations at different stages of their automation journey face different challenges and exploit different strategies to move automation forward and therefore continuously improve the relative value they derive from Developer Talent and Effort.  

This document emphasizes the importance of focusing on lifecycle costs and making new automation assets (and changes) easy and easy to justify, as opposed to a focus on stable, one-size-fits-all pipelines that are expensive to customize and change (even if they are cheap to run on a per minute basis).

## Introduction - “Automation is the number one driver of developer productivity”

One of the critical aspects of a successful automation strategy is the prioritizing of low lifecycle costs and justifiability in automation assets. This approach ensures that organizations can scale their automation efforts while remaining agile and responsive to changing requirements.  

Focusing on one-size-fits-all pipelines that are expensive to change and inefficient to run in terms of compute costs and delay can lead to several issues, including inflexibility, high maintenance costs, and difficulty in adapting to new or changing business needs. To avoid these pitfalls, organizations must invest in automation assets that are easy to maintain, adapt, and justify, ensuring that the investment yields the desired return over time. GitHub Actions & GitHub-hosted Runners keep the cost to automate and the cost to improve automation low. How can we be sure it is reasonable to prioritize such costs?

Automation is the number one driver of developer productivity^(1) (and efficient software processes are a major driver of Organizational Effectiveness metrics like Revenue Growth^(2)). 

Providing developers with better options for adopting incremental automation and ways to improve and grow automation use cases cost-effectively results in greater productivity and faster productivity improvement.

This paper is focused on clarifying this journey, identifying the value drivers, along with GitHub’s strategic advantages and historical customer successes. Combining Value Drivers with the Automation Journey provides a coherent framework that supports value assessments, comparisons, and communicates the Value of Actions both to customers within their current “zones-of-value” and their aspirational zones further out.

^(2) “Our research reveals that top-quartile Developer Velocity scores correlate with 2014–18 revenue growth that is four to five times faster than bottom-quartile Developer Velocity scores.”, McKinsey 2020

^(1) “According to our research, best-in-class tools are the primary driver of Developer Velocity.”, McKinsey 2020


## The Importance of Low Lifecycle Costs in Automation Assets

As companies adopt Developer Automation, they travel through different zones-of-value as they automate and mature their processes. The main reason for this pattern to emerge is that automation can address many different types of problems at the Developer level, Team level, and Enterprise level. Solving all of these problems and scopes in one phase isn’t realistic. So, we typically see organizations focused on only one or two zones of value at a time. Frequently, organizations even get stuck when historical decisions about automation are problematic and frustrate their forward progress. A simple example is when teams have made disparate decisions about automation tooling and then the organization is looking to reduce redundant lifecycle efforts across these teams. In such cases, existing automation will need to be re-implemented in a new standardized way to support sharing skills and artifacts across teams and individuals. 

Modeling automation as a journey clarifies that there are many types of value to pursue with automation efforts, and value will change and accumulate over time.  

It also highlights that early automation Investments have an easier case for investment. Later in the journey, As existing automation becomes significant, additional automation investment can slow down. One reason for this is that early automation can’t be easily changed and therefore, justifying more adaptability creates a chicken and egg problem.

Chicken and Egg 🐔 🥚 ...of Improving and Adopting New Automation over time.

If Existing Automation is not changing, how can we justify features that make it easier to change?

If Automation isn’t easy to change, the benefits of any investment in new Automation has to be large enough to justify the change and improvement efforts.


Organizations that can’t move to the next zone find themselves with fewer options for improving automation and tend to shift focus toward managing the cost of existing automation. This cost focus causes the rate of improvement to slow down or stop. 

GitHub Actions brings many technical advantages to bear for developing incremental automation so that the incremental cost to automate remains low, allowing organizations to advance their focus to their next zone. 

GH Actions:

- Improves Reuse^(3)
- Broadens Collaboration^(4)  
- Provides Visibility^(5)
- Ensures Control and Compliance^(6)
- Enables a focus on Decision Quality^(7)

As shown in the examples below, GH Actions lowers the Incremental Cost to improve automation to capture different types of automation value over time.

## Incremental Automation drives Incremental Value

Enterprises often find themselves trapped in cost-control mode, focusing on execution and operation expenses rather than the costs of improvement and adaptation. 

Here are several common structural limitations that organizations can encounter on this journey:

### Structural Limitations to avoid or overcome

| Limitation | Description |
|-|-|  
| 1. Lack of Technology/Skills/Bandwidth | The opportunity to Adopt automation is blocked by the inability to execute |
| 2. Lack of Standardization | The opportunity to share knowledge, skills, and assets is blocked by too much diversity and friction between teams & solutions. |
| 3. Lack of Modularization | The opportunity to create, modify, and share across more & more assets is blocked by solutions being too monolithic without the potential for sharing and blending contributions from many teams. |
| 4. Lack of Collaboration | The opportunity to involve more talent, teams, and repositories of assets is blocked by teams being unable to see, share, contribute and reuse across teams and repositories. |
| 5. Lack of Visibility & Control | The opportunity to create, modify, and share across more & more assets is blocked by inconsistent policies and fragmented access & visibility. |

Organizations risk hitting one of several of these limitations along their Automation Journey. By keeping the entire automation journey in mind, organizations can avoid limitations and maximize the value they derive from their ongoing automation efforts. Ultimately, automation creates better options, allowing organizations to respond more efficiently to changing situations.

Developer Automation is on the rise within organizations. Continuous Integration and Continuous Delivery are typical focus areas where Organizations prioritize reducing labor costs, delay, variability, and risk from non-automated processes. This leads to quick wins. 

GitHub Actions Customers are able to go well beyond CI/CD to automate other aspects of the software lifecycle: 

### GH Actions Automation Examples

| Process | Before | After | Implications |
|-|-|-|-|
| CI & Release Automation (Build, Deploy, Test) | Non-standard, not modular, with diminishing rate of change/improvement | Standard, modular, extensible, cloud-based | 1.) Improve developer feedback cycles, consistency, plus greater extensibility for inserting tasks like Code-Scanning. <br><br> Train new hires & Adopt tooling, Ensure Consistency |
| Train new hires & Adopt tooling, Ensure Consistency | Less popular, legacy tools, variable levels of checks, inconsistent quality, islands of automation | Modern, popular tooling with much higher consistency, controls, checks, and sharability, along with a consistent lifecycle for automation | 2.)Reduce training requirements and create a common foundation for sharing, visibility, and control/compliance. |  
| Security Testing & Compliance | Missing, fragmented, or inconsistent processes that involve significant waste. | Consistent approaches for security, clear direction and standards for repos & developers | 3.)Reduce risk of unknown and/or unremediated vulnerabilities. <br><br> Improve efficiency, margin-of-safety & visibility |
| Improve System Coordination and Human Collaboration | Missing, fragmented, or inconsistent processes that involve significant waste. | Self-Service, OnDemand access to exploit automation (and create new automation as needed) for repo-specific and centralized automation tasks | 4.) Reduce the delay and cost of growing the amount of coordination via automation.(Central and Team-based) |

Some time after the initial growth of uncoordinated automation, organizations tend to prioritize standardization, modularity, and collaboration. These measures help reduce friction, redundancy, and unnecessary diversity, fostering investment in operations, skill development, and reusable automation assets. GitHub Actions and GH-hosted Runners facilitate this part of the Automation Journey by making new automation easy to build and easy to run, which is crucial for enhancing the speed and collaboration surrounding automation and ultimately boosting overall agility.

The next opportunity for organizations is to extend the horizontal collaboration capabilities that GitHub is known for into the vertical direction. In addition to custom Actions and Workflows being reused voluntarily by other teams, visibility and mandatory policies can also be mandated from change management and security groups so that enterprise-wide concerns around risk mitigation and audit readiness can be automated as well. Flexibly combining vertical and horizontal collaboration to continually improve automation is critical to financial justification, the investment of new assets, and realizing the benefits of improving existing processes. 

Focusing on decision quality represents the optimal end goal in the journey depicted above. In this stage, the effort and cost of execution is low (due to high levels of automation). This shifts the focus toward selecting the best path of execution, based on the emerging information and context. Leveraging automation to support enhanced decision-making processes is crucial for organizations to excel at this level.

Conversely, when incremental automation proves costly, introducing new automation may necessitate revisiting and refactoring entire architectures and extensive shared assets. In such scenarios, only significant benefits can justify the investment. This predicament is where many enterprises find themselves "trapped." 

## Real-World Customer Stories

To better understand how new value is unlocked at different points on this automation journey, we can review a few real-world customer stories who have exploited various zones of value with GitHub Actions.

Organizations early in their Developer Automation journey go through an adoption phase where the benefits of Reducing Labor costs, Delay, Variability, and Risk from existing non-automated processes takes priority over the technology and structural considerations. This leads to Quick Wins.

Once automation reaches a certain level of scale with ad hoc uncoordinated growth, the following opportunities become areas of focus:

1. Standardization,
2. Modularity, and  
3. Collaboration

Standardization removes friction, variability and complexity and also makes it possible to invest strategically in operations, skill sets, and reusable automation assets.

For example, 

KPMG - Sharing custom-built Actions reduces time-to-value:

>"Meanwhile, since moving to GitHub, automation plays a larger role in KPMG’s workflows. For example, the company uses GitHub Actions to deploy its .NET and React applications, automating what would otherwise be a manual build step. “GitHub Actions has been incredibly powerful for us, because it reduces the time it takes for a developer to get up and running,” says Annette. Plus, because GitHub has fostered a culture of code reuse within KPMG, teams now share custom-built Actions, creating new efficiencies."

>- "For example, KPMG built custom automations with GitHub Actions to check projects for compliance with the company’s security policies."

The ability to share and reuse automation can also be extended beyond the organization to include assets developed at other companies and made available via the Marketplace.

For example,

Decathlon - Mixing custom and marketplace actions into a standardized software change model:

>"On their [Decathlon's] internal code, the team uses the standard Git flow and leverages both existing GitHub Actions and ones they’ve developed themselves. All of their actions automatically create a release note and push it onto the Wiki page of the repository. “Everything is done automatically. We see an action like an extension of continuous integration,” said Alexandre. One of the more popular features is suggesting modifications. “This way, users can directly apply the changes on GitHub.”

More advanced opportunities also emerge at this phase of growth: 

1. Enterprise wide visibility
2. Policy enforcement 
3. Reducing the cost of incremental automation

For example,

Ahold Delhaize -

>“GitHub Actions have also helped the team speed up delivery. Their self-hosted Jenkins CI system had a limited capacity that ultimately affected performance. At peak times, developers had to do a lot of sitting and waiting for their builds to start. But using Actions for CI/CD on the GitHub hosted runners, they can test code on multiple operating systems and platforms simultaneously, while also being able to scale to demand. Everyone can build their software directly without sitting in a queue.

>“Everything we build now—our React components, etc.—are all run in Kubernetes and are all 100% automated,” Hofman added. “Essentially, for every pull request that’s opened and merged into the main branch, CI triggers a workflow. And from there to QA, deployment, and production, it’s completely automated.”

>The team uses a few pre-built Actions, but when they can’t find what they need on GitHub or GitHub Marketplace, they build their own. If Ahold Delhaize developers make a useful improvement or create a new generic workflow, they’re inclined to share it. So far, they’ve built eight Actions, and are thinking about which ones to open source. “It’s a very fun, rewarding process,” said Timmer, “You’re helping build software that many others can benefit from and contribute to.”

Reducing the cost to build these types of automation capabilities is necessary to justify the continued incremental automation. How can GitHub Actions help keep the lifecycle costs of automation low?

GH Actions (and GH Hosted Runners) reduces the “cost to automate” in the following ways:

1. Standardize workflow technology and templates across all teams.
2. Leverage Scale, Minimize Redundancy. Reducing the maintenance burden of individual Dev Teams through shared assets that factor-out the building, maintenance, and support of common automation dependencies.  
3. Facilitate sharing of automation assets across teams, Standardization and minimizing redundancy creates capacity for new shared automation components. Reducing the friction for reuse while minimizing redundant maintenance efforts should therefore be a motivation for investing in sharable internal-only assets and ensuring compatibility and visibility to public, marketplace assets.
4. Provide central team visibility and control. Automation needs to support increasing levels of participation and policy enforcement to support efficient governance and oversight. 
5. Support provenance, immutability, and repeatability. Features like signed immutable images, packages, allow lists and Private container registries are needed to ensure secure software supply chain outcomes like auditability.
6. Support easy execution-optimizations. Provide clear optimization options so that work can be executed in parallel(to leverage larger runners) or ahead of time(to leverage caching) without compromising the above goals.

With these approaches in mind, automation efforts can proceed from the most justified to the least justified aspects to automate. 

### Cost and Delay Reduction Potential from Offering Two Options

- Save 540,000 hours of delay?

or
 
- Save $70 Million?

Outcome (approximated based on 5,000 developers) for each option:

| Option | Hrs of Delay | Labor Cost if Dev is Waiting |
|-|-|-|
| 2-Core Runner | 1.2 Million Hrs | $160 Million in Labor |  
| 4-Core Runner | 660,000 Hrs | $88 Million in Labor |

By providing two options instead of a one-size-fits-all fixed decision, delays and labor costs can be optimized as needed depending on context.

For more details on this research, please refer to: 

[The cost of waiting on builds](https://github.blog/2022-06-08-new-research-quantifying-the-impact-of-github-actions-speed/), by Natalie Somersall

The following graphic illustrates how new use-cases become possible as the organization improves the minimal cost and delay required to build and run automation(dotted line shifting to the right). 

![automation growth zones graphic](automation_growth_zones.png "Automation Growth Zones")

Starting with a one-size-fits all pipeline that provides little or no autonomy, we can see that as automation assets become easier and cheaper to create, maintain, and utilize, it is easier to justify their investment. This process allows ROI from automation to be realized for Team-specific, Dev-specific, and even experimental automation workloads. 

Increasing Automation can sometimes “create distance” between groups and silos (by becoming bureaucratic and a black box) or, on the other hand if shared control and visibility is prioritized, automation can form a better communication channel to support better decision-making, and actively unblock and accelerate initiatives.

For example,

McKesson - Developer Control with enforcement automated through a single, shared platform:

>"“GitHub is more than just a repository manager,” said Hurley [Mckesson Labs]. “It streamlines the software development workflow by allowing developers to manage all tools and services from a single platform they already use on a daily basis.” GitHub makes workflow automation a breeze with its many customization features and seamless integration with other tools. For instance, Developer Services configured default settings for all GitHub repositories in order to standardize their projects as much as possible. Using GitHub Actions, they can check to ensure that none of the proper settings have been incorrectly changed."

## Automation Growth Zones 

By viewing asset lifecycle costs and compute costs together, a map of Automation Growth Zones emerges, helping to clarify the shifting focus of enterprises at different stages in their growth journey.

Organizations proficient in automation ensure that their investments in lifecycle costs and compute costs are justified. They also expect that their overall compute costs must increase along with the organization’s growth both in headcount and in activity. Counter-intuitively perhaps, compute costs must also increase as it becomes more efficient, since automation is key to enhancing developer and organizational productivity.

An important implication of the value map view is that both axes must support a high level of modularity and granularity of options in order to allow for just enough lifecycle costs or compute costs, just in time to accomplish the task being automated. 

Such an approach enables organizations to optimize their automation efforts, ensuring that each incremental improvement is sustainable, justified, and well-timed. By fostering a flexible and adaptive automation environment, organizations can avoid becoming stuck