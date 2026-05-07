
Automating Network Configuration Management in the MOD: A NetDevOps Approach


Overview

This repository contains the practical artefacts, source code, and supporting materials developed as part of a Level 6 BSc (Hons) Information Technology & Communication final‑year project at Staffordshire University.
The project investigates how NetDevOps principles and network automation tooling can be applied to modernise network configuration management within a Ministry of Defence (MOD) enterprise context. Traditional manual configuration methods were evaluated against automated approaches to assess improvements in efficiency, reliability, repeatability, and operational confidence.
All work in this repository was developed and tested exclusively in lab and sandbox environments. No live MOD network configurations or sensitive data are included.


Project Aims

The primary aims of this project were to:

Investigate current challenges with manual network configuration management

Design and implement an automated configuration management framework using NetDevOps practices

Compare manual CLI‑based configuration with automated approaches using measurable performance metrics

Validate automated changes using structured testing and verification tools

Evaluate the technical and organisational implications of NetDevOps adoption within Defence environments


Technologies and Tools Used

The repository reflects industry‑aligned NetDevOps tooling and practices, including:

Linux (Ubuntu) – automation controller environment

Ansible – network configuration automation (agentless via SSH)

Python – supporting automation and validation tooling

PyATS – automated validation and configuration state comparison

YAML – data serialisation for Ansible playbooks

Git & GitHub – version control and change tracking

Cisco IOS (CML) – virtualised network devices for lab testing

Learning and tool selection were informed by structured study aligned to the Cisco CCNP DevNet Professional – AUTOCOR blueprint.


Repository Structure

The repository is organised to reflect the development and testing workflow adopted during the project

Folder names may evolve as the project was developed iteratively. All core automation and validation artefacts are preserved for reproducibility.


Key Features Demonstrated

Automated configuration of Cisco IOS devices using Ansible

Idempotent execution to prevent configuration drift

Performance comparison between manual and automated deployment

Automated validation of network state using PyATS

Version‑controlled infrastructure changes

Clear separation between automation logic, inventories, and variables



Security and Ethical Considerations

All configurations are fictional or lab‑generated

No MOD production data, credentials, or network details are included

Plain‑text credentials used in the repository are for academic demonstration only

In production environments, secure mechanisms such as Ansible Vault or external secrets managers would be required


Academic Context

This repository supports the accompanying project report:

Automating Network Configuration Management in the MOD: A NetDevOps Approach
Luke Gilmore – BSc (Hons) Information Technology & Communication
Staffordshire University


The report provides full academic context, methodology, results analysis, discussion, and conclusions. This repository should be viewed as the practical implementation evidence underpinning that report.


How to Use (Lab Environment Only)

This project is intended for educational and experimental use only.

To reproduce elements of the project:

Deploy a Linux controller (Ubuntu recommended)

Install Ansible, Python, and required collections/modules

Deploy Cisco IOS devices using Cisco Modelling Labs (CML) or DevNet sandboxes

Update inventory files with lab IP addresses

Execute playbooks from the ansible/playbooks/ directory

Use PyATS to capture and compare device state before and after changes


Future Improvements

Potential extensions to this work include:

Integration with a full CI/CD pipeline (GitHub Actions / GitLab CI)

Secure credential management using Ansible Vault

Declarative, model‑driven automation using YANG and RESTCONF

Multi‑vendor device support

Role‑based web front‑end for controlled automation execution


Disclaimer

This repository is part of an academic submission. It does not represent an operational MOD system and should not be deployed in production environments without appropriate security, governance, and organisational approval.


Author
Luke Gilmore
FdSc Information Technology & Communication
University of Staffordshire
