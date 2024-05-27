# SimpleELN-Documentation

Welcome to the **SimpleELN** user guide! 

**SimpleELN** is a user-friendly electronic laboratory notebook (ELN) system that allows researchers to securely store, organize, and share their research data and notes. This document will provide you with step-by-step tutorials to help you get started with SimpleELN and utilize its features efficiently.

Thank you for giving the **SimpleELN** web server a chance to demonstrate its capabilities and functionality. We appreciate your interest and hope you find it useful for your research and documentation needs.

[SimpleELN Documentation](https://simpleeln-documentation.readthedocs.io/en/latest/index.html).

## Edition

  - Personal Edition
    
    The Personal Edition is tailored for individual users, empowering them to create and manage their own experimental records. This edition is ideal for personal use as it ensures enhanced data security and provides a user-friendly experience during installation and daily use.
  - Team Edition
    
    The Team Edition is suitable for team-based groups, where one team account with a team admin role and multiple team user accounts can be created. This edition is ideal for multi-user single laboratories or organizations that require collaboration between team users.
  - MultiTeam Edition
    
    The MultiTeam Edition is tailored for departments, centers, companies, organizations, and other entities that encompass multiple independent team groups. This edition is particularly beneficial for multi-team laboratories or organizations that require collaboration between teams or users.

## Description

Source files: [SimpleELN-Team/SimpleELN-Documentation/edit/main/source](https://github.com/SimpleELN-Team/SimpleELN-Documentation/tree/main/source).

## Installation

~~~bash
git clone https://github.com/SimpleELN-Team/SimpleELN-Documentation
cd SimpleELN-Documentation
pip install --user sphinx sphinx_rtd_theme myst-parser sphinx-autobuild sphinx-design
~~~

## Generate the HTML documentation:

~~~bash
sphinx-build -M html source/ build/
~~~

Then point your browser to the `build/html/index.html` file.

The pre-generated documentation can also be conveniently accessed via the `html/index.html` file.

