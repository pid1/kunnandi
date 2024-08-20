
# kunnandi

[![Super-Linter](https://github.com/pid1/kunnandi/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)

ᚴᚢᚾᚾᛅᚾᛏᛁ

A repository of living knowledge. For more information, see [About](#about).

_"Quite generally, the familiar, just because it is familiar, is not cognitively understood. The commonest way in which we deceive either ourselves or others about understanding is by assuming something as familiar, and accepting it on that account; with all its pros and cons, such knowing never gets anywhere, and it knows not why. Subject and object, God, Nature, Understanding, sensibility, and so on, are uncritically taken for granted as familiar, established as valid, and made into fixed points for starting and stopping. While these remain unmoved, the knowing activity goes back and forth between them, thus moving only on their surface. Apprehending and testing likewise consist in seeing whether everybody's impression of the matter coincides with what is asserted about these fixed points, whether it seems that way to him or not."_

Georg Wilhelm Friedrich Hegel, Phenomenology of Spirit §31

## Table of Contents

- [About](#about)
- [Complexity](#complexity)
- [Leadership](#leadership)
  - [Enabling high performers](#enabling-high-performers)
- [Opportunity Cost](#opportunity-cost)
- [Socialization Syndrome](#socialization-syndrome)

## About

Kunnandi, from the Old Norse for "knowledge" or "understanding," intends to provide a living repository of my patterns of thought.

Moving beyond the topic-focused, point-in-time blog posts, Kunnandi is closer to a continuously-published collection of dictum.

Born out of my frustration with blogging as a medium, a Kunnandi provides the following features:

### Temporality

Due to constraints of the medium, documents provide recorded information from a single point in time.

Kunnandi is always as up-to-date as its last commit.

Kunnandi makes the development of the document intrinsic to its nature, providing context that is unavailable in other mediums.

### Flexibility

Kunnandi details patterns of thought. These patterns are intrinsically jumbled, intertwined, and imprecise.

By providing them in a single, continuously-updated document, their historical development and interrelationships become clearer. By documenting thought patterns instead of topics, we increase the signal to noise ratio and streamline the process of writing.

## Complexity

Complexity has to live somewhere and the real consideration is constraints.

To give the infrastructure engineering example, let’s assume we are deploying some AWS. We need an ALB, Route53 entries, a couple EC2 backends in an autoscaling group, an RDS database, an Elasticache instance, and a couple Lambdas for your cron jobs. You could deploy these ClickOps style, poking around the UI and setting everything up, or you could deploy them via your infrastructure as code tool of choice.

We could also go all out, containerize the application, get a k8s cluster in a couple clicks and deploy our Helm chart. Done! Easy! “Simple”, right?

Given an organization with a couple of folks who understand Terraform, Packer, and Github Actions, a CI/CD pipeline for this would be reasonable to create and maintain. Assuming no organizational understanding of these tools, the ability to make modifications within the UI, follow the upstream AWS documentation, and lean on AWS Support may be preferable until we can perform some cross-training and up-skill the team to where Terraform maintenance is reasonable. Given a team who has never maintained a Kubernetes cluster or containerized an app, would it be simple, or even responsible, to run this on EKS?

Is the “simple” solution consuming third-party cloud services? If the organization is too financially constrained for that, but person-hours, technological familiarity, and on-prem servers are all available to deploy an equivalent open source solution, is it then wrong to accept the operational complexity of maintaining that service rather than consuming it?

Understanding constraints and risk are deeply intertwined. See [Leadership -> Enabling high performers -> Understand and communicate risk](#understand-and-communicate-risk).

## Leadership

### Enabling high performers

High performers are enabled, not found. Our organizations are awash in talented, intelligent individuals who can complete the tasks ahead of them. A subset of these individuals stand out as top performers. These folks hold junior to principal, tech and non-tech roles, but they all have a disproportionate impact relative to their position at the organization. They create shadow org charts, working behind the scenes to bypass traditional hierarchy and accomplish their goals. We consider them to be unique, born with an intrinsic leadership capability and sense of ownership.

This is a misguided assumption which prevents us from building the sorts of organizations that enable every individual to be exceptional. Everyone at your company has the capacity to be a high performer. To enable this, culture and incentives must align to enable the intrinsic motivation and high-trust environment required for individuals to prosper.

#### Understand and communicate risk

Create an organizational understanding of risk exposure, risk capacity, and risk appetite. Is your organization in a highly regulated industry, where compliance and auditing is your largest risk exposure, or are you most exposed to market forces? Are you highly financially constrained, limiting your capacity to make bets on technology investments that might not pay off? Are you approaching an IPO, and the organization needs to “stay the course” for a period of time? Without risk understanding, it is impossible to tell how far the organization can flex. Understanding and communicating this ability to flex allows for informed decision-making. Without this, individuals have no sense of what “big bets” may or may not be feasible to take on.

#### "Know the why" or, "What is the problem we are trying to solve?"

Everyone, at all levels, must understand the goals the organization is trying to achieve.

Organizational goals do not exist in isolation. They are a distillation and distribution of complexity into understandable objectives. Without this, we increase confusion and ambiguity. With these goals, we increase clarity and organizational alignment.

This becomes more critical as you scale, as a decreasing percentage of individuals at the organization have the necessary context to make good decisions.

##### Psychological Safety and Incentives

Ownership and empowerment necessarily come along with a degree of latitude in execution. For this to work, individual incentives must align to operational outcomes. If performance reviews will be based on OKRs defined a year ago that no longer reflect the operational reality, are folks incentivized to work on the right projects? Is appropriate risk-taking rewarded, even if a project does not pan out? Exploratory opportunities as allowed by the organizational risk profile are a necessary precondition for growth, both individually and for the business. Investigate mistakes in a way that focuses on the process and situational aspects of the failure state and the decision-making process behind that failure, not individuals or teams. Stakeholders must not fear punishment or retribution.

##### Policies and procedures are written to enable, not prevent

Policies and procedures must be written such that we enable a distributed command mentality, giving individuals a framework for decision-making within the constraints of our organization. They must not be solely written as punitive, documenting what must not be done.

From an engineering standpoint, this means incorporating compliance and security deep into DevSecOps pipelines and making the compliant, secure way of working the easy, convenient way of working. Balancing tactical and strategic work, depending on a given team’s need to be proactive or reactive, may mean that scrum is abandoned in favor of Kanban for some subset of Engineering.

Shoe-horning in policies without consideration for how they will impact workflows hinders velocity. Attempting to prevent every failure with policy, especially manually enforced policy, is misguided. This is an opportunity to instead analyze ways of working and triage the root causes of potential failure. Nurture an operational standard of blameless, continuous improvement, open to feedback from stakeholders anywhere and everywhere in the organization. Artificially imposing ways of working simply because it is “how we do things” reduces the organization’s ability to execute.

##### Be clear

In all aspects, be clear in intent and outcome. Document decisions in writing, use clear and precise language, and over-communicate when decisions are made, especially when changing a previous policy.

Make the implications of the decisions clear for those impacted, and have a single source of truth that is easily accessible to the entire organization. When written decisions are the norm, teams default towards reading and asking for clarification when necessary, instead of guessing and amplifying confusion.

Use lightweight processes for decision-making so individuals always know the history and status of a proposal.

The criticality of this only increases with the fanciness of your title, as you have a disproportionate downstream impact on the rest of the organization.

## Opportunity Cost

Thomas Sowell opines in Basic Economics that “[…] the real cost of anything is still its value in alternative uses. The real cost of building a bridge is whatever else could have been built with that same labor and material. The cost of watching a television sitcom or soap opera is the value of the other things that could have been done with that same time.”

Organizations make this determination every time they choose to work on one ticket, project, or OKR over another. Making this value judgment explicit is critical to a well-functioning organization. To do this effectively, organizations must understand and communicate priorities and individuals must be incentivized to work towards those priorities.

If an organization does not understand its own priorities, it is impossible to prioritize the “right work” since that term is undefined. Organizational goals, explicitly communicated in a format like OKRs, align disparate teams around clear objectives. Even on teams that collaborate effectively, a formalized, regular goal-setting process minimizes drift and overlap across teams and departments.

Furthermore, incentivize individuals to fulfill these organizational priorities. If an organization rates employees on their response times to customer requests, but the OKRs are all centered around long-term internal projects, this misalignment means workers will never achieve the organizational goals. Either adjust the employee ratings to align with the OKRs or adjust the OKRs.

Apply this thinking to your day-to-day tasks. Is this ticket or project worth working on in light of your team, department, and organizational priorities? Are incentives structured in a way that encourages individuals to work on the projects you want them working on? If such organizational priorities are not set at all or are not clearly communicated, start a dialogue with leadership around these topics. Encourage them to provide this guidance so everyone on the team can make better decisions.

Always consider the bridge not built.

## Socialization Syndrome

Over-socialization is the internalization of social norms, values, and expectations to such an extent that the individual's personal autonomy, individuality, and creative thinking diminish. Over-socialization in the workplace, or Socialization Syndrome, is an insidious narrowing of horizons. On a long enough time scale, organizational conceptions of the possible drop to zero. The inmates, responding to the conditions of the asylum, struggle to imagine what could be. This is Blockbuster scoffing at streaming or Kodak's inability to synthesize their own market research.

Socialization Syndrome is a particular feature of organizational rigidity. Distinct from bureaucracy, it stems from cultural norms.

Amazon avoids this through a conscientious process whereby:

- Decision velocity is as valuable as decision quality 70% of the information you wish you had is good enough
- Disagree and commit means a genuine difference of opinion followed by candid discussion and subsequent quick, sincere commitment to a course of action
- Amazon accepts that ideas are gambles and failures are learning opportunities.

Skunkworks divisions are indicative of Socialization Syndrome at work. Why is your innovation sequestered? Why does your innovation need sequestering? While a short-term solution to spur creativity, examine why this is not incorporated into your normal course of business. Hackathons are similar, demonstrating a failure to make innovation routine.

Examine the incentivization structures your organization creates.

- Is innovation a cultural value?
- Do you embrace and incorporate the learning opportunity of failure?
- Have you defined your goals effectively, such that success and failure are understood?

Dmoes your team have an understanding of organizational risk tolerance as it relates to what “big bets” may or may not be feasible to take on? See [Leadership -> Enabling high performers -> Understand and communicate risk](#understand-and-communicate-risk).

Socialization Syndrome constrains organizational adaptability and innovation. It culminates in an insidious narrowing of horizons and a diminishing capacity to envision novel possibilities over time. Delve into the complexities of your cultural fabric and foster a climate that rewards innovation, embraces risk, and empowers individuals to challenge conventional thinking.

### Further Reading

Wrong, D. (1961) _The Oversocialized Conception of Man in Modern Sociology_

Goffman, E. (1961) _Asylums: Essays on the social situation of mental patients and other inmates_

Randolph, M. (2019) _That Will Never Work_

Barabba, V. (2011) _The Decision Loom_

Bezos, J. (2016) _2016 Letter to Shareholders_
