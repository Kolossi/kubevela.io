---
title:  Gcp-Config
---

## Description

Terraform module for integrating Google Cloud Platform Organziations and Projects with Lacework for cloud resource configuration assessment

## Specification


### Properties

 Name | Description | Type | Required | Default 
 ------------ | ------------- | ------------- | ------------- | ------------- 
 service_account_private_key | The private key in JSON format, base64 encoded (required when use_existing_service_account is set to true) | string | false |  
 prefix | The prefix that will be use at the beginning of every generated resource | string | false |  
 org_integration | If set to true, configure an organization level integration | bool | false |  
 project_id | A project ID different from the default defined inside the provider | string | false |  
 service_account_name | The Service Account name (required when use_existing_service_account is set to true). This can also be used to specify the new service account name when use_existing_service_account is set to false | string | false |  
 required_config_apis |  | map | false |  
 wait_time | Amount of time to wait before the next resource is provisioned | string | false |  
 organization_id | The organization ID, required if org_integration is set to true | string | false |  
 use_existing_service_account | Set this to true to use an existing Service Account | bool | false |  
 lacework_integration_name |  | string | false |  
 writeConnectionSecretToRef | The secret which the cloud resource connection will be written to | [writeConnectionSecretToRef](#writeConnectionSecretToRef) | false |  


#### writeConnectionSecretToRef

 Name | Description | Type | Required | Default 
 ------------ | ------------- | ------------- | ------------- | ------------- 
 name | The secret name which the cloud resource connection will be written to | string | true |  
 namespace | The secret namespace which the cloud resource connection will be written to | string | false |  