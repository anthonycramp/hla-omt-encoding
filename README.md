# HLA OMT Encoding

The High Level Architecture requires data that can be communicated between federates in a federation be documented per the Object Model Template (OMT) specification. This specification is captured in an XML document and used, in part, by the RTI to configure how data is transported betweeen federates (e.g., reliable vs best effort, time stamped vs receive ordered, interest management, ...).

However, before a federate is sent via the services defined in the HLA Interface Specification and provided by an RTI, it must first be encoded per the encoding definitions defined in the OMT specification AND/OR by custom encoding definitions defined for this federation. Which encoding to use for particular data structures/types is defined in the HLA OMT XML document.

This repository has been created to do a couple of things:

1. Write code, in multiple programming langauges, that implements the standard encoding definitions.
2. Compare the standard encoding definitions with other wire definitions such as Protocul Buffers, BSON, Avro, and Thrift.
3. Compare the IDLs (or equivalents) of these other wire defintions with the OMT
