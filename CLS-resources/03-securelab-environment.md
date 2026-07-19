# SecureLab environment

Primary reference: UKDS SecureLab User Guide, version 11.08, April 2026: https://ukdataservice.ac.uk/app/uploads/sa_user_guide.pdf (stable short link: https://ukdataservice.ac.uk/sa_user_guide). Covers logging on, account drives, importing files, output requests, and software specifics.

Overview pages:

- What is SecureLab: https://ukdataservice.ac.uk/help/secure-lab/what-is-securelab/
- SecureLab help index: https://ukdataservice.ac.uk/help/secure-lab/
- General SecureLab FAQs: https://ukdataservice.ac.uk/help/secure-lab/securelab-faqs/
- Five Safes framework: https://ukdataservice.ac.uk/help/secure-lab/what-is-the-five-safes-framework/

## Access routes

Access is remote via Citrix Workspace from an institution-managed device on an approved IP address, over wired Ethernet or WPA2/3 institutional wireless. Personal devices are prohibited. Alternatives: SafePod Network (https://safepodnetwork.ac.uk/safepod/), the UK Data Archive Safe Room at Essex, and for some datasets home working under a specific agreement (https://ukdataservice.ac.uk/help/homeworking/securelab-working-from-home/). Non-ONS data (CLS is DCMS-owned, i.e. non-ONS) home access conditions: https://ukdataservice.ac.uk/find-data/access-conditions/apply-to-access-controlled-data-in-secure-lab/apply-to-access-non-ons-data/ and https://ukdataservice.ac.uk/app/uploads/securelab-access-to-non-ons-data.pdf

Data handling and security guide: https://ukdataservice.ac.uk/app/uploads/cd171-researchdatahandling.pdf

There is no charge for SecureLab; it is ESRC/UKRI funded.

## Environment characteristics

- Windows-based remote desktop, no internet connectivity inside the environment.
- Personal M: drive; shared project folders for co-researchers on the same approved project; References (R:) drive holding user guides, Stata ADO files and the R package repository; an SDC folder inside the project folder for output submissions.
- All work from exploration to final paper is done inside SecureLab. There is no two-tier intermediate/final output system; colleagues on the same project view results in the shared project folder.
- Long-running jobs: disconnect (not log off) to leave e.g. a multi-hour Stata or R job running.
- Copying anything from the screen is forbidden; downloads are impossible.

## Software available as standard (per SecureLab FAQs, May 2026)

7zip, Acrobat Reader, Anaconda Navigator, Anaconda Prompt, File Explorer, Git for Windows, JASP, Jupyter Notebook, Microsoft R Open, Microsoft Word, MLWin, Mplus, Notepad++, PowerPoint, QGIS Desktop, R, R Studio, Sourcetree, SPSS, Spyder (Anaconda3), Stata, TeXworks Editor.

Other applications can be requested via the helpdesk; installation is at UKDS discretion.

## R specifics

- A local CRAN mirror is on the References drive, updated weekly. Installation instructions: SecureLab folder `References$\User_Guide\Guide to working with R packages in SecureLab`.
- Non-CRAN packages can be requested for import but are checked one-by-one; the process is slow. Plan package dependencies against CRAN before going on-TRE.
- Git for Windows and Sourcetree exist inside the environment, but with no internet there is no remote push/pull; repositories are local-only. Syntax must enter via the import procedure and leave via output release (see `04-outputs-and-sdc.md` and `05-import-support-contacts.md`).

## Stata specifics

- ADO files: check `R:\ADO_Files\` on the References drive; set `adopath ++ R:\ADO_Files\`. Missing ADOs can be requested. See the 'Stata path directory for ado files' document in the same location.

## Differences from ONS SRS

Login from the institution rather than an ONS safe room; single-tier outputs. UKDS states economic and social data in the SRS are also to be available via SecureLab. Reference: https://ukdataservice.ac.uk/help/secure-lab/securelab-faqs/
