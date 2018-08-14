
# Correlation Vector

## Background

**Correlation Vector** (a.k.a. **cV**) is a format and protocol standard for tracing and correlation of events through a distributed system based on a light weight vector clock.
The standard is widely used internally at Microsoft for first party applications and services and supported across multiple logging libraries and platforms (Services, Clients - Native, Managed, Js, iOS, Android etc). The standard powers a variety of different data processing needs ranging from distributed tracing & debugging to system and business intelligence, in various business organizations.
For more on correlation vector, read [future](https://github.com/Microsoft/CorrelationVector) roadmap and [scenarios](https://github.com/Microsoft/CorrelationVector/blob/master/Scenarios.md).

This repo provides reference implementation for Java developers to take full advantage of cV in end-to-end distributed tracing scenarios.

# Format

Format: id0[.id1. … .idN], where

* id0 is a 12 byte randomly generated number that is encoded as a base64 string on the wire. id0 is also referred to as the base value.
* id1. … .idN are 32 bit unsigned integers

Example: XXI1uDYrTQe7asf7O/0FnU.1.2

# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.


# General feedback and discussions?
Please start a discussion on the [Home repo issue tracker](https://github.com/Microsoft/CorrelationVector-Java/issues)
