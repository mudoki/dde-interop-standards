# Decentralised Data Exchange: Interoperability Standards Catalogue

*Under active development as part of an ongoing PhD literature survey.*

This catalogue lists the standards being surveyed,
with their standards body and process status, across four 
interoperability layers (Technical, Semantic, Legal, Organisational) 
defined in the [European Interoperability Framework](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=COM:2017:134:FIN). 
"RF" = royalty-free. "RDF-native" indicates
whether the standard plugs directly into the Semantic Web stack or
requires bridging.

**Legend**

**Open/RF** - licensing of the standard itself:
- `Yes` - openly published and royalty-free under the issuing body's patent policy
- `Open` - openly published; no blanket royalty-free patent grant
- `Licensed` - requires a licence to implement or use

**RDF-native** - how the standard relates to the Semantic Web stack:
- `Yes` - plugs in directly (RDF-based)
- `No` - not RDF-based
- `Partial` - connects through a documented bridge (e.g. `DCAT+ODRL`, DPV extension)
- `n/a` - sits below the data layer, does not apply


## Layer 1 - Technical

| Standard | Version | Body | Status (2026) | Open/RF | RDF-native | Role |
|---|---|---|---|---|---|---|
| [HTTP](https://httpwg.org/specs/) | 1.1/2/3 | IETF | Internet Standard | Yes | n/a | Transport substrate |
| [TLS](https://datatracker.ietf.org/wg/tls/about/ ) | 1.3 | IETF | RFC 8446 | Yes | n/a | Channel security |
| [Linked Data Platform](https://www.w3.org/TR/ldp/) | 1.0 | W3C | Rec (2015) | Yes | Yes | Read/write linked data |
| [Solid Protocol](https://solidproject.org/TR/protocol) | 0.11 | W3C Solid CG | CG Report | Yes | Yes | Decentralised storage interface |
| [Linked Data Notifications](https://www.w3.org/TR/ldn/) | 1.0 | W3C | Rec (2017) | Yes | Yes | RDF notifications |
| [Activity Streams](https://www.w3.org/TR/activitystreams-core/) | 2.0 | W3C | Rec (2017) | Yes | Yes | Activity/event vocabulary |
| [SPARQL Protocol](https://www.w3.org/TR/sparql12-protocol/) | 1.1 / 1.2 CR | W3C | Rec; 1.2 Candidate Rec | Yes | Yes | Query transport |
| [Linked Web Storage WG](https://www.w3.org/groups/wg/lws/) | -- | W3C | WG (active) | Yes | Yes | Server-side storage Recs (in progress) |

## Layer 2 - Semantic

| Standard | Version | Body | Status (2026) | Open/RF | RDF-native | Role |
|---|---|---|---|---|---|---|
| [RDF](https://www.w3.org/TR/rdf12-concepts/) | 1.1 / 1.2 CR | W3C | Rec (2014); 1.2 Candidate Rec (Apr 2026) | Yes | Yes | Core data model |
| [RDFS](https://www.w3.org/TR/rdf-schema/) | 1.1 | W3C | Rec (2014) | Yes | Yes | Lightweight schema |
| [OWL 2](https://www.w3.org/TR/owl2-overview/) | 2 | W3C | Rec (2012) | Yes | Yes | Ontology language |
| [SKOS](https://www.w3.org/TR/skos-reference/) | 1.0 | W3C | Rec (2009) | Yes | Yes | Taxonomies |
| [SPARQL Query](https://www.w3.org/TR/sparql12-query/ ) | 1.1 / 1.2 CR | W3C | Rec (2013); 1.2 Candidate Rec | Yes | Yes | Querying RDF |
| [SHACL](https://www.w3.org/TR/shacl/ ) | 1.0 / 1.2 WD | W3C | Rec (2017); 1.2 in progress | Yes | Yes | Shape validation | |
| [JSON-LD](https://www.w3.org/TR/json-ld11/) | 1.1 | W3C | Rec (2020) | Yes | Yes | JSON for linked data |
| [R2RML](https://www.w3.org/TR/r2rml/) | 1.0 | W3C | Rec (2012) | Yes | Yes | Relational-to-RDF mapping |
| [RML](https://w3id.org/rml/) | -- | W3C KGC CG | CG work | Yes | Yes | Heterogeneous-source mapping |
| [DCAT](https://www.w3.org/TR/vocab-dcat-3/) | 3 | W3C | Rec (2024) | Yes | Yes | Dataset description/discovery |
| [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/) | 3.0 | EU SEMIC | EU profile | Yes | Yes | EU profile of DCAT |
| [Dublin Core Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/) | 1.1 | DCMI | DCMI Standard | Yes | Yes | Descriptive metadata |

## Layer 3 - Legal

| Standard | Version | Body | Status (2026) | Open/RF | RDF-native | Role |
|---|---|---|---|---|---|---|
| [ODRL](https://www.w3.org/TR/odrl-model/ ) | 2.2 | W3C | Rec (2018) | Yes | Yes | Policy / usage-control expression |
| [Data Privacy Vocabulary (DPV)](https://w3id.org/dpv) | 2.3 | W3C DPVCG | CG Report (Feb 2026) | Yes | Yes | Privacy/data-protection concepts |
| [OAC (ODRL profile for Access Control)](https://w3id.org/oac) | -- | research/CG | CG-level | Yes | Yes | Access-control policies (Solid) |
| [XACML](https://docs.oasis-open.org/xacml/3.0/xacml-3.0-core-spec-en.html) | 3.0 | OASIS | OASIS Standard | Yes | No (XML) | Attribute-based access control |

## Layer 4 - Organisational

| Standard | Version | Body | Status (2026) | Open/RF | RDF-native | Role |
|---|---|---|---|---|---|---|
| [Decentralized Identifiers (DIDs)](https://www.w3.org/TR/did-1.1/) | 1.0 / 1.1 CR | W3C | Rec (2022); 1.1 Candidate Rec | Yes | Yes | Self-controlled identifiers |
| [WebID]( https://www.w3.org/TR/did-1.1/) | -- | W3C Solid CG | CG Report | Yes | Yes | HTTP-URI agent identity |
| [Verifiable Credentials Data Model](https://www.w3.org/TR/vc-data-model-2.0/) | 2.0 | W3C | Rec (May 2025) | Yes | Yes | Verifiable claims |
| [PROV-O](https://www.w3.org/TR/prov-o/) | 1.0 | W3C | Rec (2013) | Yes | Yes | Provenance |
| [OAuth 2.0](https://www.rfc-editor.org/rfc/rfc6749) | RFC 6749 | IETF | RFC | Open | No | Delegated authorisation |
| [OpenID Connect](https://openid.net/specs/openid-connect-core-1_0.html) | Core 1.0 | OpenID Foundation | Final | Open | No | Identity layer over OAuth |
| [UMA 2.0](https://docs.kantarainitiative.org/uma/wg/rec-oauth-uma-grant-2.0.html) | 2.0 | Kantara | Kantara Rec | Open | No | Party-to-party data-sharing authorisation |
| [JSON Web Token (JWT)](https://www.rfc-editor.org/info/rfc7519/ ) | RFC 7515–7519 | IETF | RFC | Yes | No | Token signing/encryption |
| [IEEE 7012](https://standards.ieee.org/ieee/7012/7192/ ) | 2025 | IEEE | IEEE Standard | Licensed | Partial | Machine-readable privacy terms |
| [Dataspace Protocol (DSP)](https://eclipse-dataspace-protocol-base.github.io/DataspaceProtocol/2025-1/) | 2025-1 | Eclipse / IDSA | Eclipse Spec | Yes | Yes (DCAT+ODRL) | Connector negotiation/transfer |
<!-- | [VC Data Integrity (+cryptosuites)](https://www.w3.org/TR/vc-data-integrity/) | 1.0 | W3C | Rec (May 2025) | Yes | Yes | Signing/verifying linked data | -->
<!-- | [Controlled Identifiers](https://www.w3.org/TR/controlled-identifiers/) | 1.0 | W3C | Rec (May 2025) | Yes | Yes | Identifier control for VCs | -->
<!-- | [Bitstring Status List](https://www.w3.org/TR/vc-bitstring-status-list/) | 1.0 | W3C | Rec (May 2025) | Yes | Yes | VC revocation/status | -->
<!-- | [RDF Dataset Canonicalization](https://www.w3.org/TR/rdf-canon/ ) (RDFC-1.0) | 1.0 | W3C | Rec (2024) | Yes | Yes | Canonical form for signing RDF | -->

## Domain-specific (health; via the EHDS scenario)

| Standard | Version | Body | Status (2026) | Open/RF | RDF-native | Role |
|---|---|---|---|---|---|---|
| HL7 FHIR | R5 | HL7 | HL7 Standard | Open spec | RDF serialisation exists | Clinical data exchange |
| SNOMED CT | -- | SNOMED Intl. | Intl. Standard | Licensed | Mappable | Clinical terminology |
