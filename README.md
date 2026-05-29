# Standards for Interoperable Decentralised Data Exchange

Organised by the four interoperability layers
(Technical, Semantic, Legal, Organisational) of the European
Interoperability Framework. "RF" = royalty-free. "RDF-native" indicates
whether the standard plugs directly into the Semantic Web stack or
requires bridging.

## Layer 1 -- Technical

| Standard | Version | Body | Status (2026) | Open/RF | RDF-native | Role |
|---|---|---|---|---|---|---|
| HTTP | 1.1/2/3 | IETF | Internet Standard | Yes | n/a | Transport substrate |
| TLS | 1.3 | IETF | RFC 8446 | Yes | n/a | Channel security |
| Linked Data Platform | 1.0 | W3C | Rec (2015) | Yes | Yes | Read/write linked data |
| Solid Protocol | 0.11 | W3C Solid CG | CG Report | Yes | Yes | Decentralised storage interface |
| Linked Data Notifications | 1.0 | W3C | Rec (2017) | Yes | Yes | RDF notifications |
| Activity Streams | 2.0 | W3C | Rec (2017) | Yes | Yes | Activity/event vocabulary |
| SPARQL Protocol | 1.1 / 1.2 CR | W3C | Rec; 1.2 Candidate Rec | Yes | Yes | Query transport |

## Layer 2 -- Semantic

| Standard | Version | Body | Status (2026) | Open/RF | RDF-native | Role |
|---|---|---|---|---|---|---|
| RDF | 1.1 / 1.2 CR | W3C | Rec (2014); 1.2 Candidate Rec (Apr 2026) | Yes | Yes | Core data model |
| RDFS | 1.1 | W3C | Rec (2014) | Yes | Yes | Lightweight schema |
| OWL 2 | 2 | W3C | Rec (2012) | Yes | Yes | Ontology language |
| SKOS | 1.0 | W3C | Rec (2009) | Yes | Yes | Taxonomies |
| SPARQL Query | 1.1 / 1.2 CR | W3C | Rec (2013); 1.2 Candidate Rec | Yes | Yes | Querying RDF |
| SHACL | 1.0 / 1.2 WD | W3C | Rec (2017); 1.2 in progress | Yes | Yes | Shape validation |
| JSON-LD | 1.1 | W3C | Rec (2020) | Yes | Yes | JSON for linked data |
| R2RML | 1.0 | W3C | Rec (2012) | Yes | Yes | Relational-to-RDF mapping |
| RML | -- | W3C KGC CG | CG work | Yes | Yes | Heterogeneous-source mapping |
| DCAT | 3 | W3C | Rec (2024) | Yes | Yes | Dataset description/discovery |
| DCAT-AP | 3.0 | EU SEMIC | EU profile | Yes | Yes | EU profile of DCAT |
| Dublin Core Terms | 1.1 | DCMI | DCMI Standard | Yes | Yes | Descriptive metadata |

## Layer 3 -- Legal

| Standard | Version | Body | Status (2026) | Open/RF | RDF-native | Role |
|---|---|---|---|---|---|---|
| ODRL | 2.2 | W3C | Rec (2018) | Yes | Yes | Policy / usage-control expression |
| Data Privacy Vocabulary (DPV) | 2.3 | W3C DPVCG | CG Report (Feb 2026) | Yes | Yes | Privacy/data-protection concepts |
| DPV regulatory extensions | tracks 2.3 | W3C DPVCG | CG Report | Yes | Yes | GDPR / DGA / EHDS IEEE-7012 concept sets |
| OAC (ODRL profile for Access Control) | -- | research/CG | CG-level | Yes | Yes | Access-control policies (Solid) |
| XACML | 3.0 | OASIS | OASIS Standard | Yes | No (XML) | Attribute-based access control |

## Layer 4 -- Organisational

| Standard | Version | Body | Status (2026) | Open/RF | RDF-native | Role |
|---|---|---|---|---|---|---|
| Decentralized Identifiers (DIDs) | 1.0 / 1.1 CR | W3C | Rec (2022); 1.1 Candidate Rec | Yes | Yes | Self-controlled identifiers |
| WebID | -- | W3C Solid CG | CG Report | Yes | Yes | HTTP-URI agent identity |
| Verifiable Credentials Data Model | 2.0 | W3C | Rec (May 2025) | Yes | Yes | Verifiable claims |
| VC Data Integrity (+cryptosuites) | 1.0 | W3C | Rec (May 2025) | Yes | Yes | Signing/verifying linked data |
| Controlled Identifiers | 1.0 | W3C | Rec (May 2025) | Yes | Yes | Identifier control for VCs |
| Bitstring Status List | 1.0 | W3C | Rec (May 2025) | Yes | Yes | VC revocation/status |
| RDF Dataset Canonicalization (RDFC-1.0) | 1.0 | W3C | Rec (2024) | Yes | Yes | Canonical form for signing RDF |
| PROV-O | 1.0 | W3C | Rec (2013) | Yes | Yes | Provenance |
| OAuth 2.0 | RFC 6749 | IETF | RFC | Yes | No | Delegated authorisation |
| OpenID Connect | Core 1.0 | OpenID Foundation | Final | Yes | No | Identity layer over OAuth |
| UMA 2.0 | 2.0 | Kantara | Kantara Rec | Yes | No | Party-to-party data-sharing authorisation |
| JOSE / JWT | RFC 7515–7519 | IETF | RFC | Yes | No | Token signing/encryption |
| IEEE 7012 | 2025 | IEEE | IEEE Standard | Licensed | Partial | Machine-readable privacy terms |
| Dataspace Protocol (DSP) | 2025-1 | Eclipse / IDSA | Eclipse Spec (ISO-track) | Yes | Yes (DCAT+ODRL) | Connector negotiation/transfer |

## Domain-specific (health; via the EHDS scenario)

| Standard | Version | Body | Status (2026) | Open/RF | RDF-native | Role |
|---|---|---|---|---|---|---|
| HL7 FHIR | R5 | HL7 | HL7 Standard | Open spec | RDF serialisation exists | Clinical data exchange |
| SNOMED CT | — | SNOMED Intl. | Intl. Standard | Licensed | Mappable | Clinical terminology |
