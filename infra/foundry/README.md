# Microsoft Foundry infrastructure modules

This directory contains the reachable Bicep modules from Microsoft's
[Foundry infrastructure samples](https://github.com/microsoft-foundry/foundry-samples).
The source revision is recorded in `..\sources.json`; the original MIT license
is preserved in `LICENSE`.

Use `..\main.bicep` as this repository's entrypoint. Unused additional-project
templates, example parameter files, generated JSON, and helper scripts are not
part of the supported deployment.

Local adaptations preserve existing subnets/NAT, allow a separate Search region,
disable public Monitor ingestion/query, and attach the shared Blob DNS zone to
the Monitor private endpoint.
