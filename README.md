# radar-wms
RaDaR (Read and Demo and Rate) framework for evaluating and selecting a bioinformatics Workflow Management System (WMS)

## User Guide

RaDaR is a tool to help users rate and select a bioinformatics Workflow Management System (WMS). The RaDaR evaluation framework can be applied to any WMS using the criteria defined at the end of this page. During the 'Read' phase, WMS are scored based on information available from their online documentation or website. In the following 'Demo' phase, WMS are scored directly, while completing any criteria that were missed during the 'Read' phase. The WMS are then 'Rated' and compared.

### Time Required

- Shortlisting: 1-2 days (depending on number of platforms on longlist)
- WMS evaluation: up to 4 hours per shortlisted platform

## Shortlisting

The first step towards choosing a WMS is to identify a shortlist of suitable platforms. An initial list of 10-15 platforms is recommended, which can be identified by searching online, looking at publications in the field, or consulting published lists. A list with basic information about 55 platforms is provided as [a downloadable CSV file](https://github.com/MarisaJL/radar-wms/blob/1f853acdf6a54b28e028888ffab3b3a5bd9c63a7/platforms.csv), which can be filtered and extended with the users' own shortlisting requirements. Fewer platforms may be available for specialised fields, while more options can be considered if enough time is available to evaluate them.

This framework does not attempt to define shortlisting criteria as they will be specific to each user and project. The themes and examples listed below provide a starting point for you to think about your own requirements, but they are not exhaustive and some of the suggested categories may not be relevant to you. You should consider what is required to enable you to use the WMS for the types of analyses you expect to run (e.g. having the necessary tools, working at the required scale and security level). Focus on the essential requirements, the features whose absence would make the WMS unusable for you, so that you can quickly rule out unsuitable options.

You might want to consider:

- Computing environment (e.g. will you be able to run the WMS on your laptop, through a cloud service, or on your institution's HPC?)
- Functions (e.g. are the tools you need pre-installed on the platform, can you create the workflow structures required for your analysis?)
- Security (e.g. will you have a password protected account, does the WMS comply with the security measures required to analyse sensitive data?)
- Scalability (e.g. does the WMS provide enough storage for your datasets, can it handle large scale analyses?)
- Cost (e.g. is the WMS free to use, are there additional costs for cloud services, can you afford it?)
- Accessibility (e.g. is the WMS compatible with your screen reader, are you able to navigate using your keyboard?)

Once a list of requirements has been drawn up, the WMS website or documentation can be checked against it. Any WMS that fail to meet all the user and project requirements can immediately be ruled out. Depending on the number of passing WMS, you may want to reduce or expand the shortlist before proceeding, by making the shortlisting criteria stricter or searching for more options to consider. A shortlist of around five platforms is recommended to enable a selection of platforms to be compared in a reasonable time.

### Test Installation

A test installation of the WMS at this stage will confirm that it can be installed and run on the available computing resources, without needing to be aware of all the technical requirements. We recommend performing this step before the evaluation process to exclude platforms that cannot be used within the target environment, which includes both the available infrastructure and your technical capabilities (or the support available to you).

Users applying the RaDaR method could note the cause of any installation problems and consider seeking help to address these before excluding any otherwise suitable platforms (e.g. minor issues such as dependencies may be easily fixed, others such as requiring additional computing power may not be possible for users on a limited budget).

You can then evaluate the shortlisted WMS that met your requirements and were successfully installed.

## 1. Read

The first round involves reading the online documentation for each WMS and scoring it against the evaluation criteria listed at the end of this page. The evaluation should be restricted to official online materials, which may include their GitHub repository, online forums, workflow repositories, or training sites. Contents pages and search boxes can help with locating information, but you could also try asking an LLM to search the official website and provide links to the relevant pages.

### Baseline criteria

You should begin by focusing on the baseline criteria, which are the first criteria in the Sustainability, Usability, Learnability, FAIRness, and Reproducibility categories. These criteria ensure that the platform meets the most basic requirements for a usable WMS (e.g. ‘WMS has been around for at least 1 year and has been maintained within the last year’ in the Sustainability category).

If you cannot tell whether the five baseline criteria are met based on the documentation, then you can proceed to the 'Demo' phase for targeted evaluation of these basic criteria, and then return to complete the 'Read' evaluations if you find the baseline criteria are in fact met.

If a platform does not provide all five of these basic functions, then it is recommended to end the evaluation and reject the WMS. Users may decide to proceed with the evaluation if the WMS only fails in categories that they consider less important for their own needs, but this is not recommended. 

### Continuing the Evaluation

If the WMS passes the first level in each category, you should continue to evaluate the WMS documentation against the remaining criteria. If you are using the online tool, you can select the appropriate score from the dropdown menu in the initial column.

For the first five categories (Sustainability, Usability, Learnability, FAIRness, and Reproducibility), each criterion should be marked as 'Yes' if it is met, 'No' if it is not met, or 'ND' for 'Not Documented' if it is unclear from the documentation. 

For Flexibility-Support, you should choose the best match for each criterion from the suggested definitions of Flexible (marked as 'F'), Supportive (marked as 'S'), or Balanced (marked as 'B). Again, an 'ND' option can be used if it is unclear from the documentation.

> **Adapting the Criteria**
>
> The criteria can be changed according to your needs and preferences. You might want to set your own thresholds for certain criteria. The Usability criteria prioritise WMS that provide a non-code interface, but can be adapted to favour code-based WMS by changing U4 to require a code-based interface.

## 2. Demo

The second round is based on direct evaluation of the WMS. It is recommended to follow any Getting Started advice or introductory tutorials to get to know the interface. Any criteria that were scored as 'ND' during the Read phase should be targeted for completion. A final decision should be made about the score for each criterion, so that all 'ND' options are replaced. If using the online tool, select the final score for each criterion from the dropdown ('ND' will not be an option for the final scores).

The 'Demo' phase should allow you to make a final decision on all criteria, but it is also a chance to familiarise yourself with the platform and get a feel for whether you would be comfortable using it.

## 3. Rate

The final step is to rate each WMS by calculating the total score for each category. If you are using the online tool, the totals will be calculated and plotted for you.

### Scoring

For the first five categories (Sustainability, Usability, Learnability, FAIRness, and Reproducibility), a score of 1 is assigned for each 'Yes' and a score of 0 for each 'No', giving a total out of five.

For Flexibility-Support, a score of -1 is assigned for each 'F', a score of 0 for each 'B', and a score of 1 for each 'S'. The total is then calculated, with a possible range between -5 and 5.

If you are using the online tool, these totals will be calculated for you. You can also download a CSV of all scores.

### Plotting

One way to compare WMS is to create a radar plot showing the total scores for Sustainability, Usability, Learnability, FAIRness, and Reproducibility. The plot will show you which WMS score highly in which categories, and whether there are any areas where they scored less well.

The Flexibility-Support scores can be displayed on a dot plot to see which WMS are at the more flexible end of the spectrum, which provide a more balanced option, and which ones are more supportive. Although negative scores are used for platforms that are more flexible, this should not be taken as a negative evaluation. Users may differ in which end of this spectrum they prefer. WMS closer to the supportive (positive) end are likely to be more suitable for the new bioinformaticians or users with limited computational experience. However, more experienced users or those who require more control of their environment, may prefer WMS at the flexible (negative) end of the spectrum.

The online tool will generate a downloadable radar plot and a dot plot of Flexibility-Support scores.

## Selecting a WMS

The goal of the RaDaR framework is to provide an objective, repeatable, and comparable method for evaluating WMS based on the needs of users, especially those with limited computational experience. The framework is not designed to identify the best platform for everyone, but rather to enable users to select the WMS that is the best match for their own needs. It is anticipated that personal preferences (e.g. which criteria matter most to the individual, the subjective experience of exploring the platforms) will still have some influence on the final platform choice, especially when the scores are similar.

You may decide that Sustainability, Usability, Learnability, FAIRness, and Reproducibility are all equally important to you, and therefore choose the WMS that has the highest overall scores across all categories. However, it may be the case that certain categories are more important for you. For example, if you are new to bioinformatics or looking for a WMS to teach to others, you might want to prioritise Learnability, choosing a WMS that scores highly in this category.

You will also need to consider which end of the Flexibility-Support spectrum you prefer. If you need more control over the computing environment or you want to modify the WMS, then you should focus on platforms at the Flexible end. If you simply want to run analyses or you need a bit more guidance, then WMS on the supportive end of the spectrum will be a better choice.

Since the RaDaR method records which criteria were 'ND' or not covered by the documentation, it should also give you an idea of the quality and completeness of this material. If many criteria were initially marked as 'ND', this suggests that the documentation is limited and it would probably be harder to find any additional information you might need when using the WMS.

If there is no clear winner after considering your priorities and comparing scores, you can draw on your experiences of interacting with the WMS during the evaluations to choose between high-scoring platforms.

## Criteria Definitions

### Sustainability

| Criterion | Definition  |
|---|---|
| S1  | WMS has been available for ≥1 year and has been actively maintained within the last 6 months  |
| S2  | WMS has been available for ≥5 years and has been actively maintained within the last 12 months  |
| S3  | Evidence of an active user or developer community (e.g. forum, chat or other activity within the last month)  |
| S4  |  Evidence of a substantial user or contributor base (e.g. reported number of users/contributors/downloads [evaluators may wish to set a threshold]) |
| S5  | Evidence of adoption in research or practice (e.g. peer-reviewed papers published in the last 5 years are named/cited, the number of publications citing the platform is given [evaluators may wish to set a threshold for this], documented case studies are provided)  |

### Usability

| Criterion | Definition  |
|---|---|
| U1  | Users can create, edit and reuse their own workflows (not limited to pre-defined workflows)  |
| U2  | Progress of workflow runs can be monitored (e.g. status indicators such as queued, running, completed)  |
| U3  | Error reporting identifies the failed step, enabling workflow to be restarted from this point (e.g. workflow resume or re-entrancy) |
| U4  | Workflow creation, editing and reuse can be performed without coding (e.g. Graphical User Interface) [Users who prefer to work in code can adapt this to score for their preferred interface/language]  |
| U5  | Both no-code and code-based interactions are supported (e.g. GUI with optional CLI or scripting interface)  |

### Learnability

| Criterion | Definition  |
|---|---|
| L1  | Documentation is available  |
| L2  | Introductory tutorial or ‘Getting Started’ information is provided for new users (e.g. installation/setting up account, navigating the WMS)  |
| L3  | Tools or components are linked to relevant documentation or external resources (e.g. Seurat pipeline on the platform includes link to the Seurat documentation)  |
| L4  | Domain or task-specific training materials are provided (beyond basic platform usage)  |
| L5  | Interactive learning support is available (e.g. support forum, workshops, courses, automatically graded quizzes, interaction with trainers)  |

### FAIRness

| Criterion | Definition  |
|---|---|
| F1  | Workflows, data, and other items can be exported for external use  |
| F2  | Metadata can be added to data & workflows (e.g. tags, annotations, descriptions)  |
| F3  | Guidance or tools are provided to support FAIR workflow creation/export (e.g. tutorials on making data/workflows FAIR, tools to enable preparation and export to ROCrate, WorkflowHub etc.)   |
| F4  | Interoperability is supported (e.g. import/export of workflows between other workflow systems or in standard formats such as CWL, WDL)  |
| F5  | Workflows can be shared through an official or community repository or workflow library  |

### Reproducibility

| Criterion | Definition  |
|---|---|
| R1  | Details of the analysis including tools, versions & parameters are recorded  |
| R2  | Executable records of workflows are available (code or scripts that can be reused to replicate or rerun analyses, rather than execution histories alone)  |
| R3  | Workflows can be versioned to track changes  |
| R4  | Human-readable reports including provenance and outputs can be generated automatically  |
| R5  | Previous versions of the tools or execution environment can be accessed or recreated  |


### Flexibility-Support Criteria

| Criterion | Flexible | Balanced | Supportive |
|-----|-----|-----|-----|
| FS1: Platform openness and control | Open-source platform that anyone can install, modify, and contribute to | Both managed and self-hosted versions are available | Fully managed platform with limited or no ability for users to modify the underlying system |
| FS2: Environment and infrastructure control | Users are responsible for managing the execution environment (e.g. dependencies, workflow engine, cloud/HPC configuration) | Platform supports both managed and user-controlled environments | Platform provides a fully managed execution environment with minimal user configuration (e.g. one installation, hosted online) |
| FS3: Tool integration and extensibility | Users can freely add or run custom tools/scripts (e.g. R, Python, bash tools) | Custom tools can be added alongside pre-installed tools, but with some restraints (e.g. wrapping,  registration, review by platform developers) | Users are limited to a curated set of pre-installed tools, with new tools only added by platform developers |
| FS4: Parameter control and guidance | Full access to all parameters with limited guidance or constraints | Advanced parameters available but partially guided (e.g. defaults provided, advanced options separated) | Strong guidance provided (e.g. recommended defaults, restricted inputs, simplified parameter interfaces) |
| FS5: User support and guidance | Minimal structured support (e.g. documentation only or developer contact provided) - typically focusing on the WMS itself rather than supporting users with analyses | Support available but limited or conditional (e.g. community forums) | Active support ecosystem (e.g. monitored forums, responsive support channels, helpdesk, may be a paid service) |
