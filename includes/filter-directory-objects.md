---
ms.localizationpriority: medium
ms.openlocfilehash: 95e6218d0f21d81491652a0229d3272a6a61d243
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562772"
---
### <a name="application-properties"></a>应用程序属性

| 名称                          | eq                                         | startsWith                                 | ge                                         | le                                         | Null 值                                 |
| --------------------------------------------- | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ |
| appId                                         | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| applicationTemplateId                         | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| createdDateTime                               | ![默认支持][RDS]               |                                            | ![默认支持][RDS]               | ![默认支持][RDS]               | ![需要高级查询参数。][AQP] |
| createdOnBehalfOf/deletedDateTime             | ![默认支持][RDS]               |                                            | ![默认支持][RDS]               | ![默认支持][RDS]               | ![不支持][NS]                       |
| 说明                                   | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![不支持][NS]                       |
| disabledByMicrosoftStatus                     | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| displayName                                   | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| info/logoUrl                                  | ![不支持][NS]                       | ![不支持][NS]                       |                                            |                                            | ![需要高级查询参数。][AQP] |
| info/termsOfServiceUrl                        | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |                                            |                                            | ![不支持][NS]                       |
| keyCredentials/any(k:k/endDateTime)           | ![需要高级查询参数。][AQP] |                                            | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |
| publisherDomain                               | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![不支持][NS]                       |
| requiredResourceAccess/any(r:r/resourceAppId) | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![不支持][NS]                       |
| signInAudience                                | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |


### <a name="service-principal-properties"></a>服务主体属性

| 属性           | eq                                         | startsWith                                 | ge                                         | le                                         | Null 值                                 |
| ----------------------------------- | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ |
| accountEnabled                      | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| appId                               | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| applicationTemplateId               | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| appOwnerOrganizationId              | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![不支持][NS]                       |
| appRoleAssignmentRequired           | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![不支持][NS]                       |
| createdObjects/any(c:c/id)          | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![不支持][NS]                       |
| 说明                         | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![不支持][NS]                       |
| displayName                         | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| info/logoUrl                        | ![不支持][NS]                       | ![不支持][NS]                       |                                            |                                            | ![需要高级查询参数。][AQP] |
| info/termsOfServiceUrl              | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |                                            |                                            | ![不支持][NS]                       |
| keyCredentials/any(k:k/endDateTime) | ![需要高级查询参数。][AQP] |                                            | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |



### <a name="device-properties"></a>设备属性

| 属性                                  | eq                                         | startsWith                   | ge                                         | le                                         | Null 值                                 |
| ------------------------------------------------ | ------------------------------------------ | ---------------------------- | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ |
| accountEnabled                                   | ![默认支持][RDS]               |                              |                                            |                                            | ![不支持][NS]                       |
| alternativeSecurityIds/any(a:a/identityProvider) | ![需要高级查询参数。][AQP] | ![不支持][NS]         |                                            |                                            | ![不支持][NS]                       |
| alternativeSecurityIds/any(a:a/type)             | ![默认支持][RDS]               |                              | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |
| approximateLastSignInDateTime                    | ![默认支持][RDS]               |                              | ![默认支持][RDS]               | ![默认支持][RDS]               | ![需要高级查询参数。][AQP] |
| deviceId                                         | ![默认支持][RDS]               |                              |                                            |                                            | ![不支持][NS]                       |
| extensionAttributes/extensionAttribute1-15 | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP]         |                                            |                                            | ![需要高级查询参数。][AQP]                       |
| displayName                                      | ![默认支持][RDS]               | ![默认支持][RDS] |                                            |                                            | ![需要高级查询参数。][AQP] |
| isCompliant                                      | ![默认支持][RDS]               |                              |                                            |                                            | ![不支持][NS]                       |
| isManaged                                        | ![默认支持][RDS]               |                              |                                            |                                            | ![不支持][NS]                       |
| mdmAppId                                         | ![默认支持][RDS]               |                              |                                            |                                            | ![不支持][NS]                       |
| onPremisesLastSyncDateTime                       | ![默认支持][RDS]               |                              | ![默认支持][RDS]               | ![默认支持][RDS]               | ![不支持][NS]                       |
| onPremisesSyncEnabled                            | ![默认支持][RDS]               |                              |                                            |                                            | ![需要高级查询参数。][AQP] |
| operatingSystem                                  | ![默认支持][RDS]               | ![默认支持][RDS] |                                            |                                            | ![需要高级查询参数。][AQP] |
| operatingSystemVersion                           | ![默认支持][RDS]               | ![默认支持][RDS] |                                            |                                            | ![需要高级查询参数。][AQP] |



### <a name="group-properties"></a>组属性

| 属性                                                   | eq                                         | startsWith                                 | ge                                         | le                                         | Null 值                                 |
|------------------------------------------------------------|--------------------------------------------|--------------------------------------------|--------------------------------------------|--------------------------------------------|--------------------------------------------|
| assignedLicenses/any(a:a/skuId)                            | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| classification                                             | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![不支持][NS]                       |
| createdOnBehalfOf/deletedDateTime                          | ![默认支持][RDS]               |                                            | ![默认支持][RDS]               | ![默认支持][RDS]               | ![不支持][NS]                       |
| 说明                                                | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![不支持][NS]                       |
| displayName                                                | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| expirationDateTime                                         | ![需要高级查询参数。][AQP] |                                            | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |
| groupTypes                                                 | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| infoCatalogs                                               | ![默认支持][RDS]               | ![默认支持][RDS]               | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |
| mail                                                       | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| mailEnabled                                                | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| mailNickname                                               | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| membershipRule                                             | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![不支持][NS]                       |
| onPremisesLastSyncDateTime                                 | ![默认支持][RDS]               |                                            | ![默认支持][RDS]               | ![默认支持][RDS]               | ![不支持][NS]                       |
| onPremisesProvisioningErrors/any(o:o/category)             | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| onPremisesProvisioningErrors/any(o:o/propertyCausingError) | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| onPremisesSamAccountName                                   | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![不支持][NS]                       |
| onPremisesSecurityIdentifier                               | ![不支持][NS]                       |                                            |                                            |                                            | ![需要高级查询参数。][AQP] |
| onPremisesSyncEnabled                                      | ![默认支持][RDS]               |                                            |                                            |                                            | ![需要高级查询参数。][AQP] |
| preferredLanguage                                          | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![需要高级查询参数。][AQP] |
| renewedDateTime                                            | ![默认支持][RDS]               |                                            | ![默认支持][RDS]               | ![默认支持][RDS]               | ![不支持][NS]                       |
| resourceProvisioningOptions (仅限 beta 版本)                     | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            |                                            |
| securityEnabled                                            | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |



### <a name="organizational-contact-properties"></a>组织联系人属性

| 属性                                                   | eq                                         | startsWith                                 | ge                           | le                           | Null 值                                 |
|------------------------------------------------------------|--------------------------------------------|--------------------------------------------|------------------------------|------------------------------|--------------------------------------------|
| companyName                                                | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                              |                              | ![需要高级查询参数。][AQP] |
| department                                                 | ![默认支持][RDS]               | ![默认支持][RDS]               |                              |                              | ![需要高级查询参数。][AQP] |
| displayName                                                | ![默认支持][RDS]               | ![默认支持][RDS]               |                              |                              | ![需要高级查询参数。][AQP] |
| givenName                                                  | ![默认支持][RDS]               | ![默认支持][RDS]               |                              |                              | ![需要高级查询参数。][AQP] |
| imAddresses                                                | ![默认支持][RDS]               | ![默认支持][RDS]               | ![默认支持][RDS] | ![默认支持][RDS] |                                            |
| jobTitle                                                   | ![默认支持][RDS]               | ![默认支持][RDS]               |                              |                              | ![需要高级查询参数。][AQP] |
| mail                                                       | ![默认支持][RDS]               | ![默认支持][RDS]               |                              |                              | ![需要高级查询参数。][AQP] |
| mailNickname                                               | ![默认支持][RDS]               | ![默认支持][RDS]               |                              |                              | ![需要高级查询参数。][AQP] |
| onPremisesLastSyncDateTime                                 | ![默认支持][RDS]               |                                            | ![默认支持][RDS] | ![默认支持][RDS] | ![不支持][NS]                       |
| onPremisesProvisioningErrors/any(o:o/category)             | ![默认支持][RDS]               |                                            |                              |                              | ![不支持][NS]                       |
| onPremisesProvisioningErrors/any(o:o/propertyCausingError) | ![默认支持][RDS]               |                                            |                              |                              | ![不支持][NS]                       |
| onPremisesSyncEnabled                                      | ![默认支持][RDS]               |                                            |                              |                              | ![需要高级查询参数。][AQP] |
| surname                                                    | ![默认支持][RDS]               | ![默认支持][RDS]               |                              |                              | ![需要高级查询参数。][AQP] |




### <a name="user-properties"></a>用户属性

| 属性                                                   | eq                                         | startsWith                                 | ge                                         | le                                         | Null 值                                 |
|------------------------------------------------------------|--------------------------------------------|--------------------------------------------|--------------------------------------------|--------------------------------------------|--------------------------------------------|
| accountEnabled                                             | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| ageGroup                                                   | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| assignedLicenses/any (a：a/skuId)                             | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| assignedPlans/any(a:a/capabilityStatus)                    | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![不支持][NS]                       |
| assignedPlans/any(a:a/service)                             | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |                                            |                                            | ![不支持][NS]                       |
| assignedPlans/any(a:a/servicePlanId)                       | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![不支持][NS]                       |
| 城市                                                       | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| companyName                                                | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![需要高级查询参数。][AQP] |
| consentProvidedForMinor                                    | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| 国家                                                    | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| createdDateTime                                            | ![需要高级查询参数。][AQP] |                                            | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |
| createdObjects/any(c:c/id)                                 | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![不支持][NS]                       |
| creationType                                               | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| department                                                 | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| displayName                                                | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| employeeHireDate                                           | ![需要高级查询参数。][AQP] |                                            | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |
| employeeId                                                 | ![默认支持][RDS]               |                                            |                                            |                                            | ![需要高级查询参数。][AQP] |
| employeeOrgData/costCenter                                 | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |                                            |                                            | ![不支持][NS]                       |
| employeeOrgData/division                                   | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |                                            |                                            | ![不支持][NS]                       |
| employeeType                                               | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![不支持][NS]                       |
| externalUserState                                          | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| externalUserStateChangeDateTime                            | ![默认支持][RDS]               |                                            | ![默认支持][RDS]               | ![默认支持][RDS]               | ![不支持][NS]                       |
| faxNumber                                                  | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![需要高级查询参数。][AQP] |
| givenName                                                  | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| identities/any(i:i/issuer)                                 | ![默认支持][RDS]               | ![不支持][NS]                       |                                            |                                            | ![默认支持][RDS]               |
| imAddresses                                                | ![默认支持][RDS]               | ![默认支持][RDS]               | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |
| infoCatalogs                                               | ![默认支持][RDS]               | ![默认支持][RDS]               | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |
| isResourceAccount                                          | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| jobTitle                                                   | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| mail                                                       | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| mailNickname                                               | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| manager/deletedDateTime                                    | ![默认支持][RDS]               |                                            | ![默认支持][RDS]               | ![默认支持][RDS]               | ![不支持][NS]                       |
| mobilePhone                                                | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![需要高级查询参数。][AQP] |
| officeLocation                                             | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![需要高级查询参数。][AQP] |
| onPremisesExtensionAttributes/extensionAttribute1-15       | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |                                            |                                            | ![需要高级查询参数。][AQP] |
| onPremisesImmutableId                                      | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| onPremisesLastSyncDateTime                                 | ![默认支持][RDS]               |                                            | ![默认支持][RDS]               | ![默认支持][RDS]               | ![不支持][NS]                       |
| onPremisesProvisioningErrors/any(o:o/category)             | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| onPremisesProvisioningErrors/any(o:o/propertyCausingError) | ![默认支持][RDS]               |                                            |                                            |                                            | ![不支持][NS]                       |
| onPremisesSamAccountName                                   | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![不支持][NS]                       |
| onPremisesSecurityIdentifier                               | ![不支持][NS]                       |                                            |                                            |                                            | ![需要高级查询参数。][AQP] |
| onPremisesSyncEnabled                                      | ![默认支持][RDS]               |                                            |                                            |                                            | ![需要高级查询参数。][AQP] |
| passwordPolicies                                           | ![不支持][NS]                       | ![不支持][NS]                       |                                            |                                            | ![需要高级查询参数。][AQP] |
| passwordProfile/forceChangePasswordNextSignIn              | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![需要高级查询参数。][AQP] |
| passwordProfile/forceChangePasswordNextSignInWithMfa       | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![需要高级查询参数。][AQP] |
| postalCode                                                 | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![需要高级查询参数。][AQP] |
| preferredLanguage                                          | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![需要高级查询参数。][AQP] |
| provisionedPlans/any(p:p/provisioningStatus)               | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![不支持][NS]                       |
| provisionedPlans/any(p:p/service)                          | ![需要高级查询参数。][AQP] | ![不支持][NS]                       |                                            |                                            | ![不支持][NS]                       |
| showInAddressList                                          | ![需要高级查询参数。][AQP] |                                            |                                            |                                            | ![不支持][NS]                       |
| state                                                      | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| streetAddress                                              | ![需要高级查询参数。][AQP] | ![需要高级查询参数。][AQP] |                                            |                                            | ![需要高级查询参数。][AQP] |
| surname                                                    | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| usageLocation                                              | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![需要高级查询参数。][AQP] |
| userPrincipalName                                          | ![默认支持][RDS]               | ![默认支持][RDS]               |                                            |                                            | ![不支持][NS]                       |
| userType                                                   | ![默认支持][RDS]               |                                            |                                            |                                            | ![需要高级查询参数。][AQP] |

[RDS]: ../concepts/images/advanced-query-parameters/default.svg
[AQP]: ../concepts/images/advanced-query-parameters/advanced.svg
[NS]: ../concepts/images/advanced-query-parameters/notSupported.svg
