---
title: Azure AD Graph和 Microsoft Graph 之间的属性差异
description: 介绍Azure AD Graph资源 (实体) 和 Microsoft Graph 之间的属性差异，以帮助相应地迁移应用。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 2d5df9eede57ff0987bfced91d34c11d4d5142f1
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296238"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph和 Microsoft Graph 之间的属性差异

本文是 *步骤 1 的一部分：查看*[迁移应用的过程](migrate-azure-ad-graph-planning-checklist.md)的 API 差异。

通常，将Azure Active Directory (Azure AD) 图形 API与 Microsoft Graph 进行比较的最佳方法是比较每个服务的基础元数据，尤其是资源说明：

- [Azure AD Graph元数据](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Microsoft Graph beta 元数据](https://graph.microsoft.com/beta/$metadata)
- [Microsoft Graph v1.0 元数据](https://graph.microsoft.com/v1.0/$metadata)

本文重点介绍资源之间的属性差异。 如果此列表中未显示某个属性，则该属性已在 microsoft Graph [的 v1.0 版本](/graph/api/overview)中可用，其名称与Azure AD Graph中的名称完全相同。

由于 [用户](#user-property-differences) 和 [组](#group-property-differences) 资源的使用频率如此之高，因此它们首先列出。 其他资源按字母顺序列出。

## <a name="user-property-differences"></a>用户属性差异

Azure AD Graph **用户** 资源继承自 **DirectoryObject**;它已重命名为 Microsoft Graph中的 **用户**，并继承自 **directoryObject**。 下面是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br>property|备注|
|---|---|---|
| **deletedTimestamp**| beta  &nbsp;-&nbsp; **deletedDateTime** <br> v1.0 &nbsp;-&nbsp; **deletedDateTime** | |
| **dirSyncEnabled** | beta &nbsp;-&nbsp;**onPremisesSyncEnabled** <br> v1.0 &nbsp;-&nbsp; **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | beta  &nbsp;-&nbsp; **faxNumber** <br> v1.0 &nbsp;-&nbsp; **传真编号** | |
| **immutableId** | beta &nbsp;-&nbsp;**onPremisesImmutableId** <br> v1.0 &nbsp;-&nbsp; **onPremisesImmutableId**  | |
| **isCompromised** | beta  &nbsp;-&nbsp; _不可用_ <br> v1.0 &nbsp;-&nbsp; _不可用_ | Microsoft Graph[标识保护](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true) API 提供了更复杂的功能。 |
| **lastDirSyncDateTime** | beta &nbsp;-&nbsp;**onPremisesLastSyncDateTime** <br> v1.0 &nbsp;-&nbsp; **onPremisesLastSyncDateTime** | |
| **mobile** | beta  &nbsp;-&nbsp; **mobilePhone** <br> v1.0 &nbsp;-&nbsp; **mobilePhone** | |
| **passwordProfile/enforceChangePasswordPolicy** | beta  &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignIn** <br> v1.0 &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignIn** | |
| **passwordProfile/forceChangePasswordNextLogin** | beta  &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignInWithMfa** <br> v1.0 &nbsp;-&nbsp; **passwordProfile/forceChangePasswordNextSignInWithMfa** | |
| **provisioningErrors** | beta &nbsp;-&nbsp; _不可用_ <br> v1.0 &nbsp;-&nbsp; _不可用_ | 此属性及其信息已弃用。  但是，可在 **onPremisesProvisioningErrors** 中找到描述任何 AD 连接 相关预配错误的新属性 |
| **refreshTokensValidFromDateTime** | **betasigninSessionsValidFromDateTime**&nbsp;-&nbsp;<br>**v1.0signinSessionsValidFromDateTime**&nbsp;-&nbsp; | |
| **signinNames** | beta &nbsp;-&nbsp; **标识/signInType** <br> v1.0 &nbsp;-&nbsp; **标识/signInType** | 此属性现在是 [objectIdentity](/graph/api/resources/objectIdentity) 资源的一部分。|
| **telephoneNumber** | beta  &nbsp;-&nbsp; **businessPhones** <br> v1.0 &nbsp;-&nbsp; **businessPhones** | |
| **thumbnailPhoto** | beta  &nbsp;-&nbsp; **照片**， 照片 <br> v1.0 &nbsp;-&nbsp; **照片**， 照片 | Azure AD缩略图照片无法通过 Microsoft Graph 获取。  请改用 [照片 API](/graph/api/resources/profilephoto) 。 |
| **userIdentities** | beta &nbsp;-&nbsp; **标识** <br> v1.0 &nbsp;-&nbsp; **标识** | 有关更多详细信息，请参阅 [objectIdentity](/graph/api/resources/objectIdentity) 资源类型。|
| **userState** | beta  &nbsp;-&nbsp; **externalUserState** <br> v1.0 &nbsp;-&nbsp; **externalUserState** | |
| **userStateChangedOn** | **betaexternalUserStateChangeDateTime**&nbsp;-&nbsp;<br>**v1.0externalUserStateChangeDateTime**&nbsp;-&nbsp; | |

## <a name="group-property-differences"></a>组属性差异

Azure AD Graph **组** 资源继承自 **DirectoryObject**;已重命名为 Microsoft Graph 中的 **组**，并继承自 **directoryObject**。 下面是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **dirSyncEnabled** | beta &nbsp;-&nbsp;**onPremisesSyncEnabled** <br> v1.0 &nbsp;-&nbsp; **onPremisesSyncEnabled** | |
| **immutableId** | beta &nbsp;-&nbsp;**onPremisesImmutableId** <br> v1.0 &nbsp;-&nbsp; **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | **betaonPremisesLastSyncDateTime**&nbsp;-&nbsp;<br>**v1.0onPremisesLastSyncDateTime**&nbsp;-&nbsp; | |
| **provisioningErrors** | beta &nbsp;-&nbsp; _不可用_ <br> v1.0 &nbsp;-&nbsp; _不可用_ | 此属性及其信息已弃用。  但是，可在 **onPremisesProvisioningErrors** 中找到描述任何 AD 连接 相关预配错误的新属性 |

## <a name="application-property-differences"></a>应用程序属性差异

Azure AD Graph **应用程序** 资源继承自 **DirectoryObject**;它已重命名为 Microsoft Graph 中的 **应用程序**，并继承自 **directoryObject**。 下面是属性差异：


| Azure AD Graph <br> (v1.6) 属性 | Microsoft Graph<br> property                                                                                                                          | 备注                                                                                                                                                                                                                                                                                                                     |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **acceptMappedClaims**             | beta &nbsp;-&nbsp;**api/acceptMappedClaims** <br> v1.0 &nbsp;-&nbsp; **api/acceptMappedClaims**                                                       | acceptMappedClaims 现在是新 API 资源的一部分。                                                                                                                                                                                                                                                                      |
| **availableToOtherTenants**        | beta &nbsp;-&nbsp; **signInAudience** <br> v1.0 &nbsp;-&nbsp; **signInAudience**                                                                      | availableToOtherTenants `false` 的默认值 (表示 `AzureADMyOrg`) 而 signInAudience 为 `AzureADandPersonalMicrosoftAccount`。                                                                                                                                                                                                                                                                                                                              |
| **errorUrl**                       | beta &nbsp;-&nbsp;_不可用_ <br> v1.0 &nbsp;-&nbsp;  _不可用_                                                                            | 此属性已弃用。                                                                                                                                                                                                                                                                                                 |
| **homepage**                       | beta &nbsp;-&nbsp;**web/homePageUrl** <br> v1.0 &nbsp;-&nbsp; **web/homePageUrl**                                                                     | 主页现在是新 Web 资源的一部分。                                                                                                                                                                                                                                                                                |
| **informationalUrls**              | beta &nbsp;-&nbsp; 信息 <br> v1.0 &nbsp;-&nbsp; 信息                                                                                           |                                                                                                                                                                                                                                                                                                                              |
| **knownClientApplications**        | betaapi&nbsp;-&nbsp;**/knownClientApplications** <br> v1.0 &nbsp;-&nbsp;**api/knownClientApplications**                                               | knownClientApplications 现在是新 api 资源的一部分。                                                                                                                                                                                                                                                                 |
| **logoutUrl**                      | beta &nbsp;-&nbsp;**web/logoutUrl** <br> v1.0 &nbsp;-&nbsp; **web/logoutUrl**                                                                         | logoutUrl 现在是 Web 资源的一部分。                                                                                                                                                                                                                                                                                   |
| **logoUrl**                        | beta &nbsp;-&nbsp;**信息/logoUrl** <br> v1.0 &nbsp;-&nbsp; **信息/logoUrl**                                                                           | logoUrl 现在是新信息资源的一部分。                                                                                                                                                                                                                                                                                |
| **mainLogo**                       | beta &nbsp;-&nbsp;**徽标** <br> v1.0 &nbsp;-&nbsp;  **徽标**                                                                                          |                                                                                                                                                                                                                                                                                                                              |
| **oauth2AllowIdTokenImplicitFlow** | betaweb&nbsp;-&nbsp;**/implicitGrantSettings/enableIdTokenIssuance**<br>v1.0 &nbsp;-&nbsp;**web/implicitGrantSettings/enableIdTokenIssuance**         | 已重命名，现在成为新的隐式GrantSettings 资源的一部分。                                                                                                                                                                                                                                                             |
| **oauth2AllowImplicitFlow**        | betaweb&nbsp;-&nbsp;**/implicitGrantSettings/enableAccessTokenIssuance**<br>v1.0 &nbsp;-&nbsp;**web/implicitGrantSettings/enableAccessTokenIssuance** | 已重命名，现在成为新的隐式GrantSettings 资源的一部分。                                                                                                                                                                                                                                                             |
| **oauth2AllowUrlPathMatching**     | beta &nbsp;-&nbsp;_不可用_ <br> v1.0 &nbsp;-&nbsp;  _不可用_                                                                            | 此属性已弃用。                                                                                                                                                                                                                                                                                                 |
| **oauth2Permissions**              | betaapi&nbsp;-&nbsp;**/oauth2PermissionScopes**<br> v1.0 &nbsp;-&nbsp;**api/oauth2PermissionScopes**                                                  | 已重命名，现在又是新 API 资源的一部分。                                                                                                                                                                                                                                                                                |
| **publicClient**                   | beta &nbsp;-&nbsp; **isFallbackPublicClient** <br> v1.0 &nbsp;-&nbsp; **isFallbackPublicClient**                                                      | 此属性现在具有一个新含义，即 &nbsp;-&nbsp; 它包含公共客户端设置（如 redirectUris）。 确定应用是否是公共客户端还是机密客户端现在自动完成，isFallbackPublicClient 属性处理无法自动确定的一个特殊情况。 |
| **recordConsentConditions**        | beta &nbsp;-&nbsp;_不可用_ <br> v1.0 &nbsp;-&nbsp;  _不可用_                                                                            | 此属性已弃用。                                                                                                                                                                                                                                                                                                 |
| **replyUrls**                      | betaweb&nbsp;-&nbsp;**/redirectUris**、 **publicClient/redirectUris**<br> v1.0 &nbsp;-&nbsp;**web/redirectUris**， **publicClient/redirectUris**        | 除了重命名，redirectUris 现在也是新 Web 和 publicClient 资源的一部分。 这样，开发人员就可以将特定 URI 用于其 Web 和公共客户端 (，例如桌面设备上安装的应用程序) 。                                                                                           |
| **samlMetadataUrl**                | beta  &nbsp;-&nbsp; _尚不可用_  <br> v1.0 &nbsp;-&nbsp; _尚不可用_                                                                  |                                                                                                                                                                                                                                                                                                                              |
| **serviceEndpoints**               | beta  &nbsp;-&nbsp; _不可用_  <br> v1.0 &nbsp;-&nbsp; _不可用_                                                                          | 此属性已弃用，但计划用于 servicePrincipal。                                                                                                                                                                                                                                                            |

## <a name="approleassignment-differences"></a>AppRoleAssignment 差异

Azure AD Graph **AppRoleAssignment** 资源继承自 **DirectoryObject**;已在 Microsoft Graph中重命名为 **appRoleAssignment**，并继承自 **directoryObject**。 下面是属性差异：


|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **creationTimestamp** | beta &nbsp;-&nbsp;**creationTimestamp** <br> v1.0 &nbsp;-&nbsp;**createdDateTime** | |
| **id** | beta &nbsp;-&nbsp;**appRoleId** <br> v1.0 &nbsp;-&nbsp;**appRoleId** | |

## <a name="contact-property-differences"></a>联系人属性差异

Azure AD Graph **联系** 人资源继承自 **DirectoryObject**;已在 Microsoft Graph 中重命名为 **orgContact**，并从 **directoryObject** 继承。 下面是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **城市** | **betaaddresse**&nbsp;-&nbsp;/city <br> v1.0 &nbsp;-&nbsp; **地址/城市**  | **City** 属性是 **地址** 资源集合的一部分。 |
| **country** | betaaddresses&nbsp;-&nbsp;**/countryOrRegion**<br> v1.0addresses&nbsp;-&nbsp;**/countryOrRegion**  | **countryOrRegion** 属性是 **地址** 资源集合的一部分。 |
| **dirSyncEnabled** | beta &nbsp;-&nbsp;**onPremisesSyncEnabled** <br> v1.0 &nbsp;-&nbsp;**onPremisesSyncEnabled**   | |
| **facsimileTelephoneNumber** | betaphones&nbsp;-&nbsp;**/businessFax** <br> v1.0 &nbsp;-&nbsp;**phone/businessFax** | 现在，支持各种 **手机类型的手机** 集合的一部分。 |
| **physicalDeliveryOfficeName** | beta &nbsp;-&nbsp;**officeLocation** <br> v1.0 &nbsp;-&nbsp; **officeLocation** | |
| **postalCode** | **betaaddresses**&nbsp;-&nbsp;/postalCode<br> v1.0 &nbsp;-&nbsp;**地址/邮政编码** | **postalCode** 属性是 **地址** 资源集合的一部分。 |
| **provisioningErrors** | beta &nbsp;-&nbsp; 不可用 <br> v1.0 &nbsp;-&nbsp; 不可用 | 此属性及其信息已弃用。  但是，可以在 **onPremisesProvisioningErrors** 中找到描述任何 AD 连接相关预配错误的新属性。 目前，这仅在 { 中 `beta`可用。 |
| **sipProxyAddress** |  beta &nbsp;-&nbsp;**imAddresses**<br> v1.0 &nbsp;-&nbsp;**imAddresses**  | |
| **state** | beta &nbsp;-&nbsp;**地址/状态**<br> v1.0 &nbsp;-&nbsp; **地址/状态**  | **State** 属性是 **地址** 资源集合的一部分。 |
| **streetAddress** | beta &nbsp;-&nbsp;**地址/街道**<br> v1.0 &nbsp;-&nbsp;**地址/街道**  | **street** 属性是 **地址** 资源集合的一部分。 |
| **telephoneNumber** | **betaphones**&nbsp;-&nbsp;/business <br> v1.0 &nbsp;-&nbsp;**电话/商业版** | 现在，支持各种 **手机类型的手机** 集合的一部分。 |
| **thumbnailPhoto** | beta &nbsp;-&nbsp;_Notyetavailable&nbsp;&nbsp;_&nbsp;<br> v1.0 &nbsp;-&nbsp; _尚不可用_ | |

## <a name="contract-property-differences"></a>协定属性差异

Azure AD Graph **协定** 资源继承自 **DirectoryObject**;已在 Microsoft Graph 中重命名为 **协定**，并继承自 **directoryObject**。 下面是属性差异：


|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **customerContextId** | beta &nbsp;-&nbsp;**customerId** <br> v1.0 &nbsp;-&nbsp; **customerId**  |  |

## <a name="device-property-differences"></a>设备属性差异

Azure AD Graph **设备** 资源继承自 **DirectoryObject**;它已重命名为 Microsoft Graph 中的 **设备**，并继承自 **directoryObject**。 下面是属性差异：


|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **approximateLastLogonTimestamp** | **betaapproximateLastSignInDateTime**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | **betacomplianceExpirationDateTime**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  **betadeviceVersion**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **deviceVersion** |  |
| **deviceOSType** | **betaoperatingSystem**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **operatingSystem** |  |
| **deviceOSVersion** | **betaoperatingSystemVersion**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **operatingSystemVersion** |  |
| **devicePhysicalIds** | **betaphysicalIds**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **physicalIds** |  |
| **deviceTrustType** | **betatrustType**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **trustType** |  |
| **dirSyncEnabled** |  **betaonPremisesSyncEnabled**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  **betaonPremisesLastSyncDateTime**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **onPremisesLastSyncDateTime** |  |

## <a name="directoryobject-property-differences"></a>DirectoryObject 属性差异

Azure AD Graph **DirectoryObject** 资源已重命名为 Microsoft Graph 中的 **directoryObject**。 在从 **DirectoryObject** 继承的其他资源中也会看到对其属性所做的更改。 下面是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **deletionTimestamp** | **betadeletedDateTime**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **deletedDateTime** | 虽然 **deletionTimestamp** 是 DateTime 类型，但 **deletedDateTime** 是 DateTimeOffset 类型。  |
| **objectId** | **betaid**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; ID | Microsoft Graph中的 **id** 属性继承自 [实体](/graph/api/resources/entity)资源。 |
| **objectType** | *betaNot*&nbsp;-&nbsp; 可用 <br> v1.0 &nbsp;-&nbsp; *不可用* | Microsoft Graph 中不使用此属性。 相反，Microsoft Graph返回 **@odata.type** 属性，但仅返回可能返回不同类型或派生类型的对象的 API。 例如， [列表组成员](/graph/api/group-list-members) API 可能会返回 [用户](/graph/api/resources/user)、 [组](/graph/api/resources/group)、 [服务主体](/graph/api/resources/serviceprincipal)、 [组织联系人](/graph/api/resources/orgcontact)或 [设备](/graph/api/resources/device)的成员。 对于用户， **@odata.type** 为 `#microsoft.graph.user`. |

## <a name="directoryobjectreference-property-differences"></a>DirectoryObjectReference 属性差异

Azure AD Graph **DirectoryObjectReference** 资源继承自 **DirectoryObject**;已重命名为 Microsoft Graph 中的 **directoryObjectPartnerReference**，并继承自 **directoryObject**。 下面是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **externalContextId** | **betaexternalPartnerTenantId**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>域属性差异

Azure AD Graph **域** 资源已重命名为 Microsoft Graph 中的 **域**。 下面是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **名称** | **betaid**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; ID | 在 Microsoft Graph中，唯一标识符 (id) 包含域名;`name`该属性不存在。 |
| **forceDeleteState** |  **betastate**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; 状态 | 在Azure AD Graph中，有单独的 forceDelete 和域状态属性。  在 Microsoft Graph中，所有域状态都由状态属性处理。 |
| **isDefaultForCloudRedirections** | _betaNotyetavailable&nbsp;&nbsp;_&nbsp;-&nbsp;&nbsp;<br> v1.0 &nbsp;-&nbsp; _尚不可用_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>OAuth2PermissionsGrant 属性差异

Azure AD Graph **OAuth2PermissionsGrant** 资源已重命名为 Microsoft Graph 中的 **oAuth2PermissionsGrant**。 下面是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **expiryTime** | **betaexpiryTime**&nbsp;-&nbsp; <br> _v1.0Removed_&nbsp;-&nbsp; | 此属性未使用，在 Microsoft Graph v1.0 中删除。 |
| **startTime** | **betastartTime**&nbsp;-&nbsp; <br> _v1.0Removed_&nbsp;-&nbsp;  | 此属性未使用，在 Microsoft Graph v1.0 中删除。 |

## <a name="policy-property-differences"></a>策略属性差异

在 Microsoft Graph中， (有命名策略类型，例如 **tokenIssuancePolicy** 或 **tokenLifetimePolicy**) ，而不是泛型策略资源类型。 策略 [概述](/graph/api/resources/policy-overview)中提供了更多详细信息。

## <a name="serviceendpoint-property-differences"></a>ServiceEndpoint 属性差异

Azure AD Graph **ServiceEndpoint** 资源继承自 **DirectoryObject**;它已重命名为 Microsoft Graph 中的 **终结点**，并继承自 **directoryObject**。 下面是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **服务 Id** | **betaproviderId**&nbsp;-&nbsp;<br> v1.0 &nbsp;-&nbsp;**providerId** | |
| **serviceName** | **betaproviderName**&nbsp;-&nbsp;<br> v1.0 &nbsp;-&nbsp;**providerName** | |
| **resourceId** | **betaproviderResourceId**&nbsp;-&nbsp;<br> v1.0 &nbsp;-&nbsp;**providerResourceId** | |

## <a name="serviceprincipal-property-differences"></a>ServicePrincipal 属性差异

Azure AD Graph **ServicePrincipal** 资源继承自 **DirectoryObject**;已重命名为 Microsoft Graph 中的 **servicePrincipal**，并继承自 **directoryObject**。 下面是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **appOwnerTenantId** | **betaappOwnerOrganizationId**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp;**appOwnerOrganizationId** | 重 命名。 |
| **informationalUrls**| beta &nbsp;-&nbsp; 信息 <br> v1.0 &nbsp;-&nbsp; 信息 | |
| **oauth2Permissions** | beta  &nbsp;-&nbsp;**publishedPermissionScopes** <br> v1.0  &nbsp;-&nbsp;**oauth2PermissionScopes** | 重 命名。 |
| **preferredTokenSigningKeyEndDateTime** | _betaNot_&nbsp;-&nbsp; 尚未提供 <br> v1.0 &nbsp;- _尚不可用_ | |
| **signInAudience** | _betaNot_&nbsp;-&nbsp; 尚未提供 <br> v1.0 &nbsp;- _尚不可用_ | |
| **serviceEndpoints** | **betaendpoint**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp;**终结点** | 重 命名。 |

## <a name="tenantdetails-property-differences"></a>TenantDetails 属性差异

Azure AD Graph **TenantDetail** 资源继承自 **DirectoryObject**;它已重命名为 Microsoft Graph 中的 **组织**，并继承自 **directoryObject**。 下面是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **companyLastDirSyncTime** | **betaonPremisesLastSyncDateTime**&nbsp;-&nbsp; <br> **v1.0onPremisesLastSyncDateTime**&nbsp;-&nbsp; |  |
| **dirSyncEnabled** | **betaonPremisesSyncEnabled**&nbsp;-&nbsp; <br> v1.0 &nbsp;-&nbsp; **onPremisesSyncEnabled** |  |
| **provisioningErrors** | _betaNot_&nbsp;-&nbsp; 可用 <br> v1.0Not&nbsp;-&nbsp; _可用_ | 此属性及其信息已弃用。|
| **telephoneNumber** | **betabusinessPhones**&nbsp;-&nbsp; <br> **v1.0businessPhones**&nbsp;-&nbsp; |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>TrustedCasForPasswordlessAuth 属性差异

Azure AD Graph **TrustedCasForPasswordlessAuth** 资源已重命名为 [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration)。 没有属性差异;但是，**certificateAuthorities** 属性使用的 **certificateAuthority** 资源类型存在差异。

### <a name="certificateauthorityinformation-property-differences"></a>CertificateAuthorityInformation 属性差异

Azure AD Graph **CertificateAuthorityInformation** 已在 Microsoft Graph 中重命名为 **certificateAuthority**。 下面是属性差异。

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **authorityType** | **betaisRootAuthority**&nbsp;-&nbsp;<br> v1.0 &nbsp;-&nbsp;**isRootAuthority** | 此属性的类型也已更改为布尔值。 以前，此属性必须设置为“RootAuthority”或“IntermediateAuthority”。 将新属性设置为 **true** 等效于“RootAuthority”。 |
| **crlDistributionPoint** | **betacertificateRevocationListUrl**&nbsp;-&nbsp; <br> **v1.0certificateRevocationListUrl**&nbsp;-&nbsp; | |
| **deltaCrlDistributionPoint** | **betadeltaCertificateRevocationListUrl**&nbsp;-&nbsp; <br> **v1.0deltaCertificateRevocationListUrl**&nbsp;-&nbsp; | |
| **trustedCertificate** | **betacertificate**&nbsp;-&nbsp; <br> **v1.0deltaCertificateRevocationListUrl**&nbsp;-&nbsp; | |
| **trustedIssuer** | **betaissuer**&nbsp;-&nbsp;<br> **v1.0issuer**&nbsp;-&nbsp; | |
| **trustedIssuerSki** | **betaissuerSki**&nbsp;-&nbsp;<br> v1.0 &nbsp;-&nbsp;**issuerSki** | |

## <a name="next-steps"></a>后续步骤

- 了解Azure AD Graph与 Microsoft Graph 之间的[方法差异](migrate-azure-ad-graph-method-differences.md)。
- 再次查看 [清单](migrate-azure-ad-graph-planning-checklist.md) 。

