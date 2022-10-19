
# 1.1 - Compare and contrast governance, risk, and compliance concepts.

## Permission to attack:

* Essentially a 'Get-out-of-jail-free' card. You have permission to attack a system/company.
* This get-out-of-jail-free card has [company contacts] names and phone numbers listed with their signatures. If a pentester get caught, they can ultimately show this card to get out of any real trouble.

## Regulatory compliance considerations:
*  **_Regulation_** -- this is what you MUST do (or how you should do it).
*  **_Compliance_** -- verifies you follow regulation (“Did you do the thing(s) you were supposed to do?”).
	* **_Compliance-based assessment_** -- governed by clearly-defined objectives & regulations.
	* Data Isolation, limited access/limited storage → usually required by a compliance assessment.
* **_PCI DSS_**  -- (Payment Card Industry Data Security Standard)
	* Governance & regulations surrounding the processing of credit card payments, which should reduce credit card fraud. PCI-DSS also requires regular vulnerability scans to be conducted. 	

	|Merchant Level|# of transactions (annually)  | External auditor | Quarterly Scans (by ASV) | Report on Compliance |		
	|--|--|--|--|--|
	| 1 | 6M > | | X | X (by QSA) |
	| 2 | 1M - 6M | | X | X |
	| 3 | 20,000 - 1M | X| X | |
	| 4 | <20,000 | X| | |

* ***GDPR*** -- (General Data Protection Regulation)
	* European Union (EU) regulation that protects data and privacy. Data can’t be collected w/out valid purpose. Right to be forgotten.

## Location Restrictions:
*  **_Tool restrictions_** -- What’s the use case? Could be regulatory or compliance driven? Or by the client's risk appetite? Could be out of the scope of the planned pentest documentation/SLA.
* ***Country limitations*** -- Pentesters need to be aware of the export restrictions of their country (and abide by them). National export restrictions would mean that the given data, services, or technology shouldn't leave the country.
* ***Local laws*** -- Who do I need to be compliant with? Local or State regulations? Be aware so you know how to conduct yourself. 
	* Certain U.S. states have specific hacking laws (ex. the New York State Cybersecurity Regulation specifically define cybersecurity requirements when performing pentests).
* Local government requirements --
	* Privacy requirements -- 
		* EU example → GDPR (privacy regarding EU).
		* US example → California Privacy Rights Act of 2020 (CRPA). It’s basically GDPR, but at a state level. 
## Legal Concepts:
* **_Statement of Work (SoW)_** -- 
	* Formal doc that details the deliverables to be performed during an engagement.
	* Contains → Scope; Responsibilities of pentester AND client; Schedule; Payment timelines; Final report.
	* What to do if → Accidental downtime due to scans/activity.
	* Update scope if needed (if a stakeholder is requesting an update to the scope, a renegotiation is most-likely necessary). 
	* All parties must sign off on the SOW.
* ***Master Service Agreement (MSA)*** --
	* Specialized type of contract. Used to govern future transactions and agreements. Recurring in nature (ex. Quarterly assessments).
	* Specific duration, timelines, permission → negotiated in the SOW.
	* Overarching “this is what we’re supposed to do” document. 
* ***Service-Level Agreement (SLA)*** -- 
	* Commitment between a pentester/service-provider AND a client (commonly used for SECaaS or Pentests).
		* Ex. “Remediate category 1 vulnerabilities within 3 days”. 
	* Defines expectations. Specific services, as well as measurable expectations, will be defined (ex. “I met the expectation of 24hr service”).
	* Both service provider AND customer → will have responsibilities defined.
	* Sanctions and reparations will be set. (for if/when violations occur).
* ***Non-Disclosure Agreement (NDA)*** -- 
	* Aka ***Confidentiality*** agreement. 
	* NDAs are usually blanket statements → “DO NOT talk/disclose X, Y, Z…”
	* Both sides should fill out NDAs (NDA legally binds BOTH parties from disclosing or disseminating).
		* Pentesters → should be conscious to not expose certain client information.
		* Clients → must be conscious to not expose Pentest details (i.e. access to pentester's information, proprietary, process, tools, etc.).
