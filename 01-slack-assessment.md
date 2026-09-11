# Vendor Assessment: Slack (as a processor)

Vendor: Slack Technologies (part of Salesforce). Service: team communication and messaging (SaaS). Role: processor, Slack processes personal data on the customer's behalf. Controller: the adopting organisation (EEA, Finland). Basis of assessment: Slack's publicly available Data Processing Addendum, GDPR and trust pages, and sub-processor documentation.

## Processor contract (Article 28)

Article 28 requires a binding contract with specific mandatory terms before a processor can handle personal data on a controller's behalf. Slack publishes a standard Data Processing Addendum built to meet GDPR requirements, and it incorporates the EU and UK Standard Contractual Clauses for international transfers. That satisfies the core requirement for a written processor contract.

The gap tends to sit elsewhere: a DPA being published isn't the same as it being executed. Controllers need to actually put it in place, referenced or signed as part of the contract, not just left available on a legal page nobody visits.

## Sub-processor governance (Article 28(2), 28(4))

A processor can only engage sub-processors under specific conditions, prior authorisation, a current list, notice of changes, and a right to object. Slack's DPA uses a general authorisation model: the customer authorises Slack to engage the sub-processors listed and updated under the DPA, with a subscription mechanism for notifications before a new one starts processing, and a defined objection window (historically ten business days).

That structure satisfies Article 28's conditions. What it doesn't do on its own is guarantee anyone's watching, the right to object only has value if the controller actually subscribes to the notification list and assigns someone to review it. Otherwise it's a right that exists on paper and nowhere else.

## International data transfers (Chapter V)

Slack is US-headquartered through Salesforce, so EEA personal data is likely transferred outside the EEA, which engages Chapter V. Slack's DPA incorporates SCCs, and through Salesforce, Slack also participates in the EU-US Data Privacy Framework (plus the UK extension and Swiss-US DPF), with Binding Corporate Rules referenced for certain services.

Two valid mechanisms stacked together is a reasonably strong position. Since Schrems II, though, SCCs alone don't automatically clear the bar, controllers should keep a short written transfer risk assessment on file noting that both DPF participation and SCCs apply, and check whether Slack's Enterprise-tier data residency options matter for their own risk appetite.

## Security (Article 32)

Slack holds ISO 27001, ISO 27017 (cloud security), and ISO 27018 (cloud personal data protection), with encryption, access controls, and audited practices documented in its trust materials. Independently audited certifications at this level are solid evidence of appropriate technical and organisational measures. The only real action item here is administrative: keep copies of the current certificates and track renewal dates, since certifications lapse.

## Data subject request support (Article 28(3)(e))

Slack provides tooling to locate, export, and delete user data, which supports a controller's own access and erasure obligations. This is adequate, and it connects directly to a controller's DSAR process. The practical step worth taking early: know which admin tool produces the export before a request lands, not during the one-month response clock.

## Recommendation

| Area | Rating |
|------|--------|
| Processor contract (DPA) | Strong |
| Sub-processor governance | Strong, if notifications are monitored |
| International transfers | Adequate, record a transfer risk assessment |
| Security | Strong |
| Data subject request support | Adequate |

Slack can be adopted as a processor. The DPA, SCCs, DPF participation, security certifications, and sub-processor transparency together satisfy Article 28 and Chapter V. Adoption should carry four conditions: execute the DPA rather than relying on it being published, subscribe to and actively monitor the sub-processor notification list with a named owner, record a short transfer risk assessment covering the SCC and DPF position, and retain security certificates while identifying DSR export tooling in advance.

Residual risk sits at low to moderate, mostly from the international transfer position, which is inherent to any US-based SaaS, and from the operational risk of a controller not tracking sub-processor changes. For a vendor at Slack's scale, the documentation itself is rarely the weak point. It's the controller's own follow-through, executing the DPA, watching for changes, keeping the transfer assessment current, that determines whether the relationship stays compliant over time.
