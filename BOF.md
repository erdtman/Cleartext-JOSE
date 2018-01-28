## BOF Session Request

- Name: JSON Clear Text Signature and Encryption (JOSE-CT)
- Description:
The goal of this group is to standardize signature and encryption schemes combining the existing JWS and JWE standards with ECMA's JSON processing rules for EcmaScript (JavaScript).   By doing that, header data (like public keys and algorithms) as well as signed JSON data can be provided in clear text.<br>&nbsp;<br>
Since core support is already available (through EcmaScript's JSON object), in Internet browsers and Node.js, the proposed schemes will implementation-wise not have to start from zero.  JSON tools written in other languages will though usually require an upgrade.

The need for this work stems from: 
- JSON have effectively replaced XML for most new systems. Unlike XML signatures which requires quite complex (and thus error-prone) canonicalization, this proposal's reliance on EcmaScript JSON processing rules makes it straightforward offering similar functionality for JSON.

- The primary target for the enhanced JWS and JWE schemes are information centric systems where the clear text approach simplifies documentation and debugging.

- There is an IETF standard in the workings which embeds signed Base64Url-encoded messages in an outer JSON object holding a clear text "type indicator" for the embedded object.  Other standards efforts in progress combine an HTTP header featuring a detached signature with an HTTP body holding JSON data in clear.  Using this proposal such workarounds would no longer be necessary.

- The close tie with EcmaScript enables support for signing JavaScript objects which for example can be used in Web pages.

Agenda
- TBD
Discussion - 1h
Status: WG Forming
