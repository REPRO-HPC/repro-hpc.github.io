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
        ["Kate Keahey","ANL / UChicago", "Practical Reproducibility: How AI Can Help Make You a Better Scientist"], 
        ["Helena Vela Beltran","Do IT Now", "EESSI: Addressing HPC Reproducibility Hurdles Through a Unified Software Stack"],
    ],
    urls = [
        "https://www.mcs.anl.gov/~keahey/",
        "https://www.linkedin.com/in/torri1"
    ],
    image_dir = "speakers",
    narrow = false) }}

{{ new_block() }}

# Program

**Friday June 26th 2026 -- Hall X8, 1st Floor**:

<div class="program-table">


| Time (CET)    | Event                             |
| ------------- | --------------------------------- |
| 09:00 - 09:05 | Welcome and Introductions ([slides](/intro-slides.pdf))        |
| 09:05 - 09:40 | Invited Talk : **Kate Keahey** -- *"Practical Reproducibility: How AI Can Help Make You a Better Scientist"* <details><summary>See abstract</summary> Reproducibility is increasingly fundamental to scientific discourse as a means to promote trust in scientific results. There is however another compelling application of reproducibility: enabling new discoveries and new science through direct experimentation with existing results. I argue that using this practical application reproducibility as a mainstream method of scientific exploration – enhancing the means of discourse that today primarily consists of writing and reading papers -- will not only enable more intuitive understanding of new results but also lead to greater scientific productivity. <br><br> However, the question arises whether this “practical reproducibility” is in fact practical in the sense that it can be implemented at sufficient scales and such that it is available to everyone. Hardware availability, lack of libraries of digital artifacts -- and, most importantly, the effort and attention required to frame and package computational experiments for reproducibility given inadequate ecosystem support for such endeavors – all pose serious challenges to this vision. <br><br> In this talk, I will describe the advantages and challenges of practical reproducibility and propose solutions that leverage recent technological advances, notably ways in which we can harness new resource configurations as well as new opportunities that became available with the advent of AI. I will also describe how we are applying those solutions in the context of Chameleon, a resource uniquely configured to support experimentation in computer science, that over the last 10 years of its existence served a community of over 14,000 users that collectively produced over 1,200 publications.</details>|
| 09:40 - 09:55 | *"Layered Reproducibility for High-Performance Computing Applications: The Feel++ and Ktirio Urban Buildings Case Study"* <br>-- J. Cladella, V. Chabannes, C. Prud'homme <br><details><summary>See abstract</summary> The High-Performance Computing (HPC) community struggles with reproducibility due to complex software stacks, heterogeneous hardware, and expensive validation cycles. This contribution presents a layered reproducibility strategy in which Feel++ provides a traceable software supply chain and Ktirio Urban Buildings (KUB) builds on it to manage versioned urban-building data, executable simulations, and checksum-verifiable result artifacts. Feel++ treats continuous integration (CI) plans, CMake presets, packaging manifests, public software metadata, operations commands, containers, software bill of materials (SBOM)/provenance metadata, and Feel++ Benchmarking reports for Feel++ and KUB cases as repository-owned artifacts. KUB applies this foundation to City Energy Model Database (CEMDB) datasets, manifests, Findable, Accessible, Interoperable, and Reusable (FAIR) packaging, and verifiable outputs for computationally expensive simulations. The case study shifts reproducibility from late manual packaging to an artifact chain linking source commits, packages, containers, benchmark configurations, dataset versions, provenance records, and generated results. </details> |
| 09:55 - 10:10 | *"ReVal: A Hardware-Aware LLM Agent for Artifact Reproducibility and Evaluation in HPC Systems"* <br>-- I. Benlamari <br><details><summary>See abstract</summary> Artifact evaluation (AE) is central to the credibility of scientific publications, but it is labor-intensive and scales poorly with rising submission volumes. The problem is most acute in High-Performance Computing (HPC), where heterogeneous hardware, site-specific schedulers, and complex software stacks make out-of-the-box reproduction rare. We present ReVal, an open-source LLM-driven agent for HPC AE that introspects the reviewer’s local node, extracts requirements and claims from the paper and its AD/AE appendix, generates a hardware-aware reproduction script, and executes it inside a fixed container with a bounded fix loop. ReVal is built on open-weight models and aims to assist reviewers as a practical tool, lowering the cost of careful reproduction and contributing to more reliable computational science.</details> |
| 10:10 - 10:25 | *"Standardising HPC Workflows for Sustainable Reproducibility: The JUBE Configuration Artefact Approach"* <br>-- J-O Mirus, F. S. M. Guimaraes, A. Sankaran, M. G. Barrios Sazo, C. Himmels, T. Breuer <br><details><summary>See abstract</summary> As HPC (High Performance Computing) stacks grow increasingly complex, developing applications is becoming more difficult and time-consuming. This complexity, combined with imprecise experiment definitions, threatens scientific integrity and wastes computational and personnel resources. To address these issues, execution steps must be captured in reproducible recipes that are explicit, repeatable, and verifiable. We present JUBE (JUelich Benchmarking Environment) as a standardised, declarative workflow framework that addresses this gap while aligning with the workshop’s emphasis on sustainable practices. Treating JUBE configurations as primary scientific artefacts enables researchers to reduce resource debt, conduct performance regression testing across generations of hardware, and create FAIR-compliant (Findable, Accessible, Interoperable, Reusable) experiment definitions that can be executed for years. We showcase how we successfully employed JUBE to standardise benchmark execution for a variety of applications during the procurement of JUPITER, the first European exascale system, and for reproducible system performance monitoring with continuous benchmarking.</details>|
| 10:25 - 11:00 | Invited Talk : **Helena Vela Beltran** -- *"EESSI: Addressing HPC Reproducibility Hurdles Through a Unified Software Stack"*<details><summary>See abstract</summary>Reproducibility is a cornerstone of trustworthy scientific progress, yet the high-performance computing (HPC) community frequently faces severe reproducibility challenges driven by complex software stacks, rapidly evolving hardware, and a historic lack of standardized deployment tools. To address these technical and methodological hurdles, this session introduces the European Environment for Scientific Software Installation (EESSI), a collaborative initiative designed to streamline how scientific software is deployed, shared, and reproduced across diverse infrastructures, including HPC clusters, cloud platforms, and local workstations. By providing a fully pre-built, module-based, and automated software environment, EESSI eliminates the inconsistencies often found across different platforms, offering a practical tool that helps researchers seamlessly package and replicate their computational environments.</details>     |
| 11:00 - 11:30 | **ISC Coffee Break**              |
| 11:30 - 11:45 | *"Nix to the Rescue for a Reproducible HPC-AI Software Stack"* <br>-- W. Du, J-M. Gratien, R. Gayno, B. Raffin <br><details><summary>See abstract</summary>Reproducibility in HPC remains difficult under the constraints of production supercomputers: no root access, limited internet, and software stacks that increasingly span C/C++, Fortran, Python, MPI, and GPU runtimes. Traditional approaches based on environment modules and Conda require manual intervention to locate dependencies, leak system libraries into builds, and fail to compose across projects. Containers help with deployment but do not by themselves guarantee reproducibility. We report on our experience building a hybrid HPC/AI software stack with Nix, covering local development on a workstation without root and remote deployment as an Apptainer image on a production cluster. Nix's consistent package layout, full environment isolation, and flake-based composition resolve the dependency discovery, leakage, and composition problems we encountered, while unifying C/C++ and Python management under a single declarative specification that also generates the deployment container. We discuss trade-offs against Spack and Guix, the development-versus-production split addressed via CMake presets, and current gaps in ML package coverage in Nixpkgs.</details>|
| 11:45 - 12:00 | *"Some Lessons learnt on FPM promises with NixOS-Compose"* <br>-- A. Salmane, Y. Sun, H. Brunie, O. Richard <br><details><summary>See abstract</summary> Reproducibility in distributed systems research is often treated as an afterthought, and achieving it in practice remains difficult. Functional Package Managers (FPM), and Nix in particular, have emerged as strong candidates for addressing this gap by making system configurations fully declarative and reproducible. NixOS-Compose (NXC) builds on this foundation to target the specific challenge of deploying and reproducing multi- node experiments. In this paper, we report on the use of NXC across a range of use-cases related to different scientific projects. We document where NXC delivers on its reproducibility promise, and where friction remains. Our findings inform a broader question that this paper works toward answering: are functional package managers keeping their promises on reproducibility in distributed systems ?</details>|
| 12:00 - 13:00 | **Panel Discussion**                  |

</div>

## Panelists

- [Kate Keahey](https://www.mcs.anl.gov/~keahey/) ([Chameleon Cloud](https://www.chameleoncloud.org/))
- [Helena Vela Beltran](https://www.linkedin.com/in/torri1) ([EESSI](https://www.eessi.io/))
- [Hatem Ltaief](https://cemse.kaust.edu.sa/profiles/hatem-ltaief) (ISC26 Research Paper Chair) 
- [Olivier Richard](https://datamove.imag.fr/olivier.richard/) ([SLICES-FR](https://slices-fr.eu/en/))

{{ new_block() }}

# Accepted Talks

**Proceedings pre-prints** [**here**](/preprints.pdf)

{{ table(
    data = "papers.csv", 
    columns = ["Title","Authors"],
    button_names = [], 
    button_data_columns = [], 
    button_output_columns = []) }}


{{ new_block() }}

# Call for Contributions

## Submission Format

- Submissions should be either a **2-page abstract** or a **4-page short paper**, excluding references, in the PDF format using the [IEEE double column template](https://www.ieee.org/conferences/publishing/templates)

- Accepted submissions will **not** appear in the ISC26's proceedings, but will be published, alongside the presented slides, on the workshop's webpage, unless explicit opt-out from the authors.

- Accepted submission will have a 15-minute timeslot including presentation and Q&A.

- Submission website: [https://easychair.org/conferences/?conf=reprohpc26](https://easychair.org/conferences/?conf=reprohpc26)

{{ new_block() }}

## Important Dates

- Call for Contributed Talks open: **March 2nd 2026**

- Submissions due: ~~April 17th 2026~~ ~~May 1st 2026 (AOE)~~ **May 6th 2026 (EoB)** (final extension)

- Notifications sent: ~~May 8th 2026~~ **May 20th 2026**

- Program finalized: **May 26th 2026**

- Camera Ready version due: **June 3rd 2026**

- Workshop Date: **June 26th 2026** 

{{ new_block() }}

# Committees

## Organizing Committee

{{ grid(
    text = [
        ["Quentin Guilloteau", "INRIA", "Web Chair"],
        ["Valérie Hayot-Sasson", "ETS Montréal", "Publicity Chair"],
        ["Dennis Hoppe", "HLRS"],
        ["Josef Weidendorfer", "Dresden University of Technology", "Program Chair"],
    ],
    urls = [
        "https://guilloteauq.github.io",
        "https://www.etsmtl.ca/en/study-at-ets/professors/vhayot-sasson",
        "https://www.hlrs.de/people/dennis-hoppe",
        "https://www.ce.cit.tum.de/caps/mitarbeiter/josef-weidendorfer/",
    ],
    image_dir = "organizers") }}


For any questions, please reach us at : [repro-hpc@groupes.renater.fr](mailto:repro-hpc@groupes.renater.fr)

{{ new_block() }}

## Abstract Reviewing Committee

- André Bauer, Illinois Institute of Technology
- Insaf Benlamari, Leibniz Supercomputing Center
- Raphaël Bleuse, Univ. Grenoble Alpes
- Tainā Coleman, San Diego Supercomputer Center
- Ludovic Courtès, INRIA
- Abdullatif  Eymash, HLRS
- Maxime Gonthier, INRIA
- Samuel Grayson, University of Illinois at Urbana-Champaign
- Arjun Parab, Leibniz Supercomputing Centre
- Millian Poquet, Univ. Toulouse III
- Bruno Raffin, INRIA
- Amir Raoofy, Leibniz Supercomputing Centre


{{ new_block() }}

![](ISC_logo.png)
