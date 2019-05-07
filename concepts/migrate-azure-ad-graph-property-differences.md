---
title: Azure AD Graph 与 Microsoft Graph 之间的属性差异
description: 介绍了 Azure AD Graph 资源 (实体) 与 Microsoft Graph 之间的属性差异, 以便帮助您相应地迁移应用。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e2f8ba237cd86ab2361c98f5b51afaa77d2b7f50
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630214"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph 与 Microsoft Graph 之间的属性差异

本文是*第1步: 查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。

通常, 将 Azure AD Graph API 与 Microsoft Graph 进行比较的最佳方式是比较每个服务的基础元数据, 尤其是资源说明:

- [Azure AD Graph 元数据](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Microsoft Graph beta 元数据](https://graph.microsoft.com/beta /$metadata)
- [Microsoft Graph 1。0版元数据](https://graph.microsoft.comv/1.0/$metadata)

在这里, 将突出显示资源之间的属性差异。 如果某个属性未显示在此列表中, 则该属性在 Microsoft Graph 的 v1。0[版本](/graph/api/overview?view=graph-rest-1.0)中已可用, 与 Azure AD Graph 中的名称完全相同。

由于经常使用用户和组, 因此先显示这些资源。  其他资源按字母顺序显示。

## <a name="user-property-differences"></a>用户属性差异

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br>property|Comments|
|---|---|---|
| **appRoleAssignments** | beta- **appRoleAssignments** <br> v1。0-_尚不可用_ | |
| **creationType** | beta 版-_尚不可用_ <br> v1。0-_尚不可用_| |
| **deletedTimestamp**| beta- **deletedDateTime** <br> v1。0- **deletedDateTime** | |
| **dirSyncEnabled** | &nbsp; -beta &nbsp; **onPremisesSyncEnabled** <br> v1。0- **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | beta- **faxNumber** <br> v1。0- **faxNumber** | |
| **immutableId** | &nbsp; -beta &nbsp; **onPremisesImmutableId** <br> v1。0- **onPremisesImmutableId**  | |
| **isCompromised** | beta 版-_不可用_ <br> v1。0-不可_用_ | Microsoft Graph[标识保护](/graph/api/resources/identityprotection-root?view=graph-rest-beta)API 提供了更复杂的功能。 |
| **lastDirSyncDateTime** | &nbsp; -beta &nbsp; **onPremisesLastSyncDateTime** <br> v1。0- **onPremisesLastSyncDateTime** | |
| **mobile** | beta- **mobilePhone** <br> v1。0- **mobilePhone** | |
| **oAuth2PermissionGrants** | beta- **oAuth2PermissionGrants** <br> v1。0-_尚不可用_ ||
| **provisioningErrors** | &nbsp; -beta &nbsp; **onPremisesProvisioningErrors** <br> v1。0- **onPremisesProvisioningErrors** | |
| **refreshTokensValidFromDateTime** | &nbsp;-beta&nbsp;**signinSessionsValidFromDateTime**<br>v1。0尚_不可用_&nbsp;-&nbsp; | |
| **signinNames** | beta 版-_尚不可用_ <br> v1。0-_尚不可用_ | |
| **telephoneNumber** | beta- **businessPhones** <br> v1。0- **businessPhones** | |
| **thumbnailPhoto** | beta-**照片**、照片 <br> v1。0-**照片**、照片 | Azure AD 缩略图照片在 Microsoft Graph 中不可用。  改为使用[照片 API](/graph/api/resources/profilephoto?view=graph-rest-1.0) 。 |
| **userIdentities** | beta 版-_尚不可用_ <br> v1。0-_尚不可用_ | |
| **userState** | beta- **externalUserState** <br> v1。0- **externalUserState** | |
| **userStateChangedOn** | &nbsp;-beta&nbsp;**externalUserStateChangeDateTime**<br>&nbsp;**** v1。0 externalUserStateChangeDateTime&nbsp;- | |

## <a name="group-property-differences"></a>组属性差异

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **dirSyncEnabled** | &nbsp; -beta &nbsp; **onPremisesSyncEnabled** <br> v1。0- **onPremisesSyncEnabled** | |
| **immutableId** | &nbsp; -beta &nbsp; **onPremisesImmutableId** <br> v1。0- **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | &nbsp;-beta&nbsp;**onPremisesLastSyncDateTime**<br>v1。0- **onPremisesLastSyncDateTime** | |
| **onPremisesDomainName** | beta 版-_尚不可用_ <br> v1。0-_尚不可用_ | 已计划, 但尚不可用。 |
| **onPremisesNetBiosName** | beta 版-_尚不可用_ <br> v1。0-_尚不可用_ | 已计划, 但尚不可用。 |
| **onPremisesSamAccountName** | beta 版-_尚不可用_ <br> v1。0-_尚不可用_ | 已计划, 但尚不可用。 |
| **provisioningErrors** | &nbsp;-beta&nbsp;**onPremisesProvisioningErrors**<br> v1。0- **onPremisesProvisioningErrors** | |

## <a name="application-property-differences"></a>应用程序属性差异

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **acceptMappedClaims**  | &nbsp; -beta &nbsp; **api/acceptMappedClaims** <br> v1。0-_尚不可用_ | acceptMappedClaims 现在是新 api 资源的一部分。 |
| **addIns** | beta 版-_尚不可用_ <br> v1。0-_尚不可用_  | |
| **applicationTemplateId** | beta 版-_尚不可用_ <br> v1。0-_尚不可用_ | |
| **命名** | &nbsp; - beta &nbsp; **orgRestrictions** <br> v1。0-_尚不可用_ | |
| **errorUrl**| &nbsp; -beta &nbsp;_不可用_ <br> v1。0-不可_用_ | 此属性已被弃用。|
| **homepage**| &nbsp; -beta &nbsp; **web/主页** <br> v1。0-_尚不可用_ | 主页现在是新 web 资源的一部分。|
| **informationalUrls**| &nbsp; -beta &nbsp;**信息** <br> v1。0-_尚不可用_ | |
| **knownClientApplications**| &nbsp;-beta&nbsp;**api/knownClientApplications** <br> v1。0-_尚不可用_ | knownClientApplications 现在是新 api 资源的一部分。 |
| **logoutUrl**| &nbsp; -beta &nbsp; **web/logoutUrl** <br> v1。0-_尚不可用_ | logoutUrl 现在是 web 资源的一部分。 |
| **logoUrl**| &nbsp; -beta &nbsp;**信息/logoUrl** <br> v1。0-_尚不可用_ | logoUrl 现在是新的 info 资源的一部分。 |
| **mainLogo**| &nbsp; -beta &nbsp;_不可用_ <br> v1。0-不可_用_ | 此属性已被弃用。|
| **oauth2AllowIdTokenImplicitFlow** | &nbsp;-beta&nbsp;**web/implicitGrantSettings/enableIdTokenIssuance**<br>v1。0-_尚不可用_ | 重命名, 现在是新的 implicitGrantSettings 资源的一部分。 |
| **oauth2AllowImplicitFlow**| &nbsp;-beta&nbsp;**web/oauth2AllowImplicitFlow**<br>v1。0-_尚不可用_ | oauth2AllowImplicitFlow 现在是新 web 资源的一部分。 |
| **oauth2AllowUrlPathMatching**| &nbsp; -beta &nbsp;_不可用_ <br> v1。0-不可_用_ | 此属性已被弃用。|
| **oauth2Permissions**| &nbsp;-beta&nbsp;**api/oauth2PermissionScopes**<br> v1。0-_尚不可用_ | 重命名, 现在是新 api 资源的一部分。 |
| **oauth2RequirePostResponse**| &nbsp; -beta &nbsp;_不可用_ <br> v1。0-不可_用_ | 此属性已被弃用。|
| **publicClient**| &nbsp; - beta &nbsp; **isFallbackPublicClient** <br> v1。0-_尚不可用_ | 此属性现在有一个新的含义-它包含公共客户端设置, 如 redirectUris。 现在, 使用 isFallbackPublicClient 属性处理一个不能自动确定的特殊情况, 来确定应用是否为公用或机密客户端。|
| **recordConsentConditions**| &nbsp; -beta &nbsp;_不可用_ <br> v1。0-不可_用_ | 此属性已被弃用。|
| **replyUrls**| &nbsp;-beta&nbsp;**web/redirectUris**<br> v1。0-_尚不可用_ | 除了重命名, redirectUris 现在也是新的 web 资源的一部分。 | |
| **samlMetadataUrl**| beta 版-_尚不可用_  <br> v1。0-_尚不可用_  | |
| **extensionProperties**| &nbsp; -beta &nbsp; **extensionProperties** <br> v1。0-_尚不可用_ | 此属性已被弃用。 |
| **serviceEndpoints**|  beta 版-_尚不可用_  <br> v1。0-_尚不可用_  | |

## <a name="approleassignment-differences"></a>AppRoleAssignment 差异

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **creationTimestamp** | &nbsp; -beta &nbsp; **creationTimestamp** <br> v1。0-_尚不可用_ | 这将被重命名为 createdDateTime。|
| **id** | &nbsp; -beta &nbsp; **appRoleId** <br> v1。0-_尚不可用_ | |

## <a name="contact-property-differences"></a>联系人属性差异

Azure AD Graph 联系人资源已重命名为 Microsoft Graph 中的 orgContact。  属性差异如下所示:

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **城市** | &nbsp;-beta&nbsp;**地址 (城市)** <br> v1。0-_尚不可用_  | City 属性是 "地址" 资源集合的一部分。 |
| **country** | &nbsp;-beta&nbsp;**** 地址&nbsp;**(countryOrRegion)**<br> v1。0-_尚不可用_  | CountryOrRegion 属性是 "地址" 资源集合的一部分。 |
| **dirSyncEnabled** | &nbsp; -beta &nbsp; **onPremisesSyncEnabled** <br> v1。0-_尚不可用_  | |
| **facsimileTelephoneNumber** | &nbsp;-beta&nbsp;**** 手机&nbsp;**(businessFax)** <br> v1。0-_尚不可用_ | 现在是电话集合的一部分, 它支持移动、商业和 businessFax。 |
| **physicalDeliveryOfficeName** | &nbsp; -beta &nbsp; **officeLocation** <br> v1。0- **officeLocation** | |
| **postalCode** | &nbsp;-beta&nbsp;**** 地址&nbsp;**(邮政编码)**<br> v1。0-_尚不可用_  | "邮政编码" 属性是 "地址" 资源集合的一部分。 |
| **provisioningErrors** | &nbsp;-beta&nbsp;**onPremisesProvisioningErrors**<br> v1。0-_尚不可用_  | |
| **sipProxyAddress** |  &nbsp; -beta &nbsp; **imAddresses**<br> v1。0-_尚不可用_  | |
| **state** | &nbsp; -beta &nbsp; **** 地址&nbsp;**(状态)**<br> v1。0-_尚不可用_  | State 属性是 "addresses" 资源集合的一部分。 |
| **streetAddress** | &nbsp; -beta &nbsp; **** 地址&nbsp;**(街道)**<br> v1。0-_尚不可用_  | "街道" 属性是 "地址" 资源集合的一部分。 |
| **telephoneNumber** | &nbsp;-beta&nbsp;**** 手机&nbsp;**(业务)** <br> v1。0-_尚不可用_ | 现在是电话集合的一部分, 它支持移动、商业和 businessFax。 |
| **thumbnailPhoto** | &nbsp; -beta &nbsp;_尚&nbsp;不可用&nbsp;_&nbsp;<br> v1。0-_尚不可用_ | |

## <a name="contract-property-differences"></a>协定属性差异

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **customerContextId** | &nbsp; -beta &nbsp; **customerId** <br> v1。0- **customerId**  |  |

## <a name="device-property-differences"></a>设备属性差异

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **approximateLastLogonTimestamp** | &nbsp;-beta&nbsp;**approximateLastSignInDateTime** <br> v1。0- **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | &nbsp;-beta&nbsp;**complianceExpirationDateTime** <br> v1。0- **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  &nbsp;-beta&nbsp;**deviceVersion** <br> v1。0- **deviceVersion** |  |
| **deviceOSType** | &nbsp;-beta&nbsp;**操作系统** <br> v1。0-**操作系统** |  |
| **deviceOSVersion** | &nbsp;-beta&nbsp;**operatingSystemVersion** <br> v1。0- **operatingSystemVersion** |  |
| **devicePhysicalIds** | &nbsp;-beta&nbsp;**physicalIds** <br> v1。0- **physicalIds** |  |
| **deviceTrustType** | &nbsp;-beta&nbsp;**trustType** <br> v1。0- **trustType** |  |
| **dirSyncEnabled** |  &nbsp;-beta&nbsp;**onPremisesSyncEnabled** <br> v1。0- **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  &nbsp;-beta&nbsp;**onPremisesLastSyncDateTime** <br> v1。0- **onPremisesLastSyncDateTime** |  |

## <a name="directoryobjectreference-property-differences"></a>DirectoryObjectReference 属性差异

Azure AD Graph directoryObjectReference 资源已重命名为 Microsoft Graph 中的 directoryObjectPartnerReference。  属性差异如下所示:

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **externalContextId** | &nbsp;-beta&nbsp;**externalPartnerTenantId** <br> v1。0- **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>域属性差异

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **name** | &nbsp;-beta&nbsp;**id** <br> 1。0版- **id** | 在 Microsoft Graph 中, 唯一标识符 (id) 包含域名称;`name`属性不存在。 |
| **forceDeleteState** |  &nbsp;-beta&nbsp;**状态** <br> 1。0版-**状态** | 在 Azure AD Graph 中, 存在单独的 forceDelete 和域状态属性。  在 Microsoft Graph 中, 所有域的状态都由 state 属性处理。 |
| **isDefaultForCloudRedirections** | &nbsp;-beta&nbsp;_尚&nbsp;不可用&nbsp;_&nbsp;<br> v1。0-_尚不可用_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>OAuth2PermissionsGrant 属性差异

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **expiryTime** | &nbsp;-beta&nbsp;**expiryTime** <br> &nbsp;_v1。0尚&nbsp;不可用&nbsp;_ &nbsp;- | 此属性不使用, 并且可能会在 Microsoft Graph 中被删除。 |
| **startTime** | beta&nbsp;-&nbsp;版**startTime** <br> &nbsp;_v1。0尚&nbsp;不可用&nbsp;_ &nbsp;-  | 此属性不使用, 并且可能会在 Microsoft Graph 中被删除。 |

## <a name="policy-property-differences"></a>策略属性差异

目前, Microsoft Graph 中的策略资源 (仅在预览中可用) 与 Azure AD Graph 非常相似。  但是, 它会发生更改, 以便有命名的策略类型 (如 tokenIssuancePolicy 或 tokenLifetimePolicy), 而不是通用策略资源类型。

## <a name="serviceendpoint-property-differences"></a>ServiceEndpoint 属性差异

Azure AD Graph ServiceEndpoint 资源已重命名为 Microsoft Graph 中的终结点。

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **性能** | &nbsp;-beta&nbsp;**功能**<br> v1。0-_尚不可用_ | |
| **serviceId** | &nbsp;-beta&nbsp;**providerId**<br> v1。0-_尚不可用_ | |
| **serviceName** | &nbsp;-beta&nbsp;**providerName**<br> v1。0-_尚不可用_ | |
| **resourceId** | &nbsp;-beta&nbsp;**providerResourceId**<br> v1。0-_尚不可用_ | |
| **url** | &nbsp;-beta&nbsp;**uri**<br> v1。0-_尚不可用_ | |

## <a name="serviceprincipal-property-differences"></a>ServicePrincipal 属性差异

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **applicationTemplateId** | beta 版-_尚不可用_ <br> v1。0-_尚不可用_ | |
| **appOwnerTenantId** | &nbsp;-beta&nbsp;**appOwnerOrganizationId** <br> v1。0-_尚不可用_ | |
| **informationalUrls**| &nbsp;-beta&nbsp;_尚不可用_ <br> v1。0-_尚不可用_ | |
| **preferredSingleSignOnMode** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1。0-_尚不可用_ | |
| **preferredTokenSigningKeyEndDateTime** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1。0-_尚不可用_ | |
| **samlSingleSignOnSettings** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1。0-_尚不可用_ | |
| **servicePrincipalType** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1。0-_尚不可用_ | |
| **signInAudience** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1。0-_尚不可用_ | |
| **tokenEncryptionKeyId** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1。0-_尚不可用_ | |
| **serviceEndpoints** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1。0-_尚不可用_ | |

## <a name="tenantdetails-property-differences"></a>TenantDetails 属性差异

在 Microsoft Graph 中, Azure AD Graph TenantDetails 资源被重命名为 "组织"。  属性差异如下所示:

|Azure AD Graph <br>(v 1。6) 属性 |Microsoft Graph<br> property|Comments|
|---|---|---|
| **companyLastDirSyncTime** | &nbsp;-beta&nbsp;**onPremisesLastSyncDateTime** <br>v1。0- **onPremisesLastSyncDateTime** |  |
| **dirSyncEnabled** | &nbsp;-beta&nbsp;**onPremisesSyncEnabled** <br> v1。0- **onPremisesSyncEnabled** |  |
| **provisoningErrors** | &nbsp;-beta&nbsp;_尚&nbsp;不可用&nbsp;_<br> v1。0-_尚不可用_ | |
| **telephoneNumber** | &nbsp;-beta&nbsp;**businessPhones** <br> v1。0- **businessPhones** |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>TrustedCasForPasswordlessAuth 属性差异

Azure AD Graph TrustedCasForPasswordlessAuth 资源已重命名为 Microsoft Graph 中的 certificateBasedAuthConfiguration。  没有属性差异。

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Graph 与 Microsoft Graph 之间的[方法差异](migrate-azure-ad-graph-method-differences.md)。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
