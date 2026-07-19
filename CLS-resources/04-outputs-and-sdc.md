# Output release and statistical disclosure control (SDC)

## Process

1. Save the finished output into the SDC folder of the project area, in a subfolder named `<projectnumber>_YYYY_MM_DD` (underscores, e.g. `998701_2021_03_15`). File names must be meaningful and match the names given on the request form.
2. Submit an output release request via the online form: https://beta.ukdataservice.ac.uk/help?id=outputRelease
3. UKDS staff perform manual SDC checks. Target response: 5 working days; allow longer at busy times.
4. Cleared outputs are emailed to the researcher.

Constraints: one output request at a time per researcher (new requests submitted before the previous concludes are not processed); requests are handled in order of receipt; frequent small requests increase secondary-disclosure risk across releases and are discouraged; be available to discuss or amend problematic items. The request form includes a research-impact question and a tick-box list restating the minimum requirements.

## What counts as an output

Outputs must be of publishable quality, have a specific purpose, and fall within the approved project scope. Permitted types: journal paper, working paper, book/chapter, commissioned/policy report, report to funder, final report, interim report, conference/seminar presentation, dissertation/thesis chapter. Raw data files, Stata .log files, SPSS output files, and R data files are not releasable. Syntax files can be released provided they contain no data and no reference to the SecureLab server name.

Intermediate results are normally shared via the project folder instead of release. Release of intermediate outputs to an external collaborator is possible only if the collaborator is UKDS-registered under the End User Licence and the output is as close as possible to a finished good.

## Minimum requirements for all outputs

- Information on data source, sample and methodology included.
- Unweighted cell counts supplied for everything: tables, percentages, graphs, model results, minima, maxima, medians, scatterplots.
- Threshold rule: minimum of 10 unweighted observations per cell/statistic.
- Graphs and figures as fixed images (e.g. JPEG).
- Tables and figures numbered and labelled; variables given meaningful names, not dataset variable names alone.
- Text explaining what each table/figure shows.
- No embedded documents, invisible content or hidden text (check with Word's Inspect Document).
- Full data citation with DOI included in the output.

Failure on any point sends the request to the back of the queue.

## Guidance documents

- Handbook on Statistical Disclosure Control for Outputs (Safe Data Access Professionals Working Group, v2.0): https://ukdataservice.ac.uk/app/uploads/sdc-handbook-v2.0.pdf — practical rules per statistic type (frequencies, magnitudes, models, survival analysis, etc.).
- Output release checklist for researchers: https://ukdataservice.ac.uk/help/secure-lab/output-release-checklist-for-researchers/
- SecureLab User Guide sections 7 and 14 (dissemination; output requests): https://ukdataservice.ac.uk/app/uploads/sa_user_guide.pdf
- The SDC standards applied follow the European 'Guidelines for the checking of output based on microdata research' (ESSnet SDC); UKDS also provides SDC training to users.

Videos: How to use SecureLab efficiently (https://youtu.be/cSSg_Q21gDM); The 11 most common SecureLab output request issues (https://youtu.be/8S1jPGuA0cE).

## Practical implications for R code written pre-TRE

- Make every table/figure generator also emit unweighted Ns.
- Build in the n>=10 suppression check before formatting results.
- Emit fixed-image graphics and write results into documents with surrounding methodological text rather than raw console output.
- Do not hard-code server paths or names in syntax intended for later release.

## Penalties for breach

Immediate (possibly permanent) termination of access and licence; sanctions sought by the data owner; for data under the Statistics and Registration Service Act 2007, penalties under s39 (fine and/or imprisonment: http://www.legislation.gov.uk/ukpga/2007/18/section/39); individual or institutional suspension from ESRC data services and funding. Self-reported unintentional breaches corrected promptly are treated with discretion.
