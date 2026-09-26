# NIS2 Knowledge Base

An English-language [Open Knowledge Format (OKF)](https://github.com/GoogleCloudPlatform/knowledge-catalog/blob/main/okf/SPEC.md) bundle covering the EU NIS2 Directive (Directive (EU) 2022/2555), its implementing regulation, the national laws that transpose it, the authorities and CSIRTs that enforce it, and the official guidance around it.

The bundle will contain concise original summaries with provision-level citations to primary sources. It does not reproduce full legal instruments, rules, guidance documents, or standards.

Current release: **none yet** (`VERSION` 0.0.0)

> **Scaffold:** the manifest, section structure, validator and registers are in place. No concepts have been ingested yet; every section index describes what will go there.

> **General orientation only:** once populated, do not rely on this knowledge base for decisions that determine, demonstrate, or materially affect legal or regulatory compliance. Verify the current primary sources and obtain qualified professional advice before making entity-classification, registration, risk-management-measure, reporting, supervisory, or other compliance-impacting decisions.

## Use With Meerkat

[Meerkat](https://github.com/zegit-zoo/meerkat) can serve the bundle as CLI, MCP, or HTTP without conversion:

```sh
mk --kb-dir . search "reporting obligations"
mk --kb-dir . show law/eu/nis2/articles/article-23
mk --kb-dir . list --category law
mk --kb-dir . mcp serve
mk --kb-dir . http serve --port 4004
```

Run these commands from the repository root. The knowledge bundle itself is under `wiki/`; Meerkat's `--kb-dir` reads that content-repository layout. The paths above are the planned concept IDs and resolve once ingestion has reached them.

The Markdown remains usable without Meerkat or any other tool.

## Coverage

The intended corpus includes:

- Directive (EU) 2022/2555, its annexes, corrigenda and Implementing Regulation (EU) 2024/2690;
- essential and important entity classification, governance, Article 21 measures, Article 23 reporting, registration and supply-chain duties;
- Annex I and Annex II sectors and entity types;
- ENISA, NIS Cooperation Group and Commission guidance;
- the 27 national transpositions with authorities, CSIRTs, deadlines and penalties, plus EEA status;
- interacting EU legislation, in particular the Cyber Resilience Act and DORA.

Coverage is measured in `coverage.yaml`. Each gate names a glob over `wiki/`, the expected number of concepts where the corpus is finite, and the count actually present. A missing official source is recorded as a research gap rather than filled by inference.

## Structure

`kb.yaml` declares the bundle's slug, extension key (`x-nis2`), categories and sections. Every section has an `index.md` describing what belongs there.

| Section | Contents |
|---|---|
| [`law/`](wiki/law/index.md) | Directive (EU) 2022/2555 article by article, its annexes, Implementing Regulation (EU) 2024/2690 and later acts, and interacting EU law (CRA, CER, DORA, GDPR, Cybersecurity Act). |
| [`obligations/`](wiki/obligations/index.md) | Role and lifecycle views: who is an essential or important entity, governance duties, Article 21 risk-management measures, Article 23 reporting clocks, registration, supply-chain security and jurisdiction. |
| [`sectors/`](wiki/sectors/index.md) | Annex I sectors of high criticality and Annex II other critical sectors, with the entity types each sector covers. |
| [`authorities/`](wiki/authorities/index.md) | EU-level bodies: competent authorities as a role, single points of contact, CSIRTs and the CSIRTs network, the NIS Cooperation Group, EU-CyCLONe, ENISA and the European vulnerability database. |
| [`guidance/`](wiki/guidance/index.md) | Official non-binding guidance: ENISA technical implementation guidance, NIS Cooperation Group documents, Commission guidelines and FAQs, national authority guidance. |
| [`standards/`](wiki/standards/index.md) | Standards the directive, the implementing regulation and national schemes refer to (ISO/IEC 27001, IEC 62443, ETSI EN 319 401 and others), recorded as identifiers, lifecycle facts and links. |
| [`jurisdictions/`](wiki/jurisdictions/index.md) | Every EU Member State's transposing law, competent authorities, CSIRT, registration deadline and penalty framework, plus EEA status. |
| [`timeline/`](wiki/timeline/index.md) | Entry into force, transposition deadline, implementing-regulation application, national registration and reporting dates, review clauses. |
| [`glossary/`](wiki/glossary/index.md) | Terms defined in Article 6 of Directive (EU) 2022/2555. |

## Source And Publication Policy

- Binding claims cite OJEU, ELI, EUR-Lex, or an official national gazette.
- Official guidance is labelled non-binding.
- A standard provides presumption of conformity only when its reference is cited in the OJEU for the requirements concerned.
- Publicly accessible drafts are linked, not copied.
- National transposition pages cite the national gazette or official legal database of the Member State.
- The CRA interface is described here but the CRA itself is covered by [CRA-knowledge-base](https://github.com/JonasLundin/CRA-knowledge-base); pages link rather than duplicate.
- Agent-generated content stays `status: draft` until a human verifies it against the cited source.
- Superseded material is retained and marked rather than silently deleted.

This repository is not legal advice, is not a conformity assessment, does not certify any product or organisation, and must not be used as the basis for compliance-impacting decisions.

## Validate

```sh
python3 -m pip install -r requirements-dev.txt
python3 -m unittest tools/test_validate.py
python3 tools/validate.py wiki
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Corrections with exact primary-source citations are welcome. Do not submit copied standards text, private compliance evidence, or confidential information.

## Related Knowledge Bases

- [CRA-knowledge-base](https://github.com/JonasLundin/CRA-knowledge-base): Regulation (EU) 2024/2847, the Cyber Resilience Act
- [CVD-knowledge-base](https://github.com/JonasLundin/CVD-knowledge-base): coordinated vulnerability disclosure, the CVE Program, CSAF, VEX and scoring
- [AI-Act-knowledge-base](https://github.com/JonasLundin/AI-Act-knowledge-base): Regulation (EU) 2024/1689 as amended
- [Conformity-Assessment-knowledge-base](https://github.com/JonasLundin/Conformity-Assessment-knowledge-base): the New Legislative Framework, modules, accreditation and notified bodies
- [Software-Supply-Chain-knowledge-base](https://github.com/JonasLundin/Software-Supply-Chain-knowledge-base): SBOM formats, attestation, provenance and VEX
- [NIST-CSF-knowledge-base](https://github.com/JonasLundin/NIST-CSF-knowledge-base): NIST Cybersecurity Framework 2.0
- [knowledge-base-template](https://github.com/JonasLundin/knowledge-base-template): the shared template every bundle in the series is built from

## Licence

Original summaries, structure, and metadata are licensed under [CC BY 4.0](LICENSE). Source documents, rules, specifications and standards retain their own terms; see [NOTICE](NOTICE).

This project is independent and is not affiliated with or endorsed by the European Commission, ENISA, the NIS Cooperation Group, any national authority or CSIRT, ISO, IEC, CEN, CENELEC, ETSI, Google Cloud, or Meerkat. Repository: https://github.com/JonasLundin/NIS2-knowledge-base
