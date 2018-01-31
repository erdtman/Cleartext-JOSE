## BOF Session Request

- Name: Cleartext JSON Object Signing and Encryption (JOSE)
- Description:
The goal of this group is to standardize signature and encryption schemes combining the existing JWS and JWE standards with ECMA's JSON processing rules for EcmaScript (JavaScript).   By doing that, header parameter data (like public keys and algorithms) and signed JSON data can be provided in clear text.<br>&nbsp;<br>Since the required EcmaScript support is already available in Internet browsers and node.js, implementations of the proposed representations not have to start from zero.  JSON tools written in other languages, however, may require additional work.

The need for this work stems from: 
- JSON has effectively replaced XML for most new systems. Unlike XML signatures, which require quite complex (and thus error-prone) canonicalization, this proposal's reliance on EcmaScript JSON processing rules makes it straightforward, offering simpler canonicalization functionality for JSON.

- The primary target for the cleartext JWS and JWE specifications are information centric systems, where the cleartext approach can simplify documentation and debugging.

- There is an IETF standard in the works that embeds signed Base64Url-encoded messages in an outer JSON object holding a cleartext "type indicator" for the embedded object [OTrP].  Other standards efforts in progress combine an HTTP header featuring a detached signature with an HTTP body holding JSON data in clear [OPENBANKING].  Using cleartext JOSE, such workarounds would no longer be necessary.

- The close tie with EcmaScript also enables support for signing JavaScript objects, which for example, can be used in Web pages.

Agenda
- TBD
- Discussion
- Status: Should the JOSE working group be reformed and the jose@ietf.org mailing list kept so existing expertise can be brought to bear?

References
- [OTrP] https://tools.ietf.org/html/draft-pei-opentrustprotocol-05#section-8.2.1.1
- [OPENBANKING] https://openbanking.atlassian.net/wiki/spaces/DZ/pages/5786479/Payment+Initiation+API+Specification+-+v1.1.0
