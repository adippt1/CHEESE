# Contributing to CHEESE

CHEESE is an open-source project, and contributions that improve its
calculations, usability, documentation, or reproducibility are welcome.
Contributions may be submitted through GitHub issues and pull requests.

Please read and follow the project [Code of Conduct](CODE_OF_CONDUCT.md) in all
project interactions.

## Ways to contribute

Useful contributions include:

- Reporting reproducible bugs
- Correcting equations, units, constants, or product-property data
- Improving explanations, documentation, or installation instructions
- Adding validation cases or calculation checks
- Improving accessibility or usability
- Proposing focused features that fit CHEESE's engineering scale-up scope

## Before opening an issue

Search the existing issues to determine whether the question or problem has
already been reported. For substantial features or changes to the calculation
framework, open an issue before writing code so the proposed scope and approach
can be discussed.

Do not submit classified, export-controlled, proprietary, personally
identifiable, or otherwise restricted information. Only include code, data, and
other material that you are authorized to share publicly.

## Reporting a bug

A useful bug report should include:

- The CHEESE version or commit used
- Operating system and Python version
- The interface mode and calculation tab involved
- The input values and units needed to reproduce the problem
- The expected and observed results
- Any warning, traceback, or relevant screenshot

For calculation discrepancies, include a hand calculation, independent
reference, or other basis for the expected result when possible.

## Proposing a calculation change

Changes to equations, constants, unit conversions, or scientific assumptions
should clearly document:

- The equation or value being changed
- Definitions and units for every affected quantity
- The physical or electrochemical basis for the change
- A literature or authoritative data source, when applicable
- At least one worked example or independent validation check
- Any limitations or conditions under which the calculation applies

Update relevant interface explanations and documentation together with the
implementation.

## Pull-request workflow

1. Fork the repository.
2. Create a focused branch from `main`.
3. Make logically organized changes with clear commit messages.
4. Install the dependencies from `requirements.txt`.
5. Start the application with:

   ```bash
   python -m streamlit run CHEESE.py
   ```

6. Exercise the affected workflow in both Simple and Advanced Mode when the
   change could affect shared calculations.
7. Confirm that units, labels, downloaded tables, warnings, and displayed
   equations remain consistent.
8. Update the README or other documentation when behavior or user instructions
   change.
9. Open a pull request with a concise description of the change, its rationale,
   and the checks performed.

Keep pull requests focused. Unrelated refactoring or formatting changes should
be submitted separately.

## Dependency changes

Explain why any new dependency is necessary. Update `requirements.txt` and
`THIRD_PARTY_LICENSES.md`, and identify the dependency's upstream project and
license. Do not add third-party code or data unless its terms permit
redistribution in this repository.

## Licensing of contributions

CHEESE is distributed under the
[BSD 3-Clause License](LICENSE). All new contributions must be made under this
license. By submitting a contribution, you agree that it may be distributed
under the same BSD 3-Clause terms and represent that you have the right to
submit it.

## Questions

Use GitHub issues for public questions about the project. Questions that should
not be posted publicly may be sent to prajapati3@llnl.gov.
