# Universal Music Group (universal-music-group)

Universal Music Group N.V. (UMG) is the world's largest music company, headquartered in Hilversum, Netherlands with operational headquarters in Santa Monica, California. Spun off from Vivendi and listed on Euronext Amsterdam (ticker: UMG) on September 21, 2021 at a EUR 54 billion valuation, UMG operates Recorded Music, Music Publishing (Universal Music Publishing Group / UMPG), and Merchandising (Bravado), plus film and television production (PolyGram Entertainment) and the artist services and catalog arm Universal Music Enterprises. The company is led by Chairman and CEO Sir Lucian Grainge. Major label families include Republic Corps (Republic, Island, Def Jam), Interscope Capitol Labels Group (Interscope, Geffen, A&M, Capitol, Blue Note, Motown), Virgin Music Group, Verve Label Group (Verve, Decca, Deutsche Grammophon, Impulse!, Philips), UMG Nashville (MCA Nashville, Mercury Nashville, EMI Records Nashville, Capitol Records Nashville), Universal Music Latin Entertainment, and Universal Music UK. Catalog scale exceeds 3 million recordings and 4 million compositions. Ownership is split among Bolloré / Vivendi (~28%), Tencent Music (~11%), Pershing Square (~10%), and the public float. UMG operates no public developer portal: catalog and metadata reach developers only indirectly through downstream DSPs (Spotify, Apple Music, YouTube, Amazon Music) and through partner / aggregator programs (7digital exposed UMG catalog under a partner API; that integration is the only third-party developer-facing surface that has ever been openly documented). Royalty and publishing portals (UMG Royalty Portal, UMPG Window) exist for songwriters and rights holders behind authentication, not as APIs. AI is the active integration vector in 2025-2026: UMG has announced licensed generative-music partnerships with Udio, Splice, KLAY Vision, SoundLabs, ProRata, BandLab, YouTube, TikTok, Meta, and KDDI, and has filed 15+ AI patents with Liquidax Capital across collaboration, rights management, music & health, and AI threat protection. These integrations operate through bilateral commercial agreements, not a self-serve developer program. The official Universal-Music-Group GitHub organization (created May 15, 2024) has 0 public repositories.

**URL:** [Visit APIs.json URL](https://www.universalmusic.com)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - AI Licensing, Big Three, Catalog, Entertainment, Generative Music, Licensing, Major Label, Merchandising, Music, Music Publishing, Recorded Music, Royalties, Streaming

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-23

## APIs

### UMG Corporate Web Surface

The universalmusic.com corporate site is the public-facing surface for Universal Music Group. It catalogs UMG's labels, divisions, news, sustainability, careers, and investor relations content. The site is a marketing and brand surface; no JSON or REST endpoints, no developer documentation, and no API key issuance are exposed. The catalog of artists, releases, and recordings is not surfaced as a queryable API.

**Human URL:** [https://www.universalmusic.com](https://www.universalmusic.com)

#### Tags:

 - Brand, Corporate, News

#### Properties

- [Website](https://www.universalmusic.com)
- [AboutUs](https://www.universalmusic.com/about/)
- [News](https://www.universalmusic.com/news/)
- [Labels](https://www.universalmusic.com/labels/)

### UMG Royalty Portal

Authenticated royalty statement portal for UMG-distributed artists and labels. Provides login-gated access to royalty statements, statement history, and supporting documentation. The portal is delivered as a web application; no public REST API, no OAuth program, and no machine-readable royalty feed are published. Access is provisioned through label and business-affairs channels rather than developer sign-up.

**Human URL:** [https://umgroyalty.com](https://umgroyalty.com)

#### Tags:

 - Authenticated, Royalties, Statements

#### Properties

- [Portal](https://umgroyalty.com)
- [Documentation](https://umgroyalty.com/includes/UserGuide.pdf)
- [Support](https://support.umgroyalty.com/hc/en-us)

### UMPG Window

Universal Music Publishing Group's songwriter and client royalty portal, providing real-time access to earnings, statements, registrations, and catalog data for UMPG-signed songwriters and publisher administration clients. Authenticated, login-gated; no public API, OAuth surface, or developer documentation. The UMPG Window iOS and Android apps wrap the same authenticated surface.

**Human URL:** [https://umpgwindow.com](https://umpgwindow.com)

#### Tags:

 - Authenticated, Compositions, Music Publishing, Royalties, Songwriters

#### Properties

- [Portal](https://umpgwindow.com)
- [Website](https://www.umusicpub.com)

### Bravado Merchandise Storefronts

Bravado is UMG's global merchandise and brand-management division, operating direct-to-consumer artist merchandise storefronts and tour merchandise for UMG's roster. Each artist store is delivered via e-commerce platforms (typically Shopify) under artist-branded domains coordinated by Bravado. No Bravado-branded public developer API, catalog feed, or partner program is documented; integrations to retail and platform partners operate through bilateral commercial agreements.

**Human URL:** [https://www.bravado.com](https://www.bravado.com)

#### Tags:

 - Brand Management, E-Commerce, Merchandise, Tour

#### Properties

- [Website](https://www.bravado.com)

### UMG Catalog Delivery to DSPs

UMG's recorded-music catalog reaches developers and end users almost exclusively through downstream Digital Service Providers (Spotify, Apple Music, Amazon Music, YouTube Music, Tidal, Deezer, Pandora, etc.). UMG delivers audio, video, and metadata to those platforms through private ingest pipelines (industry-standard DDEX ERN / RIN / MEAD messaging delivered over SFTP or vendor-specific APIs). End developers query UMG-owned content through each DSP's own public API, not through any UMG-branded API surface. UMG itself publishes no DSP-style public catalog API.

**Human URL:** [https://www.universalmusic.com](https://www.universalmusic.com)

#### Tags:

 - Catalog, DDEX, Distribution, DSP, Metadata

#### Properties

- [ReferenceStandard](https://ddex.net/)
- [PartnerProgram](https://www.universalmusic.com/contact/)

### 7digital UMG Catalog API (Partner Surface)

7digital operates a B2B catalog and media-delivery API that includes UMG-licensed recordings for hackathon and partner use. This is the closest thing to a publicly documented developer surface for UMG catalog content, but the endpoint, authentication, and commercial terms are owned and operated by 7digital, not UMG. UMG itself neither documents nor distributes API keys for this surface.

**Human URL:** [https://7digital.gitbook.io/api-doc](https://7digital.gitbook.io/api-doc)

#### Tags:

 - Aggregator, Catalog, Partner API, Recorded Music

#### Properties

- [Documentation](https://7digital.gitbook.io/api-doc)
- [PartnerOf](https://www.7digital.com)

### UMG AI Licensing Program

UMG's "Artist Centric AI" framework governs licensed access to UMG's recordings and compositions by generative-AI music platforms. The program is operated as a series of bilateral commercial agreements, not as a self-serve developer program. As of 2025-2026, announced partners include Udio (licensed generative platform with catalog training and remixing rights), Splice (AI music tools for artists), SoundLabs, KLAY Vision, ProRata, BandLab Technologies (ethical AI framework), YouTube (AI Music Principles), TikTok, Meta, and KDDI. Liquidax Capital co-develops UMG's AI patent portfolio (15+ filings across musical collaboration, multimedia content, music & health, AI threat protection, and rights management). No public OpenAPI, no token issuance, no sandbox.

**Human URL:** [https://www.universalmusic.com](https://www.universalmusic.com)

#### Tags:

 - AI, Generative Music, Licensing, Partnerships, Rights Management

#### Properties

- [PartnerProgram](https://www.universalmusic.com/contact/)
- [PressRoom](https://www.universalmusic.com/news/)

### Universal-Music-Group GitHub Organization

Official UMG GitHub organization (login Universal-Music-Group, org id 169924279), created May 15, 2024. As of profiling, the org has 0 public repositories, 0 public gists, 0 followers, no bio, no blog, no email, and no published members. The organization exists as a brand placeholder; UMG's engineering output is not published openly. An unrelated GitHub login `umg` (with 51 repos) is gated behind UMG single-sign-on and is also not an open developer surface.

**Human URL:** [https://github.com/Universal-Music-Group](https://github.com/Universal-Music-Group)

#### Tags:

 - GitHub, Source Code

#### Properties

- [GitHubOrganization](https://github.com/Universal-Music-Group)
- [ProfileAPI](https://api.github.com/users/Universal-Music-Group)

## Common Properties

- [Website](https://www.universalmusic.com)
- [AboutUs](https://www.universalmusic.com/about/)
- [News](https://www.universalmusic.com/news/)
- [Labels](https://www.universalmusic.com/labels/)
- [Careers](https://www.universalmusic.com/careers/)
- [ContactUs](https://www.universalmusic.com/contact/)
- [InvestorRelations](https://www.universalmusic.com/investors/)
- [TermsOfService](https://www.universalmusic.com/terms/)
- [PrivacyPolicy](https://www.universalmusic.com/privacy-policy/)
- [LinkedIn](https://www.linkedin.com/company/universalmusicgroup)
- [GitHubOrganization](https://github.com/Universal-Music-Group)
- [GitHubRepository](https://github.com/api-evangelist/universal-music-group)
- [Stock](https://live.euronext.com/en/product/equities/NL0015000IY2-XAMS)

## Subsidiaries

| Name | Description |
|------|-------------|
| Universal Music Publishing Group | Global music publishing arm; songwriter signings, catalog administration, and sync licensing. |
| Bravado | Global merchandise and brand-management division for UMG's artist roster. |
| PolyGram Entertainment | Film, television, and documentary production division producing music-led content. |
| Universal Music Enterprises | Catalog-marketing division managing reissues, compilations, and legacy artist releases. |
| Mercury Studios | Music film, documentary, and video production label. |

## Label Families

| Name | Description |
|------|-------------|
| Republic Corps | Republic Records, Island Records, Def Jam Recordings. |
| Interscope Capitol Labels Group | Interscope Geffen A&M, Capitol Records, Blue Note Records, Motown, Capitol Christian Music Group, Priority Records. |
| Virgin Music Group | Virgin Records, mtheory, PIAS, Integral, Caroline, Fiction, Fontana; UMG's label-services / independent-distribution arm. |
| Verve Label Group | Verve Records, Decca Records, Deutsche Grammophon, Impulse!, Philips, Brunswick, GRP, Verve Forecast. |
| UMG Nashville | MCA Nashville, Mercury Nashville, EMI Records Nashville, Capitol Records Nashville. |
| Universal Music Latin Entertainment | Universal Music Latino, Disa, Fonovisa, Machete Music. |
| Universal Music UK | EMI Records UK, Polydor UK, Island UK, Decca UK, 0207 Def Jam, EMI North. |
| Abbey Road Studios | Historic London recording studios owned by UMG. |

## Features

| Name | Description |
|------|-------------|
| Recorded Music Catalog | Over 3 million recordings spanning UMG's label families, distributed to DSPs via private DDEX-based ingest pipelines. |
| Music Publishing Catalog | Over 4 million compositions administered by Universal Music Publishing Group across writer signings and acquired catalogs. |
| Merchandise (Bravado) | Direct-to-consumer artist merchandise storefronts and tour merch operated by the Bravado division. |
| Film and Television | Music-led films, documentaries, and series produced under PolyGram Entertainment and Mercury Studios. |
| Royalty Portals | Authenticated royalty-statement portals (UMG Royalty Portal for recordings, UMPG Window for publishing) for artists, labels, and songwriters. |
| Licensed AI Partnerships | Commercial AI-music licensing program covering Udio, Splice, SoundLabs, KLAY Vision, ProRata, BandLab, YouTube, TikTok, Meta, and KDDI. |
| AI Patent Portfolio | 15+ AI patents filed with Liquidax Capital spanning collaboration, multimedia content, music & health, AI threat protection, and rights management. |

## Use Cases

| Name | Description |
|------|-------------|
| Streaming Catalog Access | End-user and developer access to UMG's recorded-music catalog occurs through downstream DSPs (Spotify, Apple Music, YouTube Music, Amazon Music, Tidal), each of which publishes its own developer API. |
| Sync Licensing | Film, TV, advertising, and game producers license UMG recordings and UMPG compositions through bilateral business-affairs negotiation, not through a self-serve API. |
| Royalty Reporting | Artists, labels, and songwriters access royalty statements through the authenticated UMG Royalty Portal and UMPG Window apps. |
| AI Training and Generation Licensing | Licensed AI platforms (Udio, Splice, SoundLabs, etc.) access UMG content under bilateral commercial agreements that govern training, generation, and downstream remixing rights. |
| Merchandise Distribution | Direct-to-consumer fan commerce operated by Bravado on behalf of UMG's artist roster. |

## Integrations

| Name | Description |
|------|-------------|
| DDEX | Industry-standard messaging suite (ERN for release notification, RIN for recording information, MEAD for media-enrichment, DSR for sales reporting) used by UMG to deliver content to DSPs. |
| Spotify | Catalog delivered to Spotify via DDEX; developers query UMG catalog through Spotify Web API rather than any UMG-branded API. |
| Apple Music | Catalog delivered to Apple Music; downstream developer access via Apple Music API. |
| YouTube / YouTube Music | Catalog and AI Music Principles partnership covering UGC matching, music identification, and licensed AI-music experiments. |
| TikTok | Licensed music partnership covering catalog availability and AI-related provisions. |
| Meta | Licensed music agreements covering Facebook, Instagram, and emerging AI surfaces. |
| KDDI | Japan telecom partner; AI-related licensed-music agreement. |
| Udio | Licensed generative-AI music platform; UMG strategic partner under Artist Centric AI framework. |
| Splice | AI music-tools partner for UMG-roster artist tooling. |
| SoundLabs | Voice-model and AI-music partner. |
| KLAY Vision | AI-music platform partner. |
| ProRata | AI training / rights attribution partner. |
| BandLab Technologies | Partner on ethical-AI framework for songwriters and artists (Oct 2023 agreement). |
| Liquidax Capital | IP asset-management and advisory firm co-developing UMG's AI patent portfolio (15+ filings). |
| 7digital | Partner aggregator that exposes UMG catalog under a B2B API used in hackathons and embedded media partners. |
| Drupal | UMG runs Drupal-based corporate properties (organization listed at drupal.org/UMG). |

## Notable Absences

| Name | Description |
|------|-------------|
| No Public Developer Portal | No developer.universalmusic.com, no api.universalmusic.com, no api keys, no OAuth program, no sandbox, no rate-limit documentation. |
| No Public OpenAPI / AsyncAPI | UMG has never published an OpenAPI, AsyncAPI, JSON Schema, or Postman collection. Catalog and metadata exchange happens privately via DDEX over SFTP/vendor APIs. |
| No Public SDKs | No first-party language SDKs in any package registry (npm, PyPI, Maven, NuGet, RubyGems, crates.io, Go modules). |
| Empty Official GitHub Organization | github.com/Universal-Music-Group exists (created May 15 2024) with 0 public repositories, 0 gists, 0 followers, and no bio. |
| No Public Changelog / Status Page | No api.umg.com/status, no public status.universalmusic.com, no machine-readable changelog. |
| No Public Pricing | No published API pricing because no API exists. Licensing, royalty, and AI-partnership terms are negotiated privately under NDA. |
| No Public RSS / Atom | Corporate news is published as HTML pages on universalmusic.com without a published RSS feed in standard well-known locations. |
| No Webhooks | No publicly documented webhook program for any UMG surface (royalty events, release notifications, content drops). |

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
