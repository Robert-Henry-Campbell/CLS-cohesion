# CLS documentation

## 2024/25 (matches Secure Access SN 9515 fieldwork period)

Annual publication page (all documents): https://www.gov.uk/government/statistics/community-life-survey-202425-annual-publication

- Technical report (methodology, sampling, response, weighting): https://www.gov.uk/government/statistics/community-life-survey-202425-annual-publication/community-life-survey-202425-technical-report
- Appendix A, Online questionnaire (PDF, 78 pp): https://assets.publishing.service.gov.uk/media/693047dd502f392086ee8b47/CL24_25_Q1_online_questionnaire_v4__Clean_.docx.pdf
- Appendix B, Paper questionnaire (PDF, 23 pp): https://assets.publishing.service.gov.uk/media/693047f5502f392086ee8b49/Community_Life_Questionnaire_2024_Verian_R1_PROOF.pdf
- Appendix D, Derived variables: https://www.gov.uk/government/statistics/community-life-survey-202425-annual-publication/community-life-survey-202425-appendix-d-derived-variables
- Guidance for interpreting these statistics: https://www.gov.uk/government/statistics/community-life-survey-202425-annual-publication/community-life-survey-202425-guidance-for-interpreting-these-statistics
- Annual data tables (ODS, 2.76 MB): https://assets.publishing.service.gov.uk/media/694144ce1ec67214e98f2f8f/Community_Life_Survey_2024_25_Annual_data_tables.FINAL.ods
- Headline findings and topic reports (loneliness and support networks; neighbourhood and community; civic engagement and social action; volunteering and charitable giving): linked from the annual publication page.

Quarterly publications for 2024/25: Oct-Dec 2024 (https://www.gov.uk/government/statistics/community-life-survey-october-to-december-2024-quarterly-release) and Jan-Mar 2025 (https://www.gov.uk/government/statistics/community-life-survey-january-to-march-2025-quarterly-publication).

## Other survey years

- GOV.UK collection (annual releases 2016-17 to 2024/25, quarterly releases, focus reports, methodology reports): https://www.gov.uk/government/collections/community-life-survey--2
- 2012-13 to 2015-16 releases and questionnaires: https://www.gov.uk/government/collections/community-life-survey
- 2023/24 annual publication: https://www.gov.uk/government/statistics/community-life-survey-202324-annual-publication
- Example earlier technical report, 2020/21 (Kantar Public, PDF): https://doc.ukdataservice.ac.uk/doc/8867/mrdoc/pdf/8867_community_life_technical_report_2020-21.pdf
- Ad-hoc statistical releases: https://www.gov.uk/government/statistical-data-sets/dcms-community-life-survey-ad-hoc-statistical-releases
- Methodology reports: paper questionnaire provision effects (https://www.gov.uk/government/publications/community-life-survey-what-difference-does-the-provision-of-paper-questionnaires-make-to-the-community-life-survey-sample-and-results) and within-household sampling study (https://www.gov.uk/government/publications/community-life-survey-within-household-sampling-comparative-study)

Per-study documentation (user guides, questionnaires, technical reports) is also attached to each UKDS catalogue record under its documentation section; PDFs are served from doc.ukdataservice.ac.uk/doc/<SN>/.

## UKDS quick start guide

https://ukdataservice.ac.uk/learning-hub/students/resources/quick-start-cls/

Summarises design, topics, routing ("Item not applicable" missing codes), and weighting.

## Weighting (from the quick start guide; variable names as in the 2020-21 dataset)

Online + paper combined:

- `SRCaliw`: design, non-response and calibration adjustments (default choice for full-sample analysis)
- `RespondentCalibrationWeight`: design and calibration
- `StandardisedBaseWeight`: design only
- `StandardisedAddressSamplingWeight`: address non-response only

Online-only:

- `SRCaliww`, `RespondentCalibrationWeight_web`, `StandardisedBaseWeight_web`

Calibration factors: ethnic group, region, housing tenure, household size, gender by age group, education by age group, internet use by age group. Confirm names and any changes for 2023/24-2024/25 in the 2024/25 technical report; the boosted LA-level design altered sampling and may alter weighting specification.

## Sampling design notes (for survey-weighted analysis code)

Address-based online surveying (ABOS), Postcode Address File frame, stratified random sampling with differential sampling fractions by stratum (primary strata based on ethnic mix). Design details per year are in each technical report.
