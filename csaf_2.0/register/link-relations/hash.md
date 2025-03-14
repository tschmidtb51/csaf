I suggest to submit for the registration of the "hash" link type the following to the relevant GitHub hosted repository [https://github.com/protocol-registries/link-relations/issues](https://github.com/protocol-registries/link-relations/issues) as issue: 

Please confirm that:

* [x]  You have read and understood the [requirements for registration](https://tools.ietf.org/html/rfc8288#section-2.1.1).
* [x]  You have checked [the registry](https://www.iana.org/assignments/link-relations/) and found no current link relation types that meet your needs.
* [x]  Your specification reference URL is stable; ideally, managed by a widely-recognised standards development organisation (e.g., published as an RFC). Otherwise, please give additional information.

If so, please enter the details of the link relation type below:

* Relation Name: hash
* Description: Refers to a resource that contains the context's hash value. The resource content SHALL start with the first byte of the hexadecimal hash value. Any subsequent data (like a filename) which is optional SHALL be separated by at least one space.
* Reference: https://docs.oasis-open.org/csaf/csaf/v2.0/os/csaf-v2.0-os.html#7115-requirement-15-rolie-feed

Any additional information (this will not be included in the registry)? 
The OASIS Common Security Advisories Framework (CSAF) Technical Committee (TC) has been chartered to standardize the implementation and exchange of security advisories. The automatic and fast discovery of relevant as well as actionable security advisories is an important step in the process of effectively mitigating and ultimately removing vulnerabilities as they become apparent. We are requesting the registration of a "hash" link type that would contain parameters and configuration requirements to allow this level of automated discovery.
Resource-Oriented Lightweight Information Exchange (ROLIE) is a standard to ease discovery of security content. ROLIE is built on top of the Atom Publishing Format and Protocol, with specific requirements that support publishing security content. Each ROLIE feed document MUST be a JSON file that conforms with [RFC8322]. Any existing hash file (requirement 18) MUST be listed in the corresponding entry of the ROLIE feed as an item of the array `link` having the `rel` value of `hash`.

For further reference, the CSAF version 2.0 OASIS Standard is always available at:
[https://docs.oasis-open.org/csaf/csaf/v2.0/csaf-v2.0.html](https://docs.oasis-open.org/csaf/csaf/v2.0/csaf-v2.0.html)  
