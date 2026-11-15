# TASK 5 – Research Report: Social Engineering Attacks

**Topic:** Phishing, Pretexting and Baiting  
**Subject:** Cybersecurity  
**Submission format:** Markdown  
**File name:** `social_engineering_report.md`

---

## 1. Introduction

Social engineering is the use of deception, manipulation and psychological influence to persuade people to reveal confidential information, perform an action, transfer money, or provide access to systems. Instead of depending only on technical weaknesses, an attacker targets the human decision-making process.

Social engineering is considered one of the most effective attack vectors because people naturally trust familiar names, authority figures and colleagues. Attackers exploit emotions such as urgency, fear, curiosity, greed, helpfulness and the desire to avoid trouble. A technically secure organisation can still be compromised if an employee is tricked into sharing a password, approving a login request or opening a malicious attachment.

### Why it is effective

- **Trust:** Attackers impersonate colleagues, banks, IT support teams, suppliers or government authorities.
- **Urgency:** Victims are told that an account will be blocked, a payment is overdue or immediate action is required.
- **Authority:** A request appears to come from a manager, executive or official.
- **Curiosity and reward:** Free gifts, attractive downloads or unknown devices encourage unsafe actions.
- **Low technical barrier:** An attacker may need only a convincing message or phone call to start an intrusion.

### Relevant statistics

The Verizon **2024 Data Breach Investigations Report (DBIR)** reported that 68% of breaches involved a non-malicious human element, such as a person making an error or falling for social engineering. In its analysis of social-engineering incidents, pretexting represented approximately 44% of action varieties and phishing approximately 31%. These figures show why organisations must treat human behaviour as an important part of cybersecurity. The percentages refer to Verizon's analysed datasets and should not be interpreted as a universal rate for every organisation.

The FBI Internet Crime Complaint Center (IC3) reported 21,489 Business Email Compromise (BEC) complaints and adjusted losses exceeding **US$2.9 billion** in 2023. BEC commonly involves impersonation and social engineering to induce unauthorised payments.

**Key point:** Social engineering is not simply a technology problem. It is a people, process and technology problem.

---

## 2. Phishing

### 2.1 Definition

Phishing is a social engineering attack in which an attacker sends a deceptive email, message, website link or other communication that appears to come from a trusted source. The purpose is to make the victim reveal credentials or financial information, approve an action, or download malware.

### 2.2 Common types of phishing

| Type | Explanation | Example |
|---|---|---|
| Spear phishing | A targeted phishing message created for a particular person or organisation using information about the target. | An employee receives an email referring to a real project and asking them to open an attached document. |
| Whaling | A targeted attack against senior executives or other high-value individuals. | A fake legal or financial request is sent to a CEO or CFO. |
| Vishing | Voice phishing conducted through telephone calls or voice-over-IP services. | A caller impersonates bank or IT support and asks the victim to disclose a one-time password. |
| Smishing | Phishing conducted through SMS or text messages. | A fake parcel-delivery or bank alert asks the recipient to visit a fraudulent website. |

### 2.3 How a phishing attack works

1. **Reconnaissance:** The attacker collects information about the target, such as their job role, organisation, colleagues or suppliers.
2. **Preparation:** The attacker creates a convincing email, text message, phone script or fake website.
3. **Delivery:** The message is sent to the victim, often with a link, attachment or urgent request.
4. **Manipulation:** The attacker uses urgency, fear, authority or curiosity to encourage the victim to act.
5. **Compromise:** The victim may disclose credentials, approve a fraudulent login, transfer money or execute malware.
6. **Abuse:** The attacker may use the stolen access to steal data, move through the network, commit fraud or launch further attacks.

### 2.4 Real-world case study: RSA SecurID breach (2011)

In March 2011, RSA disclosed that it had suffered a targeted cyberattack affecting information related to its SecurID authentication product. The initial intrusion involved spear-phishing emails sent to small groups of employees. The messages used the subject line **“2011 Recruitment Plan”** and included a malicious Excel attachment.

An employee opened the attachment, which exploited an Adobe Flash vulnerability and installed a remote-access tool. The attackers then used the initial foothold to move through the organisation, obtain additional credentials and access sensitive information related to SecurID.

**Impact and lessons:**

- A small, targeted email campaign was enough to create a serious organisational security incident.
- An employee who was not considered a high-profile target became the initial entry point.
- Email filtering alone was not sufficient to prevent the incident.
- Employee awareness, attachment controls, endpoint protection, least privilege and network monitoring are all important layers of defence.

**Sources:** Computer Weekly's reporting on RSA's disclosure and the Microsoft Security Chronicles retrospective are listed in the References section.

### 2.5 Prevention recommendations for phishing

1. **Verify the sender and destination:** Check the complete email address, domain name and URL before responding or signing in. Be alert to look-alike domains and unexpected changes in payment details.
2. **Avoid unexpected links and attachments:** Do not open unsolicited files or click suspicious links. Visit the organisation's official website by typing its address yourself.
3. **Use multi-factor authentication (MFA):** Enable MFA, preferably phishing-resistant methods such as FIDO2 security keys or passkeys. Never approve an unexpected authentication prompt or share an OTP.
4. **Report suspicious messages:** Use the organisation's approved phishing-reporting process. Security teams should investigate reported messages, block malicious domains and educate employees using realistic simulations.

---

## 3. Pretexting

### 3.1 Definition

Pretexting is a social engineering technique in which an attacker invents a believable story or false identity (a **pretext**) to gain a victim's trust and obtain information, money or access.

Unlike a basic phishing message, pretexting often involves a developed scenario and a conversation. The attacker may pretend to be an IT technician, bank employee, supplier, auditor, police officer, recruiter or senior manager.

### 3.2 How an attacker builds a false scenario

1. **Research:** The attacker studies the organisation, employee roles, reporting structure, vendors and publicly available information.
2. **Identity creation:** The attacker selects a role that the victim is likely to trust, such as IT helpdesk or a manager.
3. **Story development:** The attacker creates a believable reason for contacting the victim, such as a VPN problem, account verification or urgent invoice.
4. **Establishing trust:** The attacker uses familiar terminology, names, job titles or details about the organisation.
5. **Requesting an action:** The attacker asks for credentials, a password reset, confidential information, a payment or remote access.
6. **Exploitation:** The attacker uses the information or access obtained to commit fraud or compromise systems.

### 3.3 Real-world case study: Twitter/X employee social engineering incident (2020)

On 15 July 2020, attackers compromised Twitter's internal systems after targeting employees through phone-based social engineering. According to the New York State Department of Financial Services investigation, attackers called employees while pretending to be members of Twitter's IT helpdesk. They referred to VPN-related problems and used knowledge of the company's operations to make their story believable.

The attackers obtained employee credentials and used access to internal tools to take over high-profile accounts. The compromised accounts were used to publish cryptocurrency scam messages. The investigation reported that the attackers targeted 130 accounts, tweeted from 45 accounts, accessed direct messages from 36 accounts and downloaded data from 7 accounts.

**Impact and lessons:**

- Attackers can exploit trust in internal support teams.
- Remote-working procedures and helpdesk processes can become attractive targets.
- Employees should never disclose passwords or MFA codes to a caller claiming to be IT support.
- Sensitive helpdesk actions should require strong identity verification and approval controls.

**Sources:** New York State Department of Financial Services, *Twitter Investigation Report* (14 October 2020), and contemporaneous reporting by TechCrunch.

### 3.4 Prevention measures for pretexting

1. **Verify identity independently:** Call the person back using a known, official telephone number or contact them through an approved internal channel. Do not rely on contact details supplied by the requester.
2. **Follow approval procedures:** Require documented authorisation and a second-person check for password resets, access changes, sensitive data disclosure and financial transactions.
3. **Protect authentication information:** Never share passwords, OTPs, recovery codes or MFA approval requests. IT staff should use approved identity-verification processes and should never ask users to disclose their passwords.

---

## 4. Baiting

### 4.1 Definition

Baiting is a social engineering attack in which an attacker offers something attractive or interesting to encourage a victim to perform an unsafe action. The bait may be a physical object or a digital offer.

Baiting commonly exploits curiosity, greed, convenience or the expectation of receiving something for free.

### 4.2 Physical baiting

Physical baiting uses an object to tempt a person into compromising security.

**Examples:**

- An attacker leaves a USB drive labelled “Salary Details”, “Confidential” or “Employee List” in a public area.
- A person finds an unknown storage device in a car park and connects it to a work computer.
- An attacker leaves a device in a location where employees are likely to discover it.

The device may contain malicious files or may be configured to behave as a harmful peripheral. Connecting unknown devices to company equipment can expose systems and data.

### 4.3 Digital baiting

Digital baiting uses an online offer or download to persuade a victim to install or open unsafe content.

**Examples:**

- A fake website advertises free premium software or cracked applications.
- A fake game, movie or document download contains malware.
- A message offers a free gift, coupon or prize in exchange for downloading a file or entering personal details.

### 4.4 Case study: Dropped-USB security experiment

A useful documented example of the physical baiting technique is the controlled USB experiment reported by CLUSIL in Luxembourg. In its 2025 USB Project, the organisation distributed harmless, instrumented USB devices in public and semi-public locations to examine whether people would connect unknown devices to computers. The devices recorded whether they were plugged in and whether their contents were opened; the experiment described the devices as harmless and did not collect personal data.

The project demonstrates that the curiosity behind a dropped-USB attack remains a practical security concern. It is a controlled awareness experiment, not a report of a criminal malware infection or a confirmed corporate breach.

**Impact and lessons:**

- Unknown removable media should never be connected to workplace devices.
- Clear reporting procedures are needed for found USB devices.
- Organisations should technically restrict or control removable media.
- Security awareness should explain that a labelled or apparently lost device is not necessarily safe.

### 4.5 Prevention measures for baiting

1. **Do not connect unknown devices:** Never plug an untrusted USB drive or other found device into a personal or company computer. Give it to the IT or security team.
2. **Use removable-media controls:** Organisations should disable unauthorised USB storage where practical, allow only approved devices and use endpoint protection to scan permitted media.
3. **Download software only from trusted sources:** Use official websites and approved application stores. Avoid pirated software, suspicious advertisements, unknown links and unexpected free offers.

---

## 5. Quid Pro Quo (Bonus)

### 5.1 Definition

Quid Pro Quo is a social engineering technique in which an attacker offers a service, benefit or reward in exchange for information or access. The phrase means “something for something”.

The attacker may pretend to provide technical support, a free service, a gift or a benefit. The victim is persuaded to share credentials, install software or perform an unsafe action in return.

**Example:** A caller claims to be from technical support and offers to fix an employee's computer. In return, the caller asks the employee to reveal a password or install remote-access software from an unapproved source.

### 5.2 Prevention

- Use only official IT support channels and approved service providers.
- Do not exchange passwords, OTPs or confidential information for gifts or services.
- Verify unexpected offers independently and report suspicious requests.
- Require approved software installation and remote-access procedures.

---

## 6. Comparison of Social Engineering Attacks

| Attack type | Primary target | Psychological lever exploited | Best countermeasure |
|---|---|---|---|
| Phishing | Email and messaging users | Urgency, fear, trust and curiosity | Verify links and senders; report suspicious messages; use phishing-resistant MFA |
| Spear phishing | Selected employees or teams | Personalisation and familiarity | Targeted awareness training and independent verification |
| Whaling | Senior executives and finance leaders | Authority, urgency and responsibility | Dual approval for sensitive actions and out-of-band verification |
| Vishing | Employees and individuals receiving calls | Authority, fear and pressure | End the call and call back using a verified number |
| Smishing | Mobile phone users | Urgency, convenience and fear | Do not follow unexpected SMS links; use official apps or websites |
| Pretexting | Employees, helpdesk and finance teams | Trust, authority and believable stories | Verify identity independently and follow formal approval workflows |
| Baiting | Employees and curious users | Curiosity, greed and reward | Never use unknown devices or untrusted downloads |
| Quid Pro Quo | Users seeking help or benefits | Helpfulness and expectation of reward | Use approved support channels and never disclose authentication secrets |

---

## 7. Organisational Recommendations: Five-Point Employee Security Awareness Checklist

Organisations should build a continuous security-awareness programme rather than relying on a single annual presentation.

- [ ] **1. Recognise social engineering:** Train employees to identify suspicious emails, fake websites, impersonation, unusual phone calls, unexpected requests and suspicious USB devices.
- [ ] **2. Verify before acting:** Teach employees to verify identities, payment changes, password-reset requests and sensitive instructions using an independent, trusted channel.
- [ ] **3. Protect credentials and MFA:** Explain password security, password managers, phishing-resistant MFA and why employees must never share OTPs or approve unexpected login prompts.
- [ ] **4. Practise reporting and response:** Provide a simple process for reporting phishing, suspicious calls, lost devices and accidental clicks. Encourage early reporting without blaming employees.
- [ ] **5. Test, measure and improve:** Conduct authorised phishing simulations and scenario-based exercises. Track reporting rates, repeat-risk areas and training completion, then update the programme based on results.

### Additional organisational controls

- Apply least privilege so that compromised accounts cannot access unnecessary systems.
- Use email authentication and filtering controls, endpoint protection and web filtering.
- Require dual authorisation for high-value payments and changes to supplier bank details.
- Maintain an incident-response process for compromised credentials and suspected fraud.
- Review helpdesk identity-verification and account-recovery procedures regularly.

---

## 8. Conclusion

Social engineering attacks demonstrate that people can be targeted just as effectively as computers and networks. Phishing uses deceptive communications, pretexting builds trust through a false identity or story, and baiting uses attractive objects or offers to encourage unsafe behaviour. Quid Pro Quo adds the promise of a service or reward in exchange for access or information.

The RSA SecurID incident and the 2020 Twitter incident show how a single employee interaction can lead to a much larger security compromise. The dropped-USB experiment illustrates why physical security awareness is also important.

No single security product can eliminate social engineering. Organisations need a combination of employee education, independent verification, strong authentication, technical controls, clear reporting channels and tested response procedures. Employees should be encouraged to pause, verify and report whenever a request is unexpected or unusual.

---

## 9. References

1. **Verizon.** (2024). *2024 Data Breach Investigations Report (DBIR).*  
   https://www.verizon.com/business/resources/T202/reports/2024-dbir-data-breach-investigations-report.pdf  
   Used for statistics and analysis of the human element, phishing and pretexting in breaches.

2. **Cybersecurity and Infrastructure Security Agency (CISA).** (2024). *Avoid Phishing Scams with Three Simple Tips.*  
   https://www.cisa.gov/sites/default/files/2024-09/Secure-Our-World-Phishing-Tip-Sheet.pdf  
   Used for practical phishing recognition, reporting and response recommendations.

3. **Federal Bureau of Investigation (FBI), Internet Crime Complaint Center (IC3).** (2024). *Cyber Criminals Target Victims Using Social Engineering Techniques.*  
   https://www.ic3.gov/PSA/2024/PSA240411  
   Used for current examples of impersonation, account takeover and social engineering methods.

4. **Federal Bureau of Investigation (FBI), Internet Crime Complaint Center (IC3).** (2024). *2023 Internet Crime Report.*  
   https://www.ic3.gov/AnnualReport/Reports/2023_IC3Report.pdf  
   Used for Business Email Compromise complaint and financial-loss statistics.

5. **New York State Department of Financial Services.** (2020). *Twitter Investigation Report: Report on Investigation of Twitter’s July 15, 2020 Cybersecurity Incident and the Implications for Election Security.*  
   https://www.dfs.ny.gov/reports-and-publications/other-reports/Twitter_Report  
   Used for the Twitter employee social engineering case study.

6. **Computer Weekly.** (2011). *RSA discloses phishing-attack data breach details.*  
   https://www.computerweekly.com/news/1280095593/RSA-discloses-phishing-attack-data-breach-details  
   Used for the RSA SecurID spear-phishing case study.

7. **Microsoft.** (2011). *Microsoft Security Chronicles – April 14, 2011.*  
   https://download.microsoft.com/download/E/5/8/E582E744-3347-40F3-B6FE-E863A5E9292E/Microsoft_Security_Chronicles_April14_2011.pdf  
   Used as a retrospective technical account of the RSA incident.

8. **CLUSIL.** (2025). *USB Project: Are dropped USB keys still a threat?*  
   https://www.clusil.lu/publication-usb-project.html  
   Used for the controlled dropped-USB awareness experiment.

9. **SANS Institute.** *SANS Reading Room – Information Security White Papers.*  
   https://www.sans.org/white-papers/  
   Recommended academic-quality further reading on social engineering, phishing and security awareness.

10. **Federal Bureau of Investigation (FBI).** *Spoofing and Phishing.*  
    https://www.fbi.gov/how-we-can-help-you/common-frauds-and-scams/spoofing-and-phishing  
    Used for phishing, spoofing, vishing and smishing definitions and safety guidance.

---

**End of Report**
