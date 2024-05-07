# SimpleELN-Documentation

Welcome to the **SimpleELN** user guide! 

**SimpleELN** is a user-friendly electronic laboratory notebook (ELN) system that allows researchers to securely store, organize, and share their research data and notes. This document will provide you with step-by-step tutorials to help you get started with SimpleELN and utilize its features efficiently.

Thank you for giving the **SimpleELN** web server a chance to demonstrate its capabilities and functionality. We appreciate your interest and hope you find it useful for your research and documentation needs.

[SimpelELN Documentation](https://simpleeln-documentation.readthedocs.io/en/latest/index.html).

## Description

Source files: [SimpelELN-Team/SimpleELN-Documentation/edit/main/source](https://github.com/SimpelELN-Team/SimpleELN-Documentation/tree/main/source).

## Installation

~~~bash
git clone https://github.com/SimpelELN-Team/SimpleELN-Documentation
cd SimpleELN-Documentation
pip install --user sphinx sphinx_rtd_theme myst-parser sphinx-autobuild sphinx-design
~~~

## Generate the HTML documentation:

~~~bash
sphinx-build -M html source/ build/
~~~

Then point your browser to the `build/html/index.html` file.

The pre-generated documentation can conveniently be accessed via `html/index.html` file.

