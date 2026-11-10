# Contributing

This project welcomes contributions and suggestions. Most contributions require
you to agree to a Contributor License Agreement (CLA) declaring that you have
the right to, and actually do, grant us the rights to use your contribution.
For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether
you need to provide a CLA and decorate the PR appropriately. Simply follow the
instructions provided by the bot. You will only need to do this once across all
repositories using our CLA.

## Making changes

Open an issue for significant design changes before starting. Keep pull requests
focused, preserve upstream licenses and attribution, and update the documentation
when behavior changes. Never include credentials, deployment outputs, customer
data, or real environment identifiers in issues, pull requests, or committed files.
Use placeholders and synthetic data.

Run the [local validation commands](docs/deployment.md#verification) before
submitting a pull request. After changing Bicep, run
`.\scripts\Build-PortalTemplate.ps1` and commit the regenerated `azuredeploy.json`.
CI uses Bicep v0.44.1 to keep that generated template reproducible; use the same
version when regenerating it. Infrastructure changes should also be validated
in a dedicated Azure subscription as appropriate; local tests and CI do not
deploy resources or establish regional capacity.

## Code of conduct

This project has adopted the
[Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information, see the
[Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/)
or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any
additional questions or comments.
