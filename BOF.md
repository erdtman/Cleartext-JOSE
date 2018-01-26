## BOF Session Request

- Name: JSON Clear Text Signature and Encryption (JOSE-CT)
- Description:
The goal of this group is to standardize signature and encryption schemes combining the existing JWS and JWE standards with ECMA's JSON processing rules for EcmaScript (JavaScript).   By doing that, header data (like public keys and algorithms) as well as signed JSON data can be provided in clear text.

The need for this work stems from: 
- JSON have effectively replaced XML for most new systems. Unlike XML signatures which requires quite complex (and thus error-prone) canonicalization, this proposal's reliance on EcmaScript JSON processing rules makes it straightforward offering similar (albeit somewhat simplified) functionality for JSON.

- The primary target for the enhanced JWS and JWE schemes are information centric systems where the clear text approach simplifies documentation and debugging.

- The connection to EcmaScript enables you to also sign JavaScript objects which for example can be used in Web pages.

Agenda
- TBD
Discussion - 1h
Status: WG Forming
Responsible AD: Suresh Krishnan
BoF proponents: Mike Jones (​satish.k@nokia.com), Roland Schott (​roland.schott@telekom.de), Samita Chakrabarti (​samitac.ietf@gmail.com), Sunghoon Seo (​sh.seo@kt.com), Tom Herbert (​tom@herbertland.com), Julius Mueller (​jm169k@att.com).
BoF chairs: Dirk von Hugo, Behcet Sarikaya (proposed)
Number of people expected to attend: 100
Length of session (1, 1.5, 2, or 2.5 hours): 1.5-2 hours
Conflicts to avoid (whole Areas and/or WGs): 6lo, DMM, 6MAN, DHC
Links to the mailing list, draft charter if any, relevant Internet-Drafts,
Mailing List: ​https://www.ietf.org/mailman/listinfo/5gangip
Draft charter: ​https://mailarchive.ietf.org/arch/msg/5gip/xxx
Relevant drafts:
Problem statements:
​https://tools.ietf.org/html/draft-xyx-5gip-ps-00
Architecture:
​https://tools.ietf.org/html/draft-kanugovi-intarea-mams-protocol-04
Issues:
​https://tools.ietf.org/html/draft-vonhugo-5gangip-ip-issues-03
Solution space
​https://tools.ietf.org/html/draft-herbert-nvo3-ila-04
​https://tools.ietf.org/html/draft-mueller-ila-mobility-03
​https://tools.ietf.org/html/draft-zhu-intarea-mams-control-protocol-01
​https://tools.ietf.org/html/draft-zhu-intarea-mams-user-protocol-01
Proposed Charter Text and Milestones (TBA)
Please list any protocols or practices that already exist in this space.
If any modifications to existing protocols or practices are required, please list them.
If any entirely new protocols or practices are required, please list them.
(Optional) Please list any open source projects implementing this work.
