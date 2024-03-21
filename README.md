<!--
author:   Joy Payton
email:    k.joy.payton@gmail.com
version:  1.0.1
current_version_description: Initial version
language: en
narrator: UK English Female
title: Pennsylvania Court and Judicial Data
comment: Learn about Pennsylvania court and judicial data.
-->

# Pennsylvania Court and Judicial Data

Information about Pennsylvania Court Data (which includes judicial actions) for the purposes of data and hackathons.

Last updated March 21, 2024.

## About This README

This is the README is written with [LiaScript](https://liascript.github.io/) markdown rendering in mind.  LiaScript has its own [markdown](https://en.wikipedia.org/wiki/Markdown) dialect, so you can read this in the typical markdown way (just read this in GitHub), or you can see it "pretty printed" in the LiaScript rendered format.

To see this document as an interactive LiaScript rendered version, click on the following link/badge:

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/pm0kjp/pa-judicial-data/main/README.md#1)

Why view this in LiaScript?  LiaScript offers helpful tools for usability including pagination, Google Translate, text size and contrast changes, and display format options.  It looks a little nicer than GitHub rendered Markdown, for most users.  There are also some fun LiaScript add-ons like data visualizations.

Alternately, if you're in the LiaScript version already and you want to look at the raw markdown, you can find that at [https://github.com/pm0kjp/pa-judicial-data/blob/main/README.md](https://github.com/pm0kjp/pa-judicial-data/blob/main/README.md).

##  About Judges in Pennsylvania

Judges are elected: but voters don't know squat
-----

Judges are **elected** in the Commonwealth of Pennsylvania in partisan elections.  They also are re-elected, or "retained", in non-partisan elections every 6 or 10 years, depending on their rank.  Appellate court and Courts of Common Pleas judges have a 10 year term, and Magisterial and Philadelphia Municipal Court judges have a 6 year term.  Read more at [https://www.pacourts.us/learn/how-judges-are-elected](https://www.pacourts.us/learn/how-judges-are-elected).  

This is not the only approach to how judges get their jobs.  In other jurisdictions, judges might be  appointed by gubernatorial, legislative, or bar selection: [https://ballotpedia.org/Judicial_election_methods_by_state](https://ballotpedia.org/Judicial_election_methods_by_state).

The fact that we can elect our jurists is a great opportunity for voters to elect judges that reflect their values, whether that's around criminal law, business / civil law, constitutional law, etc.  However, these elections are **low-information**.  

When's the last time you heard ANYTHING about a judicial race?  Maybe you got a flyer from some judges saying they were endorsed by the Bar Association, but that generally only means "this person is adequately prepared for the job" as an attorney in good standing.  It doesn't say anything about what they stand for, their ethics, their politics, their experience or expertise, etc.

Judges are important and impactful!
-----

Judges have HUGE impacts on citizens' lives, especially in criminal court.

Judges have biases, vary in their severity, some are racist.  Some take their jobs seriously and some are shoddy.  Voters don't tend to have ANY info on this.  How can we know if we want to retain a judge?

One answer can be to analyze the **data related to criminal court.**  This is what was done in the [2021 RLadies / JAT Datathon](https://github.com/rladiesPHL/2021_datathon)

Of course, this doesn't answer all the questions we have, especially regarding things like family court (for the protection of families, this data is not public), civil court, Supreme Court, etc.  But criminal court judges are a great place to start with examining the data about how they do their jobs, and making this data understandable and available to voters.  That way we can decide who we want to retain.

### New Judges and JAT 

The [Judge Accountability Table (JAT)](https://judgeaccountabilitytable.org/) was a collaboration between several organizations in Philadelphia County, with the aim of having new judge candidates explain their approach to the bench and make their case to the voters.  They were last active (as near as I can tell) in 2022. 

This was an important moment because the only time that voters pay much attention at all to judicial elections is when judges are first elected.  Judicial retention votes (essentially, re-election) are mostly pro-forma.

I won't go into more detail here about the new judge elections, because this is a largely political and non-quantitative, non-computational project.  Instead, let's pivot to judicial **retention**.

### Judicial Retention

How judges keep their jobs
-----

Judges have to go back on the ballot to keep their jobs in what is known as judicial retention.  These elections are non-partisan, meaning that the political party these judges originally ran under is not disclosed on the ballot.  Voters have no indication of even the basic political orientation of judges seeking retention.

In Pennsylvania, we overwhelmingly retain judges (only one appellate judge has failed a retention vote in decades, not sure about other judges): [https://whyy.org/articles/pennsylvania-election-2023-judicial-retention-superior-court-common-pleas/](https://whyy.org/articles/pennsylvania-election-2023-judicial-retention-superior-court-common-pleas/).

We could help voters change the judiciary!
------

Will supplying voters with information about judges make a difference?  **Yes.**  By supplying voters and organizations with quantitative data about how judges act (in terms of severity, bias, focus on particular crimes, etc.), we know that we can affect electoral outcomes.  

For example: in 2023, Court of Common Pleas judges **Ann Marie Coyle** and **Paula Patrick** were named by Democratic Ward 1, 2, 9,15, and 39a, Reclaim Philadelphia and other progressive organizations in Philadelphia as candidates NOT recommended for retention.  

Additionally, Reclaim Philadelphia recommended "No" retention votes on Superior Court judge **Victor P. Stabile** and Municipal Court judges **Brad Moss**, **William A Meehan Jr.**, and **David C. Shuter**.

These "No" recommendations were not widely known or publicized, as there were other major priorities for Philadelphia political organizations (principally, the mayoral and council races).  Still, despite this being a very quiet anti-endorsement, it made a noticable difference in the [judicial retention vote results](https://philadelphiaresults.azurewebsites.us/ResultsSW.aspx?type=JDR&map=CTY).  While no one failed to retain their seats, the outcomes were significantly different for judges who were targeted for non-retention.

Philadelphia Court of Common Pleas retention vote for 2023:

<!-- data-type="BarChart" -->
| Targeted for Non-Retention? | Candidate | Retention: Yes (%) | Retention: No (%) | Total Number of Votes Cast |
| -- | --- | --- | --- | --- |
|| JACQUELINE F ALLEN | 78.63 | 21.37 | 214,321 |
|| GIOVANNI O CAMPBELL | 75.20 | 24.80 | 203,641 |
| Yes | ANNE MARIE B COYLE | 58.31 | 41.69 | 216,036|
|| RAMY I DJERASSI | 69.29 | 30.71 | 195,375 |
|| JOE FERNANDES | 74.03 | 25.97 | 195,171 |
|| HOLLY J FORD | 74.34 | 25.66 | 194,681 |
|| J SCOTT O'KEEFE | 74.31 | 25.69 | 195,281 |
|Yes| PAULA A PATRICK | 64.89 | 35.11 | 204,518 |
|| SIERRA THOMAS STREET | 77.01 | 22.99 | 205,170|
|| NINA WRIGHT PADILLA | 78.03 | 21.97 | 199,642 |

Philadelphia Municipal Court Retention vote for 2023:

<!-- data-type="BarChart" -->
| Targeted for Non-Retention? |  Candidate | Retention: Yes (%) | Retention: No (%) | Total Number of Votes Cast |
| -- | --- | --- | --- | --- |
|| MARISSA BRUMBACH| 72.37| 27.63 | 207,829 |
|Yes| WILLIAM A MEEHAN JR | 68.42 | 31.58 | 209,331 |
|Yes| BRAD MOSS | 68.45 | 31.55 | 201,895 |
|Yes| DAVID C SHUTER | 63.15| 36.85 | 200,851|
|| KAREN YVETTE SIMMONS | 77.98 | 22.02 | 205,780|
|| MARVIN L WILLIAMS | 75.93 | 24.07 | 199,476|
|| MATT WOLF | 78.67 | 21.33 | 209,706 |


## About the Criminal Legal System

Municipal Court / Magisterial District Court:
----

* Magisterial District Court is the place where lower-level crimes are adjudicated in most counties in Pennsylvania (not Philadelphia County).  Traffic cases and misdemeanor crimes can be fully adjudicated at this level. Magisterial District Judges also set bail and conduct preliminary hearings in misdemeanor and felony criminal cases to determine if the cases should be dismissed or transferred to the Court of Common Pleas for further proceedings.

* Municipal Court is the Philadelphia version of Magisterial District Court.  Municipal Court is the place where lower-level crimes are adjudicated in the City of Philadelphia. Cases that involve only misdemeanor charges are adjudicated entirely in Municipal court, and then the defendant has the option to appeal the decision to the Court of Common Pleas. Cases that involve felonies start in Municipal Court, where the judge makes an initial determination of whether the Commonwealth has shown probable cause that the defendant committed the crimes. If so, the charges are "held for court" and then move on to the Court of Common Pleas.

Court of Common Pleas:
----

* The Court of Common Pleas is the primary trial court in each county in Pennsylvania, including Philadelphia. Criminal cases that involve felonies are adjudicated in the court of common pleas, in addition to appeals from municipal court trials.

Court Docket:
---

* A court docket contains information about a single criminal case that was initiated with a single charging document and usually relates to a single incident, even if it involves multiple criminal charges. It includes a list of hearings and filings in the case and shows the outcome and sentence for each charge.

Court Summary:
---

* A court summary summarizes the criminal record of a particular defendant. It shows the charges and outcome, where applicable, for each of that defendant's cases. Cases that were in Municipal court and then hold for court and transferred to Common Pleas Court will show twice, once for each court. The Court Summary also includes some demographic information about the defendant.

Crime classifications:
----

In order of most serious to least serious, Pennsylvania crime classifications include:

* Murder
* Felony (1st Degree) (F1)
* Felony (2nd Degree) (F2)
* Felony (3rd Degree) (F3)
* Ungraded Felony (F3)
* Misdemeanor (1st Degree) (M1)
* Misdemeanor (2nd Degree) (M2)
* Misdemeanor (3rd Degree) (M3)
* Ungraded Misdemeanor (M3)
* Summary Offenses

* The mandatory minimum and maximum penalties for a criminal conviction depend on the classification of crime. Each criminal classification includes sentencing guidelines, which the court considers in determining the appropriate sentence for an offender. This includes considering the Offense Gravity Score, Prior Record Score, and any enhancements, and aggravating or mitigating circumstances.

## Issues and Questions

The criminal legal system in Pennsylvania (and elsewhere) can show bias.  Things worth studying in the criminal legal system include:

* Patterns in bail -- who is given bail, and how much?  Does this differ across defendant demographics, location in the Commonwealth, type of crime (leaving aside severity, here we mean are different types of non-violent crime treated differently)?
* Patterns in sentencing -- similar questions
* Discretionary power of prosecutors and judges -- what types of crime are presented to the court to begin with?  What types of dismissals, etc. occur?  Does this vary by region, by judge?
* A specific question raised by a Yale researcher I'm working with: "What are the determinants of somebody who gets charged with some sort of drug *distribution* (including possession with intent to distribute) versus just *possession*? As it stands right now, most decriminalization policies (including the former one in Oregon, RIP 😢) only decriminalize simple *possession* of small amounts of drugs or paraphernalia. So it really makes a difference to see, on average, if there are any determinants that make someone more likely to be charged with a distribution charge (e.g. race, use of a public defender, neighborhood of residence) rather than just possession."


## Where's the Data?

We can get public information about judicial actions (sentences, bail, defendant demographics, etc.) in several ways:

* PDFs (Code for Philly did some work with PDFs a few years ago)
* An open API that returns JSON (much easier than screen-scraping PDFs!)
* A data request (costs money). 


###  Pennsylvania Criminal Justice Database

The [Unified Judicial System of Pennyslvania (UGS)](https://ujsportal.pacourts.us/) hosts a centralized database of information about criminal cases in Pennsylvania. This allows interested parties to more easily and accurately compile the data needed to produce research on criminal justice issues in the state.  

The UJS Portal publishes information about individual cases in two formats: a human-friendly PDF file format and a structured machine-friendly file format called JSON ("JavaScript Object Notation") available through an open API ("Application Programming Interface"). An example of the PDF file format can be generated at the following url: [https://ujsportal.pacourts.us/CaseSearch](https://ujsportal.pacourts.us/CaseSearch). 

Court Dockets
-----

If you enter a docket number, for instance MJ-05215-CR-0000031-2019, at the Case Search above and click on the icon of a page with the letter "D" (for docket), you will be redirected to a downloadable PDF like the one at [https://ujsportal.pacourts.us/Report/MdjDocketSheet?docketNumber=MJ-05215-CR-0000031-2019&dnh=E%2Bkk01aSM4Gvu8r8wqYZmg%3D%3D](https://ujsportal.pacourts.us/Report/MdjDocketSheet?docketNumber=MJ-05215-CR-0000031-2019&dnh=E%2Bkk01aSM4Gvu8r8wqYZmg%3D%3D). 


Court Summaries
----

If you enter a docket number, for instance MJ-05215-CR-0000031-2019, at the Case Search above and click on the icon of a courthouse, you will be taken to a court summary PDF, like the one at [https://ujsportal.pacourts.us/Report/MdjCourtSummary?docketNumber=MJ-05215-CR-0000031-2019&dnh=E%2Bkk01aSM4Gvu8r8wqYZmg%3D%3D](https://ujsportal.pacourts.us/Report/MdjCourtSummary?docketNumber=MJ-05215-CR-0000031-2019&dnh=E%2Bkk01aSM4Gvu8r8wqYZmg%3D%3D).

Combined Data
----

To use the API, you'd use the URL `https://services.pacourts.us/public/v1/cases/` followed by a docket number. 

An example of the JSON file format is available here: [https://services.pacourts.us/public/v1/cases/MJ-05215-CR-0000031-2019](https://services.pacourts.us/public/v1/cases/MJ-05215-CR-0000031-2019).

To the best of my knowledge, this combines the data from Court Dockets and Court Summaries into one JSON document.

### About Dockets

Counties Outside of Philadelphia
-----

In counties outside of Philadelphia, the Magisterial District Courts ("MJ") maintain jurisdiction over criminal preliminary arraignments and preliminary hearings, summary criminal offenses, traffic offenses, municipal code violations, landlord / tenant suits, and civil claims where damages do not exceed $12,000. Dockets for such cases have a docket number that looks something like `MJ-05243-CR-0000127-2019`, where:

* `05` represents the district ID number listed [here](http://www.pacourts.us/courts/courts-of-common-pleas/judicial-districts) (in this example, it is the district ID for Allegheny County)
* `243` represents the particular magisterial district court (in this example, it is the district court for Carla M. Swearingen in McKees Rocks, PA)
* `CR` represents a criminal docket type. The Magisterial District Courts also publish dockets for civil (`CV`), traffic (`TR`), and summary offenses (`SA`). 
* `0000127` represents the docket iterator
* `2019` represents the year the docket was initially filed.

More serious criminal cases are transferred to the Court of Common Pleas ("CP") and will have a code similar to `CP-02-CR-0000001-2019`, where the `02` represents the *county* number (not the district ID number) listed [here](http://www.pacourts.us/courts/courts-of-common-pleas/judicial-districts). Such cases will thus have both a MJ and CP docket.

Philadelphia County
------

In Philadelphia County, the Philadelphia Municipal Court ("MC") has initial jurisdiction in processing every criminal arrest in Philadelphia and conducts misdemeanor trials and preliminary hearings for all felony cases. Such dockets have the code `MC-51-CR-0000001-2019`. More serious criminal cases are adjudicated in the Common Pleas Courts ("CP") and will have the code `CP-51-CR-0000001-2019`. Such cases will have both a MC and a CP docket.





### API Considerations

The API, which returns JSON for a given docket or court summary you indicate, is useful.

However, one problem is identifying what parameters to put in your request (which docket numbers exist).  Other issues relate to throttling limits of the API and the need to combine JSON data in a useful schema for analysis.  

An ACLU staffer did work to download and schematize data related specifically to Philadelphia County dockets a few years ago.  This is the data we had for the JAT/RLadies hackathon. I put it up in BigQuery and made a deidentified version of the data available in .csvs for data/hackathon participants.

This system of ETL from the API, however, is **not currently working** (it was a well-done, multi-system kludge by a non-developer who has moved on to bigger and better things).  My fork of this system, with updated notes indicating how far I got into trying to troubleshoot it, can be found at [https://github.com/pm0kjp/padockets](https://github.com/pm0kjp/padockets).  This is a private repository, so request access of Joy Payton and I'll be happy to add you.  

One worthy endeavor could be to fix / modernize / redesign a system that would:

* Identify which dockets exist
* Grab those dockets from the UJS API
* Transform the JSON into a more easily interrogable format (e.g. SQL database in the cloud)
* Automate periodic updating of the data on an ongoing basis.

### Data Considerations

Organizations (and maybe citizens?) can also request a custom data pull from the Commonwealth, at a cost of $80 per worker hour.  I have a well-organized dataset that was obtained this way, consisting of a huge statewide set of pipe delimited text files for the date range 1/1/2016 through 2/6/2023.  

Here are the data files, which are related to Common Pleas Criminal Case Management System (CPCMS) and Magisterial District Judge System (MDJS).

* CPCMS_AliasData.txt
* CPCMS_AttorneyData.txt
* CPCMS_BailActionData.txt
* CPCMS_BailPostData.txt
* CPCMS_CalendarEventData.txt
* CPCMS_CaseData.txt
* CPCMS_DiversionaryData.txt
* CPCMS_DocketEntryData.txt
* CPCMS_FinancialData.txt
* CPCMS_OffenseData.txt
* CPCMS_ParticipantConfinementData.txt
* CPCMS_PaymentPlanData.txt
* CPCMS_RelatedCaseData.txt
* CPCMS_SentenceData.txt
* CPCMS_SentenceLinkData.txt
* MDJS_AliasData.txt
* MDJS_AttorneyData.txt
* MDJS_BailActionData.txt
* MDJS_BailPostData.txt
* MDJS_CalendarEventData.txt
* MDJS_CaseConfinementData.txt
* MDJS_CaseData.txt
* MDJS_DocketEntryData.txt
* MDJS_FinancialData.txt
* MDJS_OffenseData.txt
* MDJS_PaymentPlanData.txt
* MDJS_SentenceData.txt

And here's what some of these pipe-delimited files have as columns:

* `CPCMS_AttorneyData.txt`: DocketNumber|OTN|AttorneyName|SupremeCourtNumber|RepresentationType|AttorneyStatus|RepresentationDate|AttorneyStatusDate|Address|City|State|ZipCode
* `CPCMS_SentenceData.txt`: DocketNumber|OTN|OriginatingOffenseSequenceNumber|OffenseSequenceNumber|SentenceType|SentenceDate|SentencePeriod|ProgramType|EffectiveSentenceDate|MinYears|MinMonths|MinDays|MinHours|MaxYears|MaxMonths|MaxDays|MaxHours|SentencingJudge|SentencingLocation|SentencingEventType|SentenceConditions|CreditForTimeServed|CaseDisposition|OffenseDisposition|DisposingJudge
* `CPCMS_OffenseData.txt`: DocketNumber|OTN|OffenseSequenceNumber|Title|Section|SubSection|Description|OffenseDate|OffenseDisposition|OffenseDispositionDate|LeadOffenseIndicator|OffenseGrade

This could be a great basis for a more data-analysis focused hackathon for people who are more interested in data science than software development.

Ideally, however, results from data analysis could be displayed in a website and made user-friendly with developer help!

## What Do I, Joy, Offer?

* I'm not a lawyer
* I'm not "JAT" and I don't represent any organization
* I can't make (the entire) hackathon (going to see the eclipse on April 8)

BUT

I am passionate about:

* Criminal legal reform
* Voter education
* Data science education
 
I can also explain (as can others) the work and outcomes in the RLadies/JAT hackathon.

I am willing to offer:

* Regular (but not 100%) attendance at planning meetings
* Appearance (if not 100% participation) in the actual hackathon
* Education in how to use BigQuery (I teach this for O'Reilly), SQL, R, Python (I teach these skills at CHOP).  For example I can make data education modules similar to [the ones I and my team produce](https://arcus.github.io/education_modules/list_of_modules) for our research into metascience and data science education for biomedical researchers.