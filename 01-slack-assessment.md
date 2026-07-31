# Vendor Assessment, Slack (as a processor)

**Vendor:** Slack Technologies (part of Salesforce).
**Service:** team communication / messaging (SaaS).
**Role:** processor (Slack processes personal data on the customer's behalf).
**Controller:** the adopting organisation (EEA / Finland).
**Basis of assessment:** Slack's publicly available Data Processing Addendum, GDPR/trust pages, and sub-processor documentation.

---

## 1. Processor contract (Article 28)

Article 28 requires a binding contract (a DPA) with specific mandatory terms before a processor handles personal data on a controller's behalf.

**Findings:**
- Slack publishes a **standard Data Processing Addendum** that customers can incorporate, and it is designed to meet GDPR requirements.
- The DPA **incorporates the EU (and UK) Standard Contractual Clauses** for international transfers.

**Assessment:** A published, GDPR-oriented DPA that incorporates SCCs satisfies the core Article 28 requirement for a written processor contract. **Action for the controller:** ensure the DPA is actually put in place (referenced or signed) as part of the contract, not merely available, this is a common gap where a DPA exists but is never executed.

---

## 2. Sub-processor governance (Article 28(2), 28(4))

A processor may only engage sub-processors under conditions: prior authorisation, a current list, notice of changes, and a right to object.

**Findings (from the DPA):**
- Slack operates a **general authorisation** model for sub-processors: the customer authorises Slack to engage sub-processors listed and updated per the DPA.
- Slack **maintains a current list of sub-processors** and provides a **subscription mechanism** so customers can be **notified of new sub-processors** before they start processing.
- Customers have a defined **right to object** to a new sub-processor (the DPA sets a window, historically ten business days, to raise a reasonable objection).

**Assessment:** This meets the Article 28 sub-processor conditions, general authorisation is permitted provided notice and an objection right exist, which they do. **Action for the controller:** actually **subscribe to the sub-processor notification list** and assign someone to review changes, the objection right is worthless if no one is watching for new sub-processors.

---

## 3. International data transfers (Chapter V)

Slack is US-headquartered (Salesforce), so EEA personal data is likely transferred outside the EEA, engaging Chapter V.

**Findings:**
- Slack's DPA **incorporates EU/UK Standard Contractual Clauses** as a transfer mechanism.
- Through Salesforce, Slack participates in the **EU-US Data Privacy Framework** (and the UK extension and Swiss-US DPF).
- Salesforce also references **Binding Corporate Rules** for certain services.

**Assessment:** Multiple valid transfer mechanisms are in place (SCCs plus DPF participation). This is a reasonably strong transfer posture. **Action for the controller:** post-*Schrems II*, SCCs alone are not automatically sufficient, the controller should record a brief **transfer risk assessment** noting that DPF participation and SCCs both apply, and confirm whether any data-residency options (Slack offers some at the Enterprise tier) are relevant to its risk appetite.

---

## 4. Security (Article 32)

**Findings:**
- Slack holds **ISO 27001** and the related **ISO 27017** (cloud security) and **ISO 27018** (cloud personal-data protection) certifications.
- Encryption, access controls, and audited security practices are described in its trust documentation.

**Assessment:** Recognised, independently audited certifications indicate appropriate technical and organisational measures under Article 32. **Action for the controller:** retain copies of the current certificates as evidence, and note the renewal dates.

---

## 5. Data-subject-request support (Article 28(3)(e))

A processor must help the controller respond to data-subject requests.

**Findings:**
- Slack provides **tooling and documented processes** to help customers locate, export, and delete user data, supporting the controller's obligations for access and erasure requests.

**Assessment:** Adequate. This directly supports the controller's own DSAR handling (see the DSAR project). **Action for the controller:** understand *which* admin tools produce the export, before a request arrives, not during the one-month clock.

---

## 6. Recommendation and residual risk

| Area | Rating |
|------|--------|
| Processor contract (DPA) | Strong |
| Sub-processor governance | Strong (if notifications are monitored) |
| International transfers | Adequate (record a transfer risk assessment) |
| Security | Strong |
| DSR support | Adequate |

**Overall: acceptable to adopt, with conditions.**

**Recommendation:** Slack can be adopted as a processor. It offers a GDPR-oriented DPA with SCCs, DPF participation, strong security certifications, and sub-processor transparency, which collectively satisfy the Article 28 and Chapter V requirements. Adoption should be conditional on the controller completing four practical steps:

1. **Execute** the DPA (do not just rely on it being published).
2. **Subscribe to and monitor** the sub-processor notification list, and assign an owner.
3. **Record a short transfer risk assessment** covering the SCCs / DPF position.
4. **Retain** the security certificates and identify the DSR export tooling in advance.

**Residual risk:** low to moderate, driven mainly by the international-transfer position (inherent to any US-based SaaS) and by the *operational* risk that the controller fails to monitor sub-processor changes. Both are manageable with the steps above.

---

## Reflection

The pattern this illustrates: for a mature vendor like Slack, the **documentation is usually strong**, the real risk sits with the **controller's own follow-through**, executing the DPA, watching for sub-processor changes, and recording the transfer assessment. Vendor assessment is not only reading the vendor's paperwork; it is identifying the **actions the controller must take** to make the relationship compliant and keep it that way.
