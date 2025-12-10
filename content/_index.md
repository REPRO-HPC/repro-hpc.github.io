+++
title = "Workshop in Reproducibility at ISC26"
+++

Reproducibility is a cornerstone for trustworthy and robust scientific progress.

The High-Performance Computing (HPC) community often faces reproducibility challenges due to complex software stacks, cutting-edge hardware, and costly operations (computations, data transfers, etc.).
The reproducibility challenges could also be explained by a lack of education on what reproducibility is, a lack of tools offered by the platforms to support reproducibility, inconsistencies in the various venues' guidelines for packaging the artifacts, or a lack of incentives for the authors to make an extra effort.

Overall, reproducibility in HPC is mostly a **methodological and technical problem, which can only be addressed by gathering the community and discussing all together about the way forward**.

This workshop brings together the HPC community (researchers, practitioners, platform providers, and educators) to share their feedback, tools, and best practices to tackle the reproducibility hurdles met in HPC.

{{ new_block() }}

# Workshop Topics

The topics of interest of the workshop include, but are not limited to, the following:

### General

- Feedback/Lessons learned/Success stories from artifact authors, reviewers, and chairs, trying to package an experiment or trying to reproduce an experiment
- Methods to create a "minimal reproducible experiment" to proxy the reproduction on the energy consuming full-scale version
- Energy-efficient artifact reproduction in HPC
- Case studies of sustainable (or unsustainable) artifact evaluation in HPC
- Long-term reproducibility: ensuring artifacts remain accessible and evaluable as hardware/software evolves
- Feedback from teaching HPC reproducibility principles
- Reproducibility in the age of AI: concerns and opportunities
 
### Software Environment / Workflow / CI/CD

- Methods and tools to create a standalone and portable experiments (package managers, containers,...)
- Methods and tools to support reproducibility in HPC from the early development stages (CI/CD, provenance, SBOM, ...)
- Methods and tools to support FAIR principles
 
### Platforms (HPC Centers and Testbeds)

- Tools and services that should be offered by HPC centers and testbeds to improve/support reproducibility
- Billing, access, and "security" to HPC centers and testbeds for reproduction attempts
 
### Artifact Evaluation Process

- Proposals for new Artifact Evaluation processes (timelines, badges, reports, interactions between authors and reviewers, reviewer roles, etc.)
- Incentives and recognition for Reproducibility in HPC (for authors and reviewers)
- Human-centric sustainability: reducing reviewer/author fatigue and chair workload
- Community standards for balancing rigor, efficiency, and human effort
- "Proper" evaluation of proprietary software/hardware


{{ new_block() }}


# Invited Speakers

{{ grid(
    text = [
        ["Speaker A","Institution A"], 
        ["Speaker B","Institution B"],
    ],
    urls = [
        "https://aterenin.github.io/academic-workshop#speaker_a",
        "https://aterenin.github.io/academic-workshop#speaker_b",
    ],
    images = [
        "placeholder.svg",
        "placeholder.svg",
    ],
    narrow = false) }}


{{ new_block() }}

# Program at Glance

| Time (CET)    | Event                     |
| ------------- | ------------------------- |
| 09:00 - 09:10 | Welcome and Introductions |
| 09:10 - 09:50 | Invited Talk #1           |
| 09:50 - 10:05 | Contributed Talk #1       |
| 10:05 - 10:20 | Contributed Talk #2       |
| 10:20 - 11:00 | Invited Talk #2           |
| 11:00 - 11:30 | *ISC Coffee Break*        |
| 11:30 - 11:45 | Contributed Talk #3       |
| 11:45 - 12:00 | Contributed Talk #4       |
| 12:00 - 13:00 | Panel Discussion          | 

[more details](/program)


{{ new_block() }}


# Accepted Contributions

{{ table(
    data = "papers.csv", 
    columns = ["Title","Authors"],
    button_names = ["abstract","slides"], 
    button_data_columns = [3,4], 
    button_output_columns = [1,1]) }}



{{ new_block() }}
