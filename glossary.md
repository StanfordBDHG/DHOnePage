# Digital Health Glossary

*Biodesign for Digital Health*

The acronyms and terms you'll keep running into across the regulatory, technical, and payment sides of the course, grouped by where you're most likely to hit them rather than alphabetically. A few terms that aren't acronyms are mixed in where leaving them out would be odd; those have a dash in the second column.

---

## 1. Regulatory and policy

### Federal agencies and offices

| Acronym | Spelled out | Definition |
|---|---|---|
| HHS | US Department of Health and Human Services | The cabinet-level department that houses nearly every federal health agency on this list (CMS, FDA, CDC, NIH, OCR, ONC, SAMHSA), so most federal health policy is ultimately HHS policy. |
| CMS | Centers for Medicare & Medicaid Services | The agency that runs Medicare, Medicaid, CHIP, and the ACA marketplaces; it's the largest payer in the country, and commercial insurers tend to copy its coverage and payment decisions. |
| CMMI | Center for Medicare and Medicaid Innovation (the "Innovation Center") | The arm of CMS created by the ACA to test new payment and delivery models (ACOs, InCK, ACCESS, ASPIRE) before they're expanded or shut down. |
| CCIIO | Center for Consumer Information and Insurance Oversight | The CMS office that oversees the ACA marketplaces and the private insurance rules the ACA created. |
| FDA | Food and Drug Administration | The agency that regulates drugs, devices, and the software that counts as a device, and decides whether a product can be sold at all; CDRH (the Center for Devices and Radiological Health) is the part that handles devices and digital health. |
| CDC | Centers for Disease Control and Prevention | The federal public health agency, which touches digital health mostly through surveillance, immunization registries, and public health reporting standards. |
| NIH | National Institutes of Health | The federal biomedical research funder, and the sponsor of large data programs like the All of Us precision medicine cohort. |
| OCR | Office for Civil Rights | The HHS office that enforces HIPAA (it investigates breaches and levies the fines) as well as the ACA's nondiscrimination rules, including how they apply to clinical algorithms. |
| ONC (now ASTP/ONC) | Office of the National Coordinator for Health Information Technology, reorganized in 2024 under the Assistant Secretary for Technology Policy | The federal agency that maintains rules and regulations behind interoperability in the US, certifies EHRs, and runs TEFCA; most people still just say ONC. |
| SAMHSA | Substance Abuse and Mental Health Services Administration | The HHS agency for mental health and substance use, which also owns the 42 CFR Part 2 confidentiality rules for substance use treatment records. |
| HRSA | Health Resources and Services Administration | The HHS agency that funds the safety net: FQHCs, rural health programs, and the 340B drug discount program. |
| OIG | Office of Inspector General | HHS's internal watchdog, which audits federal health programs, investigates fraud, waste, and abuse, and can exclude providers from Medicare and Medicaid. |
| FTC | Federal Trade Commission | The consumer protection and competition agency that goes after deceptive marketing claims and unfair data practices, which makes it the de facto privacy regulator for all the health apps HIPAA doesn't cover. |
| FCC | Federal Communications Commission | The agency that regulates broadband and wireless spectrum, which matters for telehealth access and connected devices. |
| DEA | Drug Enforcement Administration | The Justice Department agency that controls prescribing of controlled substances, including the still-temporary rules that let clinicians prescribe them over telehealth without an in-person visit. |
| AG | Attorney General (state) | Each state's top lawyer, who can investigate and sue companies under state consumer protection, privacy, and AI laws, and who lately has been more aggressive on health tech than the federal agencies. |

### Laws, rules, and policy vocabulary

| Acronym | Spelled out | Definition |
|---|---|---|
| HIPAA | Health Insurance Portability and Accountability Act (1996) | The federal law that sets the baseline privacy and security rules for health data held by providers, health plans, clearinghouses, and their vendors; people are often surprised to learn it doesn't cover most consumer apps. |
| HITECH | Health Information Technology for Economic and Clinical Health Act (2009) | The landmark federal legislation that enabled much of the digital health industry, providing over $30B in incentives for health systems to adopt electronic health records (it also added breach notification and much bigger HIPAA penalties). |
| ACA | Affordable Care Act (2010) | The health reform law that expanded Medicaid, created the insurance marketplaces, and set up CMMI, ACOs, and much of the value-based payment machinery we talk about in this course. |
| Cures Act | 21st Century Cures Act (2016) | The law that banned information blocking, required EHRs to expose standardized APIs, and carved certain clinical decision support software out of FDA's definition of a device. |
| Information blocking | — | The Cures Act rule that providers, EHR vendors, and HIEs can't unreasonably interfere with access to or exchange of electronic health information, which is why patients now see notes and results the moment they're final. |
| MACRA | Medicare Access and CHIP Reauthorization Act (2015) | The law that replaced the old Medicare physician payment formula with the Quality Payment Program, which pays clinicians partly on quality and cost performance. |
| TEFCA | Trusted Exchange Framework and Common Agreement | The ONC-led framework for nationwide exchange, where a small number of designated networks (QHINs) agree to one set of rules so data can move anywhere in the country instead of through a patchwork of regional HIEs. |
| HTI-1 | Health Data, Technology, and Interoperability rule | ONC's 2023 rule that updated EHR certification and added the first federal transparency requirements for AI and predictive tools built into certified EHRs. |
| Section 1557 | Section 1557 of the ACA | The ACA's nondiscrimination provision, which OCR has applied to clinical algorithms and decision support tools, so a provider can be on the hook for using a tool that discriminates by race, sex, age, or disability. |
| 42 CFR Part 2 | Title 42, Code of Federal Regulations, Part 2 | The federal rule that gives substance use disorder treatment records more protection than HIPAA does, generally requiring patient consent before they can be shared (recently brought a bit closer to HIPAA). |
| CFR | Code of Federal Regulations | Where federal regulations live once they're final; 45 CFR is HIPAA, 21 CFR is FDA, 42 CFR is CMS and public health. |
| NPRM | Notice of Proposed Rulemaking | A draft regulation published in the Federal Register for public comment, the stage where industry and advocates try to shape a rule before it's final (an RFI, Request for Information, is the even earlier "we're thinking about this" step). |
| AKS | Anti-Kickback Statute | The criminal law against paying or receiving anything of value for referrals of federally funded healthcare business, which is why "free" software or devices for providers have to fit a safe harbor; its civil cousin, the Stark Law, bars physicians from referring to entities they have a financial stake in. |
| FCA | False Claims Act | The law that makes billing Medicare or Medicaid for things you didn't do (or shouldn't have billed) a federal offense, with whistleblower provisions that make it the government's main fraud enforcement tool. |
| CPOM | Corporate Practice of Medicine (doctrine) | The state-law rule, strongest in California, New York, and Texas, that only licensed physicians can own medical practices or employ physicians, which is why telehealth companies are structured as an MSO contracting with a physician-owned professional corporation. |
| MSO | Management Services Organization | The company that supplies the non-clinical side of a practice (technology, staff, billing, marketing) under a management agreement, the standard way to build a venture-backed clinical business under CPOM. |
| IMLC | Interstate Medical Licensure Compact | The agreement among most states that speeds up getting licensed in several of them, which matters because a telehealth clinician has to be licensed where the patient is, not where the clinician sits (PSYPACT is the equivalent for psychologists). |
| Scope of practice | — | State rules on what each type of licensed professional is allowed to do, and the reason only a human can be licensed to provide healthcare services today; an AI can't hold a license, so someone licensed has to be accountable for the care. |
| Regulatory sandbox | — | A state program that lets a company test a product under relaxed rules with regulator oversight for a limited time; Utah's AI Office is the current example, with supervised experiments in AI-assisted prescription renewals. |
| State AI laws | — | The growing set of state laws aimed at AI specifically (California, Colorado, Illinois, and New York among the first), covering things like disclosure when AI drafts patient communications, limits on AI-only therapy, and bias requirements for consequential decisions; these are moving far faster than anything federal. |
| GDPR | General Data Protection Regulation | The EU's privacy law, which treats health data as a special category and gives individuals rights (access, erasure, portability) that go well beyond HIPAA; it applies the moment you have a European user. |

### FDA and device regulation

| Acronym | Spelled out | Definition |
|---|---|---|
| FD&C Act | Federal Food, Drug, and Cosmetic Act (1938) | The law that gives FDA its authority, and whose definition of a "device" (as amended by the Cures Act) decides whether your software is regulated at all. |
| SaMD | Software as a Medical Device | Software that is itself the medical device (an app that diagnoses or guides treatment) rather than software embedded in a hardware device, which is SiMD, software in a medical device. |
| Intended use | — | The purpose a product is marketed for, which is what FDA actually regulates; the same sensor can be an unregulated wellness product or a Class II device depending on what you claim it does. |
| General wellness | — | FDA's policy of not regulating low-risk products meant only for general wellness (fitness, sleep, stress), which is where most consumer wearables sit; the line is drawn by your claims, not your hardware, and the January 6, 2026 update let non-invasive wearables estimate blood pressure, glucose, SpO2 and HRV under it as long as the claims stay wellness-only. |
| CDS | Clinical Decision Support | Software that gives clinicians information or recommendations to support a decision; the Cures Act exempts it from FDA oversight only if, among other criteria, the clinician can independently review the basis for the recommendation rather than just trust the output (and since FDA's January 2026 guidance it may propose a single treatment plan, not just a list of options, as long as the clinician reviews and finalizes it). |
| Class I / II / III | Device risk classes | FDA's three risk tiers: Class I is low risk and mostly exempt from review, Class II is moderate risk and where most SaMD lands, and Class III is high risk and needs full premarket approval. |
| 510(k) | Premarket Notification (named for section 510(k) of the FD&C Act) | The most common FDA pathway, where you show your device is "substantially equivalent" to one already on the market; most AI-enabled devices have gone this route. |
| De Novo | De Novo classification request | The pathway for novel low- to moderate-risk devices with no predicate to compare against, which creates a new device type that later products can file 510(k)s against. |
| PMA | Premarket Approval | The most rigorous FDA pathway, reserved for Class III devices and usually requiring clinical trials. |
| Breakthrough Devices | Breakthrough Devices Program | FDA's program that gives faster review and more interaction to devices that could meaningfully improve diagnosis or treatment of serious conditions. |
| IRB | Institutional Review Board | The committee that reviews and approves research on human subjects, which you'll deal with for any study, pilot, or dataset involving real patients. |
| GMLP | Good Machine Learning Practice | The ten principles FDA (with Health Canada and the UK's MHRA) published for developing AI and machine learning devices responsibly. |
| PCCP | Predetermined Change Control Plan | A plan submitted with an AI-enabled device describing how the model will be updated or retrained over time, so the manufacturer doesn't have to go back to FDA for every change. |
| QMSR | Quality Management System Regulation | FDA's updated quality system rules for device manufacturers, aligned with the international ISO 13485 standard and in effect since February 2026. |
| RWD / RWE | Real-World Data / Real-World Evidence | Data collected outside traditional trials (EHRs, claims, wearables, registries) and the evidence built from it, which FDA increasingly accepts in regulatory decisions. |
| TEMPO | Technology-Enabled Meaningful Patient Outcomes pilot | FDA's pilot, paired with CMS's ACCESS Model, that lets manufacturers use digital health devices with ACCESS patients before they have marketing authorization, in exchange for sharing real-world data with FDA. |

### Privacy law and HIPAA mechanics

| Acronym | Spelled out | Definition |
|---|---|---|
| PHI | Protected Health Information | Any individually identifiable health information held by a HIPAA covered entity or its business associates; the same data in a consumer app with no covered entity behind it isn't PHI (ePHI is just the electronic version, and PII is the broader non-HIPAA term for anything that identifies a person). |
| CE | Covered Entity | The three kinds of organizations HIPAA directly regulates: providers that bill electronically, health plans, and clearinghouses. |
| BA / BAA | Business Associate / Business Associate Agreement | A vendor that handles PHI on behalf of a covered entity, and the contract that makes it legally responsible for protecting that data; if you sell to health systems you'll sign a lot of these. |
| Privacy Rule, Security Rule, Breach Notification Rule | — | HIPAA's three main regulations: who can use and share PHI and for what, the administrative, physical, and technical safeguards required to protect ePHI, and what you have to do (and whom you have to tell) when it's exposed. |
| TPO | Treatment, Payment, and Operations | The three purposes for which HIPAA lets covered entities use and share PHI without asking the patient's permission. |
| De-identification | — | Stripping data so it's no longer PHI, by either HIPAA's Safe Harbor method (remove 18 specific identifiers) or Expert Determination (a statistician certifies that re-identification risk is very small); a Limited Data Set keeps dates and geography and can be shared for research under a Data Use Agreement. |
| COPPA | Children's Online Privacy Protection Act | The FTC-enforced law that restricts collecting personal data online from children under 13 without verifiable parental consent, which every pediatric app has to design around. |
| FERPA | Family Educational Rights and Privacy Act | The federal law protecting student education records, which governs (instead of HIPAA) most health information held by schools and school-based programs. |
| HBNR | Health Breach Notification Rule | The FTC rule requiring health apps and other companies outside HIPAA to notify users and the FTC when health data is breached or shared without permission. |
| CCPA / CPRA | California Consumer Privacy Act / California Privacy Rights Act | California's general consumer privacy law, which covers the health data that falls outside HIPAA and has been the template for most other state privacy laws (Washington's My Health My Data Act is the first one aimed squarely at consumer health data). |
| CMIA | Confidentiality of Medical Information Act (California) | California's medical privacy law, which is stricter than HIPAA in places and explicitly reaches some apps and vendors HIPAA doesn't. |

---

## 2. Health data and technical terms

### Systems

| Acronym | Spelled out | Definition |
|---|---|---|
| EHR / EMR | Electronic Health Record / Electronic Medical Record | The system where clinical care is documented, ordered, and billed; technically an EMR is one practice's record and an EHR is the longitudinal, shareable version, but in practice people use the terms interchangeably. |
| PHR | Personal Health Record | A record the patient controls rather than the provider (Apple Health is the main modern example). |
| HIE | Health Information Exchange | A regional or statewide organization (or the activity itself) that moves patient records between unaffiliated providers. |
| CEHRT | Certified EHR Technology | An EHR that has passed ONC's certification program, which is the prerequisite for most federal quality and incentive programs and the lever ONC uses to push new standards into the market. |
| CDSS | Clinical Decision Support System | Software that delivers alerts, reminders, order sets, or recommendations at the point of care, usually firing inside order entry (CPOE) or documentation. |
| DSI | Decision Support Intervention | ONC's regulatory term (from HTI-1) for the predictive and evidence-based decision support tools inside certified EHRs, which now come with "source attribute" transparency requirements so users can see how a model was built and validated. |
| ADT | Admit, Discharge, Transfer (messages) | The HL7 messages announcing that a patient was admitted, discharged, or moved, which are the backbone of most real-time care coordination and the event notifications hospitals are now required to send. |
| MPI / EMPI | (Enterprise) Master Patient Index | The system that figures out which records across different systems belong to the same person, necessary because the US has no national patient identifier. |
| PDMP | Prescription Drug Monitoring Program | The state databases of controlled substance prescriptions that clinicians have to check before prescribing opioids and similar drugs. |
| eRx | Electronic prescribing | Sending prescriptions electronically from the EHR to the pharmacy, nearly all of it over the Surescripts network using the NCPDP SCRIPT standard. |
| IIS | Immunization Information System | The state and local immunization registries that EHRs report vaccines to, which in pediatrics are often the most complete record a child has. |

### Standards and exchange

| Acronym | Spelled out | Definition |
|---|---|---|
| HL7 | Health Level Seven International | The standards organization behind most of the health data standards on this list (v2, CDA, FHIR); "level seven" refers to the application layer of the network model. |
| HL7 v2 | Health Level Seven version 2 | The decades-old pipe-delimited messaging standard that still carries most hospital data traffic (lab results, ADT feeds, orders); ugly, but everywhere. |
| C-CDA | Consolidated Clinical Document Architecture | HL7's XML document standard for packaging a clinical summary to send between systems; the Continuity of Care Document (CCD) is the most common type and what gets exchanged in most transitions of care. |
| FHIR | Fast Healthcare Interoperability Resources | The data standard that is used to transfer health data between applications and EHRs, built on ordinary web technology (REST APIs and JSON) rather than older messaging formats. |
| API | Application Programming Interface | The defined way one piece of software talks to another; in health IT "the API" almost always means a FHIR endpoint. |
| SMART on FHIR | Substitutable Medical Applications, Reusable Technologies | The open standard for launching a third-party app inside an EHR and letting it read FHIR data with the user's permission, which is how most EHR-integrated apps are built. |
| OAuth 2.0 / OpenID Connect | — | The web standards for authorization and identity that SMART on FHIR uses, so a patient or clinician can grant an app access without handing over a password. |
| Bulk FHIR | FHIR Bulk Data Access ("Flat FHIR") | The FHIR specification for pulling data on a whole population at once instead of one patient at a time, which is what makes FHIR usable for analytics and payer exchange. |
| USCDI | United States Core Data for Interoperability | The federally defined minimum set of data elements (problems, meds, labs, notes, and so on) that certified EHRs must be able to exchange, updated roughly annually; the US Core FHIR profiles spell out exactly how each element is represented. |
| QHIN | Qualified Health Information Network | A network approved to participate in TEFCA and exchange with every other QHIN (Epic, eHealth Exchange, Health Gorilla, and CommonWell are examples). |
| Patient Access API | — | The FHIR API that CMS requires Medicare Advantage, Medicaid, and marketplace plans to offer so members can pull their claims and clinical data into apps of their choice; the same rules require prior authorization APIs by 2027. |
| CDS Hooks | — | The HL7 standard that lets an outside service push decision support "cards" into the EHR workflow at defined trigger points, like when an order is signed. |
| X12 / EDI | ASC X12 / Electronic Data Interchange | The transaction standards HIPAA requires for claims, eligibility checks, and payments (the 837 claim and the 835 remittance are the ones you'll hear about). |
| DICOM | Digital Imaging and Communications in Medicine | The standard format and protocol for medical images. |
| OMOP | Observational Medical Outcomes Partnership (common data model) | The research data model, maintained by the OHDSI community, that maps data from different EHRs into one standard schema so the same analysis can run across institutions. |

### Clinical terminologies and code sets

| Acronym | Spelled out | Definition |
|---|---|---|
| LOINC | Logical Observation Identifiers Names and Codes | The standardized terminology that's used to describe observations like lab tests and vitals. |
| SNOMED CT | Systematized Nomenclature of Medicine, Clinical Terms | The comprehensive clinical terminology for problems, findings, and procedures the way clinicians document them (as opposed to ICD, which is organized for billing). |
| RxNorm | — | The National Library of Medicine's standardized names and codes for clinical drugs, which is what lets a system recognize that two differently branded products are the same medication. |
| NDC | National Drug Code | FDA's product- and package-level identifier for each drug, used in pharmacy and claims. |
| CVX | Vaccine Administered codes | The CDC code set for vaccines, used by EHRs and immunization registries. |

### AI and security

| Acronym | Spelled out | Definition |
|---|---|---|
| NLP | Natural Language Processing | The branch of AI that reads and structures free text, which in healthcare means pulling meaning out of clinical notes. |
| LLM | Large Language Model | The class of AI models (GPT, Claude, Gemini) trained on enormous amounts of text that now sits behind ambient documentation, patient message drafting, and most of the "AI in healthcare" conversation; note that most FDA-cleared AI devices are older-style machine learning models for imaging and signals, not LLMs. |
| SOC 2 | System and Organization Controls 2 | The third-party audit report (from the AICPA) that health systems and payers almost always ask vendors for as proof that security controls actually work as described. |
| HITRUST | Health Information Trust Alliance (CSF certification) | A healthcare-specific security certification that bundles HIPAA, NIST, ISO, and other requirements into one assessment; expensive to get, but it opens enterprise doors. |
| MFA / SSO | Multi-Factor Authentication / Single Sign-On | Requiring a second factor beyond a password, and letting users log into many systems with one identity; both are baseline expectations for anything touching PHI. |

---

## 3. Health finance and payment

### Payers and programs

| Acronym | Spelled out | Definition |
|---|---|---|
| Medicare | — | The federal program for people 65 and over and some with disabilities, split into Part A (hospital), Part B (outpatient and physician), Part C (Medicare Advantage), and Part D (drugs); because CMS sets its rules nationally, Medicare is where most new payment ideas, including the digital health codes, show up first. |
| MA | Medicare Advantage (Medicare Part C) | Private plans paid a risk-adjusted capitated rate by CMS to cover Medicare beneficiaries, now more than half of them, which makes MA plans a major buyer of anything that improves Star ratings or lowers cost. |
| Medicaid | — | The joint federal-state program for low-income people that covers nearly half of US children and is administered differently in every state, which is why a "Medicaid strategy" is really 50 separate strategies. |
| CHIP | Children's Health Insurance Program | The federal-state program for kids whose families earn too much for Medicaid but can't afford private coverage, usually run alongside Medicaid. |
| MCO | Managed Care Organization | An arrangement where an insurance company gets paid on a per-capita basis to take care of a subgroup of the population; most Medicaid enrollees are now in MCOs rather than state-run fee-for-service Medicaid. |
| EPSDT | Early and Periodic Screening, Diagnostic, and Treatment | Medicaid's benefit guarantee for anyone under 21, which entitles kids to all medically necessary care, including screening and developmental services adult Medicaid doesn't have to cover; it's the legal hook for a lot of pediatric services. |
| ESI | Employer-Sponsored Insurance | Coverage through an employer, which is how most working-age adults are insured and why employer benefits are such a common sales channel for adult-focused digital health. |
| Self-insured | — | An employer that pays its employees' claims itself and hires an insurer or a third-party administrator (TPA) only to process them, which gives it the freedom to buy digital health benefits directly; most large employers are self-insured. |
| PBM | Pharmacy Benefit Manager | The middleman that manages drug benefits for plans and employers, negotiating rebates and deciding which drugs are covered. |
| FQHC | Federally Qualified Health Center | Community health centers that get federal grants and enhanced Medicaid payment to serve underserved areas, paid a per-visit rate rather than fee-for-service, which changes what a digital tool has to prove to be worth it to them. |
| SBHC | School-Based Health Center | A clinic located in a school, often run by an FQHC or hospital, that bills Medicaid and is one of the few places where the health and education sectors actually share patients and money. |

### How money moves

| Acronym | Spelled out | Definition |
|---|---|---|
| FFS | Fee-for-Service | The traditional model where every visit, test, and procedure is billed separately, which rewards volume over outcomes and is what value-based care is trying to move away from. |
| Capitation | — | A fixed payment per person per period to cover whatever care that person needs, which shifts financial risk from the payer to whoever accepts it. |
| PMPM | Per Member Per Month | The standard unit of capitated payment and of digital health pricing to plans and health systems (a $2 PMPM contract for 100,000 members is $2.4M a year); PEPM, per employee per month, is the same idea when selling to employers. |
| VBC | Value-Based Care | The umbrella term for payment arrangements that tie what a provider earns to quality and cost outcomes rather than volume. |
| APM | Alternative Payment Model | CMS's term for any payment model that isn't pure fee-for-service (bundles, ACOs, capitation); "Advanced APMs" carry downside risk and earn bonuses under MACRA. |
| ACO | Accountable Care Organization | A group of providers that agrees to be accountable for the total cost and quality of care for a defined population and keeps a share of any savings (the Medicare Shared Savings Program, MSSP, is the permanent and largest version). |
| Shared savings | — | The mechanism where a provider gets a portion of the money saved against a spending benchmark; "two-sided" or "downside" risk means they also owe money if spending comes in over. |
| DRG | Diagnosis-Related Group | The inpatient payment unit where Medicare pays a hospital a fixed amount per admission based on the diagnosis, regardless of what the stay actually cost. |
| RVU | Relative Value Unit | The measure of the work, practice expense, and malpractice cost of each service, which (times a dollar "conversion factor") sets what Medicare pays for a CPT code; also how a lot of physicians' productivity and pay get measured. |
| PFS | Physician Fee Schedule | CMS's annual rule setting Medicare payment for each code, which is also where new digital health codes (RPM, RTM, digital mental health treatment) get created each year. |
| HCC | Hierarchical Condition Category | The risk adjustment coding system CMS uses to pay more for sicker populations, which is why documenting diagnoses completely is worth real money in Medicare Advantage and ACOs (and why there's so much fraud enforcement around it). |
| MLR | Medical Loss Ratio | The share of premiums an insurer spends on medical care, which the ACA requires to be at least 80 to 85 percent, limiting what plans can spend on administration and profit (and shaping how they classify what they buy from vendors). |
| PA | Prior Authorization | The insurer's requirement that certain services be approved before they're delivered, a major administrative burden and now the target of CMS rules requiring payers to automate it through APIs. |
| NCD / LCD | National / Local Coverage Determination | Medicare's formal decisions on whether a service is covered nationwide (an NCD) or only in a region (an LCD, issued by the regional Medicare Administrative Contractor, or MAC, that processes claims there). |
| RCM | Revenue Cycle Management | The whole back-office process from registration through coding, claims, denials, and collections; also a very large software category and where a lot of healthcare AI is actually making money today. |

### Codes and billing

| Acronym | Spelled out | Definition |
|---|---|---|
| CPT | Current Procedural Terminology | The AMA-owned code set for procedures and services that drives most outpatient billing, including the telehealth, RPM, and care management codes; Category III codes are temporary ones for new technologies that get tracked but usually not paid, the first step toward reimbursement for a new device or procedure. |
| HCPCS | Healthcare Common Procedure Coding System | CMS's code set that includes CPT (Level I) plus Level II codes for supplies, drugs, equipment, and services CPT doesn't cover, including many of the newer Medicare care management codes (the ones starting with G). |
| ICD-10-CM | International Classification of Diseases, 10th Revision, Clinical Modification | The diagnosis code set on every US claim, which is what justifies that a service was medically necessary; ICD-11 exists, but the US hasn't moved yet. |
| E/M | Evaluation and Management (codes) | The CPT codes for office and hospital visits, the bread and butter of physician billing, now leveled by time or by the complexity of medical decision-making. |
| NPI | National Provider Identifier | The 10-digit number every clinician and organization needs in order to bill, and the key you'll use to join provider data across datasets. |
| RPM | Remote Patient (or Physiologic) Monitoring | The CPT codes that pay for supplying a patient a connected device and reviewing the data it sends, which is the main reimbursement pathway for device-based digital health. |
| RTM | Remote Therapeutic Monitoring | The parallel codes for monitoring non-physiologic data like medication adherence, pain, or therapy exercises, which opened reimbursement to app-based products and to physical therapists and others who can't bill RPM. |
| CCM / PCM | Chronic Care Management / Principal Care Management | Codes that pay a monthly fee for non-face-to-face care coordination of patients with chronic conditions, which is what many "care management" startups are actually billing. |
| BHI / CoCM | Behavioral Health Integration / Collaborative Care Model | Codes that pay primary care practices for behavioral health delivered with a care manager and a consulting psychiatrist, the evidence-based model a lot of pediatric and adult mental health programs are built on. |
| APCM | Advanced Primary Care Management | The Medicare codes introduced in 2025 that bundle care management into a monthly per-patient payment without time tracking, a step toward capitated primary care. |
| DMHT | Digital Mental Health Treatment (codes) | The Medicare codes, also new in 2025, that pay for FDA-cleared digital mental health treatment devices prescribed by a clinician, the first real Medicare pathway for prescription digital therapeutics. |
| Telehealth flexibilities | — | The pandemic-era Medicare waivers (home as an allowed site of care, no rural restriction, audio-only in some cases) that Congress has mostly extended in short increments rather than making permanent, which puts the telehealth industry back on a cliff every few months. |

### Quality, value, and population health

| Acronym | Spelled out | Definition |
|---|---|---|
| HEDIS | Healthcare Effectiveness Data and Information Set | NCQA's standardized set of quality measures that health plans report (immunization rates, well-child visits, A1c control), which is what plans are graded on and therefore what they'll pay vendors to move. |
| NCQA | National Committee for Quality Assurance | The nonprofit that accredits health plans and maintains HEDIS and the Patient-Centered Medical Home (PCMH) recognition program. |
| Star Ratings | — | CMS's one-to-five star quality score for Medicare Advantage and Part D plans, which directly determines bonus payments and is why MA plans care so much about HEDIS and CAHPS. |
| CAHPS | Consumer Assessment of Healthcare Providers and Systems | The AHRQ-developed patient experience surveys that feed into Star Ratings and hospital quality scores. |
| Core Sets | Child and Adult Core Sets | The CMS-defined quality measure sets for Medicaid and CHIP; states have had to report the Child Core Set since 2024, and it's the closest thing pediatrics has to the HEDIS-driven incentives that adult care runs on. |
| QPP / MIPS | Quality Payment Program / Merit-based Incentive Payment System | The MACRA program that adjusts Medicare physician payment up or down based on quality, cost, improvement activities, and interoperability performance. |
| PI | Promoting Interoperability | The successor to Meaningful Use (the HITECH-era program that paid providers to adopt certified EHRs and use them in specific ways), now the part of MIPS and the hospital program that scores how providers actually use their EHRs. |
| SDOH / HRSN | Social Determinants of Health / Health-Related Social Needs | The non-medical factors (housing, food, transportation, income) that shape health, and the individual-level version of them (this patient is food insecure), which Medicaid programs are increasingly screening for and paying to address. |
| 1115 waiver | Section 1115 demonstration waiver | The mechanism that lets a state run its Medicaid program differently from federal rules to test something new, which is how states fund things like housing supports, community health workers, and pediatric pilots. |
| ILOS | In Lieu of Services | The Medicaid managed care option to pay for a substitute service (medically tailored meals, a digital program) instead of a covered one when it's cost-effective, a relatively new way to get non-traditional services paid for. |
| ROI | Return on Investment | The number every payer and health system will ask you for, usually expected within a year, and the reason preventive and pediatric interventions, whose returns land years later and often in someone else's budget, have a harder time getting funded. |
| Wrong-pocket problem | — | When the organization that pays for an intervention isn't the one that captures the savings (a school pays and Medicaid saves, or the other way around), which is one of the central reasons pediatric prevention is underfunded. |

### Federal models worth knowing

| Acronym | Spelled out | Definition |
|---|---|---|
| InCK | Integrated Care for Kids | The CMMI model (2020 through 2026) that funded state and local partnerships to integrate physical, behavioral, and social services for Medicaid-covered children, with alternative payment models to support it. |
| ASPIRE | Accelerating State Pediatric Innovation Readiness and Effectiveness | The CMMI model announced in March 2026 as the successor to InCK: a 10-year, up-to-five-state, $125M program that pays Medicaid providers to take accountability for the quality and cost of care for kids under 21 with (or at risk of) complex medical and behavioral needs. |
| ACCESS | Advancing Chronic Care with Effective, Scalable Solutions | The CMMI model, with its first cohort starting in 2026, that pays organizations delivering technology-enabled care to Medicare patients with chronic conditions on outcomes rather than per service; it's the first Medicare payment model built around digital health companies, and the kind of thing pediatrics doesn't have yet. |

### Digital health business models (the taxonomy from our npj Digital Medicine paper)

| Acronym | Spelled out | Definition |
|---|---|---|
| D2C | Direct to Consumer | The company sells access to its product straight to the patient or caregiver, with no insurer, employer, or provider in between (an app subscription, for example). |
| B2B / B2B2C | Business to Business / Business to Business to Consumer | Selling to an organization (health system, plan, employer) rather than to individuals, and the variant where that organization then offers the product to its members or employees; most digital health revenue is one of these. |
| SaaS | Software as a Service | Subscription software hosted by the vendor, which is how most digital health is sold to providers and plans and structurally looks a lot like capitation (a recurring per-unit fee). |
| Billable to insurance | — | The company itself delivers a clinical service and bills a payer for it under a CPT code, which means it needs licensed clinicians, payer contracts, and a billing operation. |
| Capitated revenue | — | The company sells access to its product on a subscription (usually PMPM) basis to a provider, health system, health plan, employer, or Medicaid program, whether or not the underlying service is billable to insurance; this was the most common model among the pediatric companies we studied. |
| CBO | Community-Based (or Community Benefit) Organization | Nonprofits like food banks, family resource centers, and youth programs, which along with schools and government agencies are the "other" payers funding a lot of pediatric mental health and social-needs programs. |
| DTx / PDT | Digital Therapeutics / Prescription Digital Therapeutic | Software that delivers a clinical intervention on its own (CBT for insomnia, for example) with evidence behind it; "prescription" DTx are FDA-cleared and ordered by a clinician, and until the 2025 DMHT codes had almost no reimbursement pathway. |
