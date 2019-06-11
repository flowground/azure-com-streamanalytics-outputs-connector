# ![LOGO](logo.png) StreamAnalyticsManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the StreamAnalyticsManagementClient API (version 2016-03-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/streamanalytics-outputs/2016-03-01/swagger.json<br/>
Generated at: 2019-06-11T18:14:32+03:00

## API Description



## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists all of the outputs under the specified streaming job.

*Tags:* `Outputs`

#### Input Parameters
* `$select` - _optional_ - The $select OData query parameter. This is a comma-separated list of structural properties to include in the response, or "*" to include all properties. By default, all properties are returned except diagnostics. Currently only accepts '*' as a valid value.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.

### Deletes an output from the streaming job.

*Tags:* `Outputs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.
* `outputName` - _required_ - The name of the output.

### Gets details about the specified output.

*Tags:* `Outputs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.
* `outputName` - _required_ - The name of the output.

### Updates an existing output under an existing streaming job. This can be used to partially update (ie. update one or two properties) an output without affecting the rest the job or output definition.

*Tags:* `Outputs`

#### Input Parameters
* `If-Match` - _optional_ - The ETag of the output. Omit this value to always overwrite the current output. Specify the last-seen ETag value to prevent accidentally overwriting concurrent changes.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.
* `outputName` - _required_ - The name of the output.

### Creates an output or replaces an already existing output under an existing streaming job.

*Tags:* `Outputs`

#### Input Parameters
* `If-Match` - _optional_ - The ETag of the output. Omit this value to always overwrite the current output. Specify the last-seen ETag value to prevent accidentally overwriting concurrent changes.
* `If-None-Match` - _optional_ - Set to '*' to allow a new output to be created, but to prevent updating an existing output. Other values will result in a 412 Pre-condition Failed response.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.
* `outputName` - _required_ - The name of the output.

### Tests whether an output's datasource is reachable and usable by the Azure Stream Analytics service.

*Tags:* `Outputs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.
* `outputName` - _required_ - The name of the output.

## License

**flow**ground :- Telekom iPaaS / azure-com-streamanalytics-outputs-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
