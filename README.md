# Deeply-Sourced Seeps Field Sampling Framework
[![CC BY](https://forthebadge.com/images/badges/cc-by.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Powered by Coffee](https://forthebadge.com/images/badges/powered-by-coffee.svg)](https://forthebadge.com/)
[![Built with Science](https://forthebadge.com/images/badges/built-with-science.svg)](https://forthebadge.com/)

[![Giovannelli Lab](https://img.shields.io/badge/BY-Giovannelli_Lab-blue)](https://dgiovannelli.github.io/)
![In the Field](https://img.shields.io/badge/MADE-In_the_Field-yellowgreen)
[![Funded by ERC](https://img.shields.io/badge/Funded%20by-ERC-ff6400.svg)](https://erc.europa.eu/)
[![ERC CoEvolve](https://img.shields.io/badge/Project-ERC%20CoEvolve-000fa9.svg)](https://www.coevolve.eu/)
![Sweat & Mosquitoes](https://img.shields.io/badge/Made_with-Sweat_%26_Mosquitoes-red.svg)
![Field Tested](https://img.shields.io/badge/Field_tested-From_Arctic_to_Tropics-informational)
![Field Tested](https://img.shields.io/badge/Field_tested-Mud%2C_Gas_%26_Bad_Weather-brown)
![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)

Field-ready protocols, templates, scoring tools, and supporting resources for standardized synoptic sampling of deeply-sourced seeps and the study of subsurface geosphere–biosphere interactions.

## About this repository

This repository provides the field-ready resources associated with our standardized framework for sampling deeply-sourced thermal springs and natural seeps as access points to subsurface systems.

The framework was developed across multiple field programs to support synoptic, co-located collection of microbiological, geochemical, geological, and environmental data while maintaining sample traceability across field operations, analytical workflows, and data repositories. The complete rationale and Standard Operating Procedure (SOP) are described in the associated manuscript:

> Giovannelli D., Jessen G.L., de Moor J.M., Barry P.H., Lloyd K.G.. 2026. A standardized field framework for integrated microbiological and geochemical sampling of  deeply-sourced seeps across large-scale geological gradients. _Open Research Europe, submitted_
> [DOI]

This repository is the operational companion to the published SOP. It contains printable field resources, templates, coding systems, examples, and supporting material that can be used directly during expedition planning, sampling, and subsequent data management.

The framework reflects the workflow developed for our specific scientific questions, particularly the investigation of geosphere–biosphere interactions through deeply-sourced seeps. It is intentionally modular, and many of its components can be adapted to other environments and research questions requiring standardized, synoptic, co-located sampling across multiple matrices, campaigns, and laboratories.

## Going to the field?

If you are leaving tomorrow and do not have time to read everything, start here:

1. **Read the SOP** — preferably before step 2.
2. **Print the Field Log** — one for each planned sampling event, plus extras. There are never enough extras.
3. **Print or laminate the Field Hazard Card and Risk Matrix** — for standardized recording of site hazards and operational risk.
4. **Print or laminate the MatType Card** — for consistent description of microbial mats at the sampling location.
5. **Check the Sampling Series** — prepare and pre-label containers before deployment.
6. **Check the vial-label examples** — particularly if multiple laboratories or operators are preparing sampling material.
7. **Take the Subsurface Confidence Matrix with you** — several of the required proxies depend on field measurements and observations that cannot be reconstructed later.
8. **Check the equipment and expedition-support lists** — including the Remote Area Field Aid Kit (RAFAK) where appropriate.

The paper explains *why*. This repository is mostly about *how*.

## Repository contents

### Field logs

Printable and editable field logs used to record each sampling event. The field log links the CollectionID to geographic position, environmental conditions, physicochemical measurements, field geochemistry, collected samples, photographs, spatial datasets, and field observations.

Where provided, completed examples illustrate how the log is used under actual field conditions.

### Sampling series and checklists

Reference material for assembling the standard sampling series before deployment, including required containers, preservation reagents, sample volumes, storage requirements, and analytical destinations.

The series should be adapted to the scientific objectives of each campaign while preserving the relationship between the sampling event, physical sample, and analytical fractions.

### Sample and vial labels

Examples of field labels for samples, analytical fractions, and individual containers are provided to illustrate the implementation of the identifier architecture.

The SampleID identifies the physical sampled material associated with a CollectionID. Secondary operational codes such as `GEO`, `ISO`, `PCF`, and other analysis-specific labels identify containers or analytical fractions derived from that sample and do not become part of the SampleID.

The examples are intended as practical guidance rather than mandatory label layouts. Label size, material, printer technology, and information density can be adapted to the containers and field conditions used by individual teams.

### Field Hazard Card and Risk Matrix

The hazardCode provides a compact field descriptor of site characteristics and operational hazards encountered during seep sampling. The accompanying reference card and risk matrix support consistent assignment and interpretation of the code during field operations.

The hazardCode is a project-specific field tool. It does **not** replace expedition-specific risk assessment, institutional safety procedures, appropriate training, or professional judgment.

If the matrix says you should not sample something, finding a more adventurous postdoc is not an acceptable mitigation strategy.

### Microbial mat descriptor

The MatType reference card provides a standardized three-character descriptor for recording the dominant color, physical structure, and putative metabolic association of microbial mats observed at the sampling location.

Putative metabolic associations are field observations, not functional assignments. They should be evaluated subsequently using geochemical, molecular, and other analytical evidence.

### Subsurface confidence assessment

The multi-proxy framework evaluates the degree to which a sample preserves evidence of a subsurface signal relative to surface influence.

Individual interpretable proxies are scored from −1 to +1 and combined into a normalized subsurface confidence score constrained between −1 and +1. The score should always be retained together with the individual proxy values and proxy coverage, for example:

`S_norm = 0.60; 5/7 proxies evaluated`

At least five complementary proxies are recommended for robust assessment. Formal classification requires at least three interpretable proxies spanning two independent evidence domains. Missing or uninterpretable proxies are not equivalent to an intermediate score of zero.

The scoring framework is an operational evidence-synthesis tool. It is not a quantitative estimate of the fraction of subsurface fluid in a sample and is not currently a statistically calibrated or differentially weighted index. See the associated paper for the complete rationale, scoring criteria, and limitations.

### Remote Area Field Aid Kit (RAFAK)

The repository includes the contents and organization of the **Remote Area Field Aid Kit (RAFAK)** used to support field campaigns in remote environments.

The RAFAK material is provided as an expedition-planning resource and is not part of the scientific sampling SOP itself. Its contents should be adapted to expedition duration, remoteness, environmental conditions, team composition, available evacuation infrastructure, institutional requirements, and the training and qualifications of field personnel.

It is not a substitute for appropriate medical advice, expedition risk assessment, first-aid training, or emergency planning.

### Protocols and QA/QC tools

Additional protocols, data-validation resources, and QA/QC tools associated with the framework will be released in a dedicated repository as they are developed and tested.

## Know your codes

Several coding systems coexist in the framework because they describe different things.

**Sample identifiers** (`ExpID → SiteID → CollectionID → SampleID`) track the identity and provenance of physical samples.

**Operational codes** (`GEO`, `ISO`, `PCF`, etc.) identify analytical fractions, containers, or downstream workflows associated with those samples. They are not part of the SampleID.

**Field descriptors** (`hazardCode`, `MatType`) encode standardized observations made at the sampling location.

Keeping these functions separate prevents identifiers from becoming progressively longer descriptions of everything anyone has ever done to a sample.

If you are tempted to encode additional information directly into the SampleID, resist.

## Core principles

The individual protocols can be modified, but we recommend preserving several principles when adapting the framework:

* sample geological gradients rather than treating sites as isolated observations;
* collect biological, geochemical, and environmental measurements synoptically and as closely co-located as possible;
* target the least-mixed accessible expression of the source fluid;
* characterize the local surface background;
* separate sample identity from analytical and descriptive metadata;
* record deviations, failed measurements, and missing samples explicitly;
* preserve the relationship between a CollectionID and all samples and analytical fractions derived from that event;
* assess subsurface signal preservation using multiple independent lines of evidence rather than a single proxy;
* retain field context alongside analytical data.

Standardization does not mean pretending every seep is the same. It means documenting differences without losing the ability to compare them.

## Suggested repository structure

```text
/
├── README.md
├── LICENSE
│
├── field-logs/
│   ├── field-log-printable.pdf
│   └── field-log-editable.*
│
├── field-cards/
│   ├── hazard-code-card.pdf
│   ├── hazard-risk-matrix.pdf
│   ├── mat-type-card.pdf
│   └── subsurface-confidence-card.pdf
│
├── sampling/
│   ├── sampling-series-checklist.pdf
│   ├── sample-labeling-guide.pdf
│   ├── vial-label-examples.pdf
│   └── equipment-checklist.pdf
│
├── expedition-support/
│   └── RAFAK/
│       ├── RAFAK-contents.pdf
│       └── README.md
│
├── protocols/
    └── ...
```

The exact directory structure may evolve as additional resources are added.

## Versions, releases, and citation

This GitHub repository contains the actively maintained version of the framework. Field protocols evolve: equipment changes, new environments expose weaknesses, and occasionally something that looked perfectly sensible behind a desk turns out to be ridiculous in a swamp.

Stable releases associated with publications or major framework versions are archived through Zenodo and assigned a DOI.

If you use these resources in published work, please cite both the associated paper and the specific archived release used for your field campaign.

## Adapting the framework

You are welcome to adapt individual components of the framework to different environments, analytical workflows, and scientific questions.

When doing so, document modifications explicitly. In particular, changes to identifier definitions, controlled vocabularies, scoring criteria, or proxy thresholds should be recorded with the resulting dataset. Two datasets using similarly named codes but different underlying definitions are considerably harder to integrate than two datasets that openly document their differences.

Where possible, retain the original field definitions alongside modified or extended fields to facilitate interoperability.

## Found something that does not work in the field?

Good. Tell us.

This framework was built through repeated field use and is expected to evolve. If a field sheet is confusing, a category does not describe what you encountered, a protocol fails under particular environmental conditions, or you have developed a better solution, open an issue and describe the problem and the setting in which it occurred.

We are particularly interested in applications outside the geological and environmental settings in which the framework was originally developed.

Bug reports involving mud, rain, volcanic gases, frozen equipment, boats, questionable roads, or unexpected animals are entirely legitimate bug reports.

## Contributing

Suggestions, corrections, additional field-tested solutions, and documented extensions are welcome through GitHub issues and pull requests.

For substantive changes to the identifier architecture, hazard classification, MatType descriptors, or subsurface confidence framework, please describe the rationale and provide examples or data supporting the proposed modification. These components affect interoperability among campaigns and should therefore evolve conservatively.

## License

Unless otherwise specified, documentation, templates, field cards, figures, and other reusable materials in this repository are released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.

Software and source code, where provided, may be distributed under a separate software license specified within the corresponding directory.

Please attribute the framework and cite the associated publication and archived release when reusing or adapting these materials.

## Acknowledgements

This framework was developed through multiple field campaigns and collaborative research projects involving researchers, students, field technicians, local collaborators, institutions, and communities across a wide range of geological settings.

Development of the framework was supported in part by the European Research Council through the **ERC CoEvolve** project and by the additional projects and programs acknowledged in the associated publication.

Many of the procedures provided here exist because something, somewhere, once went wrong in the field. **We thank everyone who helped us figure out why.**
