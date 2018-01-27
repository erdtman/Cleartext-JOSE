## BOF Session Request

- Name: JSON Clear Text Signature and Encryption (JOSE-CT)
- Description:
The goal of this group is to standardize signature and encryption schemes combining the existing JWS and JWE standards with ECMA's JSON processing rules for EcmaScript (JavaScript).   By doing that, header data (like public keys and algorithms) as well as signed JSON data can be provided in clear text.

The need for this work stems from: 
- JSON have effectively replaced XML for most new systems. Unlike XML signatures which requires quite complex (and thus error-prone) canonicalization, this proposal's reliance on EcmaScript JSON processing rules makes it straightforward offering similar functionality for JSON.

- The primary target for the enhanced JWS and JWE schemes are information centric systems where the clear text approach simplifies documentation and debugging.

- There are IETF standards in the workings which embed signed messages in an outer JSON object holding a "type indicator" for the embedded object.  Other standards efforts are using an HTTP header featuring a detached JWS signature + an HTTP body holding JSON data in clear.  Using this proposal such workarounds wouldn't be necessary.

- The connection to EcmaScript enables you to also sign JavaScript objects which for example can be used in Web pages.

Agenda
- TBD
Discussion - 1h
Status: WG Forming
