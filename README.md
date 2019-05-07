# ![LOGO](logo.png) ADHybridHealthService **flow**ground Connector

## Description

A generated **flow**ground connector for the ADHybridHealthService API (version 2014-01-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/adhybridhealthservice-ADHybridHealthService/2014-01-01/swagger.json<br/>
Generated at: 2019-05-07T17:37:05+03:00

## API Description

REST APIs for Azure Active Directory Connect Health

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Gets the details of Active Directory Domain Service, for a tenant, that are onboarded to Azure Active Directory Connect Health.

*Tags:* `Adds`

#### Input Parameters
* `$filter` - _optional_ - The service property filter to apply.
* `serviceType` - _optional_ - The service type for the services onboarded to Azure Active Directory Connect Health. Depending on whether the service is monitoring, ADFS, Sync or ADDS roles, the service type can either be AdFederationService or AadSyncService or AdDomainService.
* `skipCount` - _optional_ - The skip count, which specifies the number of elements that can be bypassed from a sequence and then return the remaining elements.
* `takeCount` - _optional_ - The take count , which specifies the number of elements that can be returned from a sequence.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Onboards a service for a given tenant in Azure Active Directory Connect Health.

*Tags:* `Adds`

#### Input Parameters
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of Active Directory Domain Services for a tenant having Azure AD Premium license and is onboarded to Azure Active Directory Connect Health.

*Tags:* `Services`

#### Input Parameters
* `$filter` - _optional_ - The service property filter to apply.
* `serviceType` - _optional_ - The service type for the services onboarded to Azure Active Directory Connect Health. Depending on whether the service is monitoring, ADFS, Sync or ADDS roles, the service type can either be AdFederationService or AadSyncService or AdDomainService.
* `skipCount` - _optional_ - The skip count, which specifies the number of elements that can be bypassed from a sequence and then return the remaining elements.
* `takeCount` - _optional_ - The take count , which specifies the number of elements that can be returned from a sequence.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Deletes an Active Directory Domain Service which is onboarded to Azure Active Directory Connect Health.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service which needs to be deleted.
* `confirm` - _optional_ - Indicates if the service will be permanently deleted or disabled. True indicates that the service will be permanently deleted and False indicates that the service will be marked disabled and then deleted after 30 days, if it is not re-registered.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of an Active Directory Domain Service for a tenant having Azure AD Premium license and is onboarded to Azure Active Directory Connect Health.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Updates an Active Directory Domain Service properties of an onboarded service.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service which needs to be deleted.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of the servers, for a given Active Directory Domain Service, that are onboarded to Azure Active Directory Connect Health.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The server property filter to apply.
* `isGroupbySite` - _required_ - Indicates if the result should be grouped by site or not.
* `query` - _optional_ - The custom query.
* `nextPartitionKey` - _required_ - The next partition key to query for.
    Possible values:  .
* `nextRowKey` - _required_ - The next row key to query for.
    Possible values:  .
* `takeCount` - _optional_ - The take count , which specifies the number of elements that can be returned from a sequence.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of the Active Directory Domain servers, for a given Active Directory Domain Service, that are onboarded to Azure Active Directory Connect Health.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The server property filter to apply.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the alerts for a given Active Directory Domain Service.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The alert property filter to apply.
* `state` - _optional_ - The alert state to query for.
* `from` - _optional_ - The start date to query for.
* `to` - _optional_ - The end date till when to query for.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the service configurations.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `grouping` - _optional_ - The grouping for configurations.

### Gets the dimensions for a given dimension type in a server.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `dimension` - _required_ - The dimension type.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Deletes the user preferences for a given feature.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `featureName` - _required_ - The name of the feature.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the user preferences for a given feature.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `featureName` - _required_ - The name of the feature.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Adds the user preferences for a given feature.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `featureName` - _required_ - The name of the feature.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the forest summary for a given Active Directory Domain Service, that is onboarded to Azure Active Directory Connect Health.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the service related metrics information.

*Tags:* `Adds`

#### Input Parameters
* `$filter` - _optional_ - The metric metadata property filter to apply.
* `serviceName` - _required_ - The name of the service.
* `perfCounter` - _optional_ - Indicates if only performance counter metrics are requested.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the service related metric information.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `metricName` - _required_ - The metric name
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the service related metrics for a given metric and group combination.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `metricName` - _required_ - The metric name
* `groupName` - _required_ - The group name
* `groupKey` - _optional_ - The group key
* `fromDate` - _optional_ - The start date.
* `toDate` - _optional_ - The end date.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the server related metrics for a given metric and group combination.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `metricName` - _required_ - The metric name
* `groupName` - _required_ - The group name
* `groupKey` - _optional_ - The group key
* `fromDate` - _optional_ - The start date.
* `toDate` - _optional_ - The end date.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the average of the metric values for a given metric and group combination.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `metricName` - _required_ - The metric name
* `groupName` - _required_ - The group name
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the sum of the metric values for a given metric and group combination.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `metricName` - _required_ - The metric name
* `groupName` - _required_ - The group name
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets complete domain controller list along with replication details for a given Active Directory Domain Service, that is onboarded to Azure Active Directory Connect Health.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The server property filter to apply.
* `withDetails` - _optional_ - Indicates if InboundReplicationNeighbor details are required or not.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets Replication status for a given Active Directory Domain Service, that is onboarded to Azure Active Directory Connect Health.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets complete domain controller list along with replication details for a given Active Directory Domain Service, that is onboarded to Azure Active Directory Connect Health.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The server property filter to apply.
* `isGroupbySite` - _required_ - Indicates if the result should be grouped by site or not.
* `query` - _required_ - The custom query.
* `nextPartitionKey` - _required_ - The next partition key to query for.
    Possible values:  .
* `nextRowKey` - _required_ - The next row key to query for.
    Possible values:  .
* `takeCount` - _optional_ - The take count , which specifies the number of elements that can be returned from a sequence.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of the servers, for a given Active Directory Domain Controller service, that are onboarded to Azure Active Directory Connect Health Service.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The server property filter to apply.
* `dimensionType` - _optional_ - The server specific dimension.
* `dimensionSignature` - _optional_ - The value of the dimension.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Onboards  a server, for a given Active Directory Domain Controller service, to Azure Active Directory Connect Health Service.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service under which the server is to be onboarded.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Deletes a Active Directory Domain Controller server that has been onboarded to Azure Active Directory Connect Health Service.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `serviceMemberId` - _required_ - The server Id.
* `confirm` - _optional_ - Indicates if the server will be permanently deleted or disabled. True indicates that the server will be permanently deleted and False indicates that the server will be marked disabled and then deleted after 30 days, if it is not re-registered.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of a server, for a given Active Directory Domain Controller service, that are onboarded to Azure Active Directory Connect Health Service.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `serviceMemberId` - _required_ - The server Id.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of an alert for a given Active Directory Domain Controller service and server combination.

*Tags:* `Adds`

#### Input Parameters
* `serviceMemberId` - _required_ - The server Id for which the alert details needs to be queried.
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The alert property filter to apply.
* `state` - _optional_ - The alert state to query for.
* `from` - _optional_ - The start date to query for.
* `to` - _optional_ - The end date till when to query for.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the credentials of the server which is needed by the agent to connect to Azure Active Directory Connect Health Service.

*Tags:* `Adds`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The property filter to apply.
* `serviceMemberId` - _required_ - The server Id.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of a tenant onboarded to Azure Active Directory Connect Health.

*Tags:* `Configuration`

#### Input Parameters
* `api-version` - _required_ - The version of the API to be used with the client request.

### Updates tenant properties for tenants onboarded to Azure Active Directory Connect Health.

*Tags:* `Configuration`

#### Input Parameters
* `api-version` - _required_ - The version of the API to be used with the client request.

### Onboards a tenant in Azure Active Directory Connect Health.

*Tags:* `Configuration`

#### Input Parameters
* `api-version` - _required_ - The version of the API to be used with the client request.

### Lists the available Azure Data Factory API operations.

*Tags:* `operations`

#### Input Parameters
* `api-version` - _required_ - The version of the API to be used with the client request.

### Checks if the user is enabled for Dev Ops access.

*Tags:* `DevOps`

#### Input Parameters
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the connector details for a service.

*Tags:* `ServiceMembers`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `serviceMemberId` - _required_ - The server Id.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of services, for a tenant, that are onboarded to Azure Active Directory Connect Health.

*Tags:* `Services`

#### Input Parameters
* `$filter` - _optional_ - The service property filter to apply.
* `serviceType` - _optional_ - The service type for the services onboarded to Azure Active Directory Connect Health. Depending on whether the service is monitoring, ADFS, Sync or ADDS roles, the service type can either be AdFederationService or AadSyncService or AdDomainService.
* `skipCount` - _optional_ - The skip count, which specifies the number of elements that can be bypassed from a sequence and then return the remaining elements.
* `takeCount` - _optional_ - The take count , which specifies the number of elements that can be returned from a sequence.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Onboards a service for a given tenant in Azure Active Directory Connect Health.

*Tags:* `Services`

#### Input Parameters
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of services for a tenant having Azure AD Premium license and is onboarded to Azure Active Directory Connect Health.

*Tags:* `Services`

#### Input Parameters
* `$filter` - _optional_ - The service property filter to apply.
* `serviceType` - _optional_ - The service type for the services onboarded to Azure Active Directory Connect Health. Depending on whether the service is monitoring, ADFS, Sync or ADDS roles, the service type can either be AdFederationService or AadSyncService or AdDomainService.
* `skipCount` - _optional_ - The skip count, which specifies the number of elements that can be bypassed from a sequence and then return the remaining elements.
* `takeCount` - _optional_ - The take count , which specifies the number of elements that can be returned from a sequence.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Deletes a service which is onboarded to Azure Active Directory Connect Health.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service which needs to be deleted.
* `confirm` - _optional_ - Indicates if the service will be permanently deleted or disabled. True indicates that the service will be permanently deleted and False indicates that the service will be marked disabled and then deleted after 30 days, if it is not re-registered.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of a service for a tenant having Azure AD Premium license and is onboarded to Azure Active Directory Connect Health.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Updates the service properties of an onboarded service.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service which needs to be deleted.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Checks if the tenant, to which a service is registered, is whitelisted to use a feature.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `featureName` - _required_ - The name of the feature.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the alerts for a given service.

*Tags:* `Alerts`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The alert property filter to apply.
* `state` - _optional_ - The alert state to query for.
* `from` - _optional_ - The start date to query for.
* `to` - _optional_ - The end date till when to query for.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Checks if the service has all the pre-requisites met to use a feature.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `featureName` - _required_ - The name of the feature.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the count of latest AAD export errors.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the categorized export errors.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `errorBucket` - _required_ - The error category to query for.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the export status.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Adds an alert feedback submitted by customer.

*Tags:* `Feedback`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets a list of all alert feedback for a given tenant and alert type.

*Tags:* `Feedback`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `shortName` - _required_ - The name of the alert.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the service related metrics information.

*Tags:* `Metrics`

#### Input Parameters
* `$filter` - _optional_ - The metric metadata property filter to apply.
* `serviceName` - _required_ - The name of the service.
* `perfCounter` - _optional_ - Indicates if only performance counter metrics are requested.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the service related metrics information.

*Tags:* `Metrics`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `metricName` - _required_ - The metric name
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the service related metrics for a given metric and group combination.

*Tags:* `Metrics`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `metricName` - _required_ - The metric name
* `groupName` - _required_ - The group name
* `groupKey` - _optional_ - The group key
* `fromDate` - _optional_ - The start date.
* `toDate` - _optional_ - The end date.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the server related metrics for a given metric and group combination.

*Tags:* `Metrics`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `metricName` - _required_ - The metric name
* `groupName` - _required_ - The group name
* `groupKey` - _optional_ - The group key
* `fromDate` - _optional_ - The start date.
* `toDate` - _optional_ - The end date.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the average of the metric values for a given metric and group combination.

*Tags:* `Metrics`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `metricName` - _required_ - The metric name
* `groupName` - _required_ - The group name
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the sum of the metric values for a given metric and group combination.

*Tags:* `Metrics`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `metricName` - _required_ - The metric name
* `groupName` - _required_ - The group name
* `api-version` - _required_ - The version of the API to be used with the client request.

### Updates the service level monitoring configuration.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the service level monitoring configurations.

*Tags:* `Services`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the bad password login attempt report for an user

*Tags:* `Reports`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `dataSource` - _optional_ - The source of data, if its test data or customer data.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets all Risky IP report URIs for the last 7 days.

*Tags:* `Reports`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Initiate the generation of a new Risky IP report. Returns the URI for the new one.

*Tags:* `Reports`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of the servers, for a given service, that are onboarded to Azure Active Directory Connect Health Service.

*Tags:* `ServiceMembers`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The server property filter to apply.
* `dimensionType` - _optional_ - The server specific dimension.
* `dimensionSignature` - _optional_ - The value of the dimension.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Onboards  a server, for a given service, to Azure Active Directory Connect Health Service.

*Tags:* `ServiceMembers`

#### Input Parameters
* `serviceName` - _required_ - The name of the service under which the server is to be onboarded.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Deletes a server that has been onboarded to Azure Active Directory Connect Health Service.

*Tags:* `ServiceMembers`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `serviceMemberId` - _required_ - The server Id.
* `confirm` - _optional_ - Indicates if the server will be permanently deleted or disabled. True indicates that the server will be permanently deleted and False indicates that the server will be marked disabled and then deleted after 30 days, if it is not re-registered.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of a server, for a given service, that are onboarded to Azure Active Directory Connect Health Service.

*Tags:* `ServiceMembers`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `serviceMemberId` - _required_ - The server Id.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the details of an alert for a given service and server combination.

*Tags:* `Alerts`

#### Input Parameters
* `serviceMemberId` - _required_ - The server Id for which the alert details needs to be queried.
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The alert property filter to apply.
* `state` - _optional_ - The alert state to query for.
* `from` - _optional_ - The start date to query for.
* `to` - _optional_ - The end date till when to query for.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the credentials of the server which is needed by the agent to connect to Azure Active Directory Connect Health Service.

*Tags:* `ServiceMembers`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `$filter` - _optional_ - The property filter to apply.
* `serviceMemberId` - _required_ - The server Id.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Deletes the data uploaded by the server to Azure Active Directory Connect Health Service.

*Tags:* `ServiceMembers`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `serviceMemberId` - _required_ - The server Id.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the last time when the server uploaded data to Azure Active Directory Connect Health Service.

*Tags:* `ServiceMembers`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `serviceMemberId` - _required_ - The server Id.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the export status.

*Tags:* `ServiceMembers`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `serviceMemberId` - _required_ - The server Id.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the global configuration.

*Tags:* `ServiceMembers`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `serviceMemberId` - _required_ - The server id.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the server related metrics for a given metric and group combination.

*Tags:* `Metrics`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `metricName` - _required_ - The metric name
* `groupName` - _required_ - The group name
* `serviceMemberId` - _required_ - The server id.
* `groupKey` - _optional_ - The group key
* `fromDate` - _optional_ - The start date.
* `toDate` - _optional_ - The end date.
* `api-version` - _required_ - The version of the API to be used with the client request.

### Gets the service configuration.

*Tags:* `ServiceMembers`

#### Input Parameters
* `serviceName` - _required_ - The name of the service.
* `serviceMemberId` - _required_ - The server Id.
* `api-version` - _required_ - The version of the API to be used with the client request.

## License

**flow**ground :- Telekom iPaaS / azure-com-adhybridhealthservice-ad-hybrid-health-service-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
