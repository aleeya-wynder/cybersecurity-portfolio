# Learning Log

Weekly notes from my cybersecurity studies: Transition to Cyber, WGU, and TryHackMe.
Newest entries at the top.

---

## Week 1: Foundations of Cybersecurity & the CIA Triad
*Transition to Cyber program · Week of Nov 1, 2026*

### What I learned
- **Confidentiality:** only authorized people can access data. Threats: data breaches, phishing for passwords, insider leaks.
- **Integrity:** data stays accurate and isn't changed without permission. Threats: tampering, man-in-the-middle attacks.
- **Availability:** systems and data are accessible when needed. Threats: ransomware, DDoS attacks, hardware failure.

### Lab: Front-Line Security Scenarios
Worked through 5 industry scenarios (healthcare, finance, retail, and more) as the
employee on the front line. For each one, I picked the safest response and identified
which part of the CIA triad was at risk.

**Example: Healthcare**
- **Situation:** A caller claiming to be a physician asked a hospital scheduler to email
  a patient's full chart to their personal Gmail "just this once."
- **My response:** Direct them to the hospital's approved secure portal instead.
- **CIA element at risk:** Confidentiality
- **Why:** Patient records are protected health information (HIPAA). Sending them to a
  personal email moves them outside the hospital's control, and the caller's identity
  wasn't verified.
- **Red flags I spotted:** urgency ("between rooms"), a request to bypass normal process
  ("just this once"), and an unverified identity over the phone. These are classic
  social engineering tactics.
- **Lesson:** The secure option still helps the person get what they need. Security
  works best when it doesn't just say "no."

**Example: Finance**
- **Situation:** A credit union customer emailed asking to change their wire transfer
  recipient to a new account "because their old bank is closing." The email chain
  looked legitimate.
- **My response:** Call the customer at the phone number already on file to verify
  before making any change.
- **CIA element at risk:** Integrity
- **Why:** If the email is fake, the attacker gets the account details changed and
  the customer's money goes to them. This is Business Email Compromise (BEC).
  Replying to the email doesn't help, because the attacker may control that inbox.
- **Red flags I spotted:** a request to change payment details, a believable excuse,
  and an email thread that seems trustworthy. Attackers often hijack real threads.
- **Lesson:** Verify out-of-band, through a separate channel you already trust (like
  the phone number on record). It's the industry-standard defense against BEC.

**Example: Government**
- **Situation:** A city's online permit portal was down all morning, and residents
  couldn't submit applications.
- **My response:** Notify IT/security, write down the symptoms (when it started, what
  errors appear), and post a clear status update with an expected timeline for the
  public.
- **CIA element at risk:** Availability
- **Why:** Residents can't reach a service they depend on. The outage could be a
  technical failure or an attack such as a DDoS, so it needs to be investigated as an
  incident rather than just waited out.
- **Lesson:** Incident response isn't only technical. Getting the right people
  involved quickly and keeping the public informed are part of the job.
