---
title: Azure AD Graph 与 Microsoft Graph 之间的属性差异
description: 介绍了 Azure AD Graph 资源（实体）与 Microsoft Graph 之间的属性差异，以便帮助您相应地迁移应用。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2294956bd24a6fc984032b68ab1d2a7298a87e74
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41233947"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph 与 Microsoft Graph 之间的属性差异

本文是*第1步：查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。

通常，将 Azure AD Graph API 与 Microsoft Graph 进行比较的最佳方式是比较每个服务的基础元数据，尤其是资源说明：

- [Azure AD Graph 元数据](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Microsoft Graph beta 元数据](https://graph.microsoft.com/beta /$metadata)
- [Microsoft Graph 1.0 版元数据](https://graph.microsoft.comv/1.0/$metadata)

在这里，将突出显示资源之间的属性差异。 如果某个属性未显示在此列表中，则该属性在 Microsoft Graph 的 v1.0[版本](/graph/api/overview?view=graph-rest-1.0)中已可用，与 Azure AD Graph 中的名称完全相同。

由于经常使用用户和组，因此先显示这些资源。  其他资源按字母顺序显示。

## <a name="user-property-differences"></a>用户属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br>property|备注|
|---|---|---|
| **appRoleAssignments** | &nbsp; - beta &nbsp; **appRoleAssignments** <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **deletedTimestamp**| &nbsp; - beta &nbsp; **deletedDateTime** <br> &nbsp; **** v1.0 deletedDateTime &nbsp; - | |
| **dirSyncEnabled** | &nbsp; -beta &nbsp; **onPremisesSyncEnabled** <br> &nbsp; **** v1.0 onPremisesSyncEnabled &nbsp; - | |
| **facsimileTelephoneNumber** | &nbsp; - beta &nbsp; **faxNumber** <br> &nbsp; **** v1.0 faxNumber &nbsp; - | |
| **immutableId** | &nbsp; -beta &nbsp; **onPremisesImmutableId** <br> &nbsp; **** v1.0 onPremisesImmutableId &nbsp; -  | |
| **isCompromised** | &nbsp; - beta &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_ | Microsoft Graph[标识保护](/graph/api/resources/identityprotection-root?view=graph-rest-beta)API 提供了更复杂的功能。 |
| **lastDirSyncDateTime** | &nbsp; -beta &nbsp; **onPremisesLastSyncDateTime** <br> &nbsp; **** v1.0 onPremisesLastSyncDateTime &nbsp; - | |
| **mobile** | &nbsp; - beta &nbsp; **mobilePhone** <br> &nbsp; **** v1.0 mobilePhone &nbsp; - | |
| **oAuth2PermissionGrants** | &nbsp; - beta &nbsp; **oAuth2PermissionGrants** <br> v1.0 尚_不可用_ &nbsp; - &nbsp; ||
| **provisioningErrors** | &nbsp; - beta &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_ | 此属性及其信息已被弃用。  但是，可以在**onPremisesProvisioningErrors**中找到描述任何 AD Connect 相关设置错误的新属性。 |
| **refreshTokensValidFromDateTime** | &nbsp;-beta&nbsp;**signinSessionsValidFromDateTime**<br>v1.0 尚_不可用_&nbsp;-&nbsp; | |
| **signinNames** | &nbsp; - beta &nbsp; **标识/signInType** <br> &nbsp; - 1.0 &nbsp;版**标识/signInType** | 此属性现在是[objectIdentity](/graph/api/resources/objectIdentity?view=graph-rest-1.0)资源的一部分。|
| **telephoneNumber** | &nbsp; - beta &nbsp; **businessPhones** <br> &nbsp; **** v1.0 businessPhones &nbsp; - | |
| **thumbnailPhoto** | &nbsp; - beta &nbsp; **照片**、照片 <br> v1.0 照片，照片**** &nbsp; - &nbsp; | Azure AD 缩略图照片在 Microsoft Graph 中不可用。  改为使用[照片 API](/graph/api/resources/profilephoto?view=graph-rest-1.0) 。 |
| **userIdentities** | &nbsp; - beta &nbsp; **标识** <br> &nbsp; - 1.0 &nbsp;版**标识** | 有关更多详细信息，请参阅[objectIdentity](/graph/api/resources/objectIdentity?view=graph-rest-1.0)资源类型。|
| **userState** | &nbsp; - beta &nbsp; **externalUserState** <br> &nbsp; **** v1.0 externalUserState &nbsp; - | |
| **userStateChangedOn** | &nbsp;-beta&nbsp;**externalUserStateChangeDateTime**<br>&nbsp;**** v1.0 externalUserStateChangeDateTime&nbsp;- | |

## <a name="group-property-differences"></a>组属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **dirSyncEnabled** | &nbsp; -beta &nbsp; **onPremisesSyncEnabled** <br> &nbsp; **** v1.0 onPremisesSyncEnabled &nbsp; - | |
| **immutableId** | &nbsp; -beta &nbsp; **onPremisesImmutableId** <br> &nbsp; **** v1.0 onPremisesImmutableId &nbsp; - | |
| **lastDirSyncDateTime** | &nbsp;-beta&nbsp;**onPremisesLastSyncDateTime**<br>&nbsp; **** v1.0 onPremisesLastSyncDateTime &nbsp; - | |
| **onPremisesDomainName** | &nbsp; - beta &nbsp; 、onpremisesdomainname <br> &nbsp; - v1.0 &nbsp; 、onpremisesdomainname | |
| **onPremisesNetBiosName** | &nbsp; - beta &nbsp; onPremisesNetBiosName <br> &nbsp; - v1.0 &nbsp; onPremisesNetBiosName | |
| **onPremisesSamAccountName** | &nbsp; - beta &nbsp; onPremisesSamAccountName <br> &nbsp; - v1.0 &nbsp; onPremisesSamAccountName |  |
| **provisioningErrors** | &nbsp; - beta &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_ | 此属性及其信息已被弃用。  但是，可以在**onPremisesProvisioningErrors**中找到描述任何 AD Connect 相关设置错误的新属性。 |

## <a name="application-property-differences"></a>应用程序属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **acceptMappedClaims**  | &nbsp; -beta &nbsp; **api/acceptMappedClaims** <br> v1.0 api **/acceptMappedClaims** &nbsp; - &nbsp; | acceptMappedClaims 现在是新 api 资源的一部分。 |
| **applicationTemplateId** | &nbsp; - beta &nbsp; _尚不可用_ <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **命名** | &nbsp; - beta &nbsp; **signInAudience** <br> &nbsp; **** v1.0 signInAudience &nbsp; - | |
| **errorUrl**| &nbsp; -beta &nbsp;_不可用_ <br> v1.0 1.0 &nbsp; - &nbsp;_不可用_   | 此属性已被弃用。|
| **homepage**| &nbsp; -beta &nbsp; **web/homePageUrl** <br> v1.0 web **/homePageUrl** &nbsp; - &nbsp; | 主页现在是新 web 资源的一部分。|
| **informationalUrls**| &nbsp; -beta &nbsp;**信息** <br> &nbsp; - 1.0 &nbsp;版**信息** | |
| **knownClientApplications**| &nbsp;-beta&nbsp;**api/knownClientApplications** <br> v1.0 api **/knownClientApplications** &nbsp; - &nbsp; | knownClientApplications 现在是新 api 资源的一部分。 |
| **logoutUrl**| &nbsp; -beta &nbsp; **web/logoutUrl** <br> v1.0 web **/logoutUrl** &nbsp; - &nbsp; | logoutUrl 现在是 web 资源的一部分。 |
| **logoUrl**| &nbsp; -beta &nbsp;**信息/logoUrl** <br> v1.0 1.0 &nbsp; - &nbsp; **info/logoUrl** | logoUrl 现在是新的 info 资源的一部分。 |
| **mainLogo**| &nbsp; -beta &nbsp;**徽标** <br> &nbsp; -1.0 &nbsp;版**徽标**   | |
| **oauth2AllowIdTokenImplicitFlow** | &nbsp;-beta&nbsp;**web/implicitGrantSettings/enableIdTokenIssuance**<br>v1.0 web **/implicitGrantSettings/enableIdTokenIssuance** &nbsp; - &nbsp; | 重命名，现在是新的 implicitGrantSettings 资源的一部分。 |
| **oauth2AllowImplicitFlow**| &nbsp;-beta&nbsp;**web/implicitGrantSettings/enableAccessTokenIssuance**<br>v1.0 web **/implicitGrantSettings/enableAccessTokenIssuance** &nbsp; - &nbsp; | 重命名，现在是新的 implicitGrantSettings 资源的一部分。 |
| **oauth2AllowUrlPathMatching**| &nbsp; -beta &nbsp;_不可用_ <br> v1.0 1.0 &nbsp; - &nbsp;_不可用_   | 此属性已被弃用。|
| **oauth2Permissions**| &nbsp;-beta&nbsp;**api/oauth2PermissionScopes**<br> v1.0 api **/oauth2PermissionScopes** &nbsp; - &nbsp; | 重命名，现在是新 api 资源的一部分。 |
| **publicClient**| &nbsp; - beta &nbsp; **isFallbackPublicClient** <br> &nbsp; **** v1.0 isFallbackPublicClient &nbsp; - | 此属性现在具有一个新的&nbsp; - &nbsp;含义，它包含像 redirectUris 这样的公共客户端设置。 现在，使用 isFallbackPublicClient 属性处理一个不能自动确定的特殊情况，来确定应用是否为公用或机密客户端。|
| **recordConsentConditions**| &nbsp; -beta &nbsp;_不可用_ <br> v1.0 1.0 &nbsp; - &nbsp;_不可用_   | 此属性已被弃用。|
| **replyUrls**| &nbsp;-beta&nbsp;**web/redirectUris**、 **publicclient 重命名/redirectUris**<br> &nbsp; **** **** v1.0 web/redirectUris、publicclient 重命名/redirectUris &nbsp; - | 除了重命名，redirectUris 现在也是新的 web 和 Publicclient 重命名资源的一部分。 这样，开发人员就可以使用其 web 和公共客户端的特定 Uri （例如，在桌面设备上安装的应用程序）。 | |
| **samlMetadataUrl**| &nbsp; - beta &nbsp; _尚不可用_  <br> v1.0 尚_不可用_ &nbsp; - &nbsp;  | |
| **serviceEndpoints**|  &nbsp; - beta &nbsp; _不可用_  <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_  | 此属性已弃用，但计划用于 servicePrincipal。|

## <a name="approleassignment-differences"></a>AppRoleAssignment 差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **creationTimestamp** | &nbsp; -beta &nbsp; **creationTimestamp** <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | 这将被重命名为 createdDateTime。|
| **id** | &nbsp; -beta &nbsp; **appRoleId** <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |

## <a name="contact-property-differences"></a>联系人属性差异

Azure AD Graph 联系人资源已重命名为 Microsoft Graph 中的 orgContact。  属性差异如下所示：

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **城市** | &nbsp;-beta&nbsp;**地址（城市）** <br> v1.0 地址 **（城市）** &nbsp; - &nbsp;  | City 属性是 "地址" 资源集合的一部分。 |
| **country** | &nbsp;-beta&nbsp;**** 地址&nbsp;**（countryOrRegion）**<br> &nbsp;-1.0&nbsp;**** 版地址&nbsp;**（countryOrRegion）**  | CountryOrRegion 属性是 "地址" 资源集合的一部分。 |
| **dirSyncEnabled** | &nbsp; -beta &nbsp; **onPremisesSyncEnabled** <br> &nbsp; **** v1.0 onPremisesSyncEnabled &nbsp; -   | |
| **facsimileTelephoneNumber** | &nbsp;-beta&nbsp;**** 手机&nbsp;**（businessFax）** <br> &nbsp;&nbsp; **** v1.0 电话 **（businessFax** ） - &nbsp; | 现在是电话集合的一部分，它支持移动、商业和 businessFax。 |
| **physicalDeliveryOfficeName** | &nbsp; -beta &nbsp; **officeLocation** <br> &nbsp; **** v1.0 officeLocation &nbsp; - | |
| **postalCode** | &nbsp;-beta&nbsp;**** 地址&nbsp;**（邮政编码）**<br> &nbsp; -1.0 &nbsp; **** 版地址&nbsp;**（邮政编码）** | "邮政编码" 属性是 "地址" 资源集合的一部分。 |
| **provisioningErrors** | &nbsp; - beta &nbsp;不可用 <br> v1.0 1.0 &nbsp; - &nbsp;不可用 | 此属性及其信息已被弃用。  但是，可以在**onPremisesProvisioningErrors**中找到描述任何 AD Connect 相关设置错误的新属性。 目前仅在 beta 版中提供此功能。 |
| **sipProxyAddress** |  &nbsp; -beta &nbsp; **imAddresses**<br> &nbsp; **** v1.0 imAddresses &nbsp; -  | |
| **state** | &nbsp; -beta &nbsp; **** 地址&nbsp;**（状态）**<br> &nbsp; - 1.0 &nbsp; **** 版地址&nbsp;**（状态）**  | State 属性是 "addresses" 资源集合的一部分。 |
| **streetAddress** | &nbsp; -beta &nbsp; **** 地址&nbsp;**（街道）**<br> &nbsp;&nbsp; **** v1.0 地址 **（街道**） - &nbsp;  | "街道" 属性是 "地址" 资源集合的一部分。 |
| **telephoneNumber** | &nbsp;-beta&nbsp;**** 手机&nbsp;**（业务）** <br> &nbsp;&nbsp; **** v1.0 电话 **（企业版）** - &nbsp; | 现在是电话集合的一部分，它支持移动、商业和 businessFax。 |
| **thumbnailPhoto** | &nbsp; -beta &nbsp;_尚&nbsp;不可用&nbsp;_&nbsp;<br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |

## <a name="contract-property-differences"></a>协定属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **customerContextId** | &nbsp; -beta &nbsp; **customerId** <br> &nbsp; **** v1.0 customerId &nbsp; -  |  |

## <a name="device-property-differences"></a>设备属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **approximateLastLogonTimestamp** | &nbsp;-beta&nbsp;**approximateLastSignInDateTime** <br> &nbsp; **** v1.0 approximateLastSignInDateTime &nbsp; - |  |
| **complianceExpiryTime** | &nbsp;-beta&nbsp;**complianceExpirationDateTime** <br> &nbsp; **** v1.0 complianceExpirationDateTime &nbsp; - |  |
| **deviceObjectVersion** |  &nbsp;-beta&nbsp;**deviceVersion** <br> &nbsp; **** v1.0 deviceVersion &nbsp; - |  |
| **deviceOSType** | &nbsp;-beta&nbsp;**操作系统** <br> &nbsp; - 1.0 &nbsp;版**操作系统** |  |
| **deviceOSVersion** | &nbsp;-beta&nbsp;**operatingSystemVersion** <br> &nbsp; **** v1.0 operatingSystemVersion &nbsp; - |  |
| **devicePhysicalIds** | &nbsp;-beta&nbsp;**physicalIds** <br> &nbsp; **** v1.0 physicalIds &nbsp; - |  |
| **deviceTrustType** | &nbsp;-beta&nbsp;**trustType** <br> &nbsp; **** v1.0 trustType &nbsp; - |  |
| **dirSyncEnabled** |  &nbsp;-beta&nbsp;**onPremisesSyncEnabled** <br> &nbsp; **** v1.0 onPremisesSyncEnabled &nbsp; - |  |
| **lastDirSyncTime** |  &nbsp;-beta&nbsp;**onPremisesLastSyncDateTime** <br> &nbsp; **** v1.0 onPremisesLastSyncDateTime &nbsp; - |  |

## <a name="directoryobjectreference-property-differences"></a>DirectoryObjectReference 属性差异

Azure AD Graph directoryObjectReference 资源已重命名为 Microsoft Graph 中的 directoryObjectPartnerReference。  属性差异如下所示：

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **externalContextId** | &nbsp;-beta&nbsp;**externalPartnerTenantId** <br> &nbsp; **** v1.0 externalPartnerTenantId &nbsp; - |  |

## <a name="domain-property-differences"></a>域属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **name** | &nbsp;-beta&nbsp;**id** <br> &nbsp; - 1.0 &nbsp;版**id** | 在 Microsoft Graph 中，唯一标识符（id）包含域名称;`name`属性不存在。 |
| **forceDeleteState** |  &nbsp;-beta&nbsp;**状态** <br> &nbsp; - 1.0 &nbsp;版**状态** | 在 Azure AD Graph 中，存在单独的 forceDelete 和域状态属性。  在 Microsoft Graph 中，所有域的状态都由 state 属性处理。 |
| **isDefaultForCloudRedirections** | &nbsp;-beta&nbsp;_尚&nbsp;不可用&nbsp;_&nbsp;<br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |

## <a name="oauth2permissionsgrant-property-differences"></a>OAuth2PermissionsGrant 属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **expiryTime** | &nbsp;-beta&nbsp;**expiryTime** <br> &nbsp;_v1.0 尚&nbsp;不可用&nbsp;_ &nbsp;- | 此属性不使用，并且可能会在 Microsoft Graph 中被删除。 |
| **startTime** | beta&nbsp;-&nbsp;版**startTime** <br> &nbsp;_v1.0 尚&nbsp;不可用&nbsp;_ &nbsp;-  | 此属性不使用，并且可能会在 Microsoft Graph 中被删除。 |

## <a name="policy-property-differences"></a>策略属性差异

在 Microsoft Graph 中，有命名的策略类型（如 tokenIssuancePolicy 或 tokenLifetimePolicy），而不是通用策略资源类型。 [策略概述](/graph/api/resources/policy-overview?view=graph-rest-beta)中提供了更多详细信息。 在1.0 版中，策略尚不可用。

## <a name="serviceendpoint-property-differences"></a>ServiceEndpoint 属性差异

Azure AD Graph ServiceEndpoint 资源已重命名为 Microsoft Graph 中的终结点。

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **性能** | &nbsp;-beta&nbsp;**功能**<br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **serviceId** | &nbsp;-beta&nbsp;**providerId**<br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **serviceName** | &nbsp;-beta&nbsp;**providerName**<br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **resourceId** | &nbsp;-beta&nbsp;**providerResourceId**<br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **url** | &nbsp;-beta&nbsp;**uri**<br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |

## <a name="serviceprincipal-property-differences"></a>ServicePrincipal 属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **applicationTemplateId** | &nbsp; - beta &nbsp; _尚不可用_ <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **appOwnerTenantId** | &nbsp;-beta&nbsp;**appOwnerOrganizationId** <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **informationalUrls**| &nbsp;-beta&nbsp;_尚不可用_ <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **preferredSingleSignOnMode** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **preferredTokenSigningKeyEndDateTime** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **samlSingleSignOnSettings** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **servicePrincipalType** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **signInAudience** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **tokenEncryptionKeyId** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |
| **serviceEndpoints** | &nbsp;-beta&nbsp;_尚不可用_ <br> v1.0 尚_不可用_ &nbsp; - &nbsp; | |

## <a name="tenantdetails-property-differences"></a>TenantDetails 属性差异

在 Microsoft Graph 中，Azure AD Graph TenantDetails 资源被重命名为 "组织"。  属性差异如下所示：

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **companyLastDirSyncTime** | &nbsp;-beta&nbsp;**onPremisesLastSyncDateTime** <br> &nbsp;**** v1.0 onPremisesLastSyncDateTime&nbsp;- |  |
| **dirSyncEnabled** | &nbsp;-beta&nbsp;**onPremisesSyncEnabled** <br> &nbsp; **** v1.0 onPremisesSyncEnabled &nbsp; - |  |
| **provisioningErrors** | &nbsp;-beta&nbsp;_不可用_ <br> v1.0 1.0&nbsp;-&nbsp;_不可用_ | 此属性及其信息已被弃用。|
| **telephoneNumber** | &nbsp;-beta&nbsp;**businessPhones** <br> &nbsp;**** v1.0 businessPhones&nbsp;- |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>TrustedCasForPasswordlessAuth 属性差异

Azure AD Graph TrustedCasForPasswordlessAuth 资源已重命名为[certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration?view=graph-rest-beta)，并且仅在 Microsoft Graph beta 终结点中可用。 没有属性差异;但是， **certificateAuthorities**属性使用的**certificateAuthority**资源类型存在差异。

### <a name="certificateauthorityinformation"></a>CertificateAuthorityInformation

将 Azure AD Graph CertificateAuthorityInformation 重命名为 Microsoft Graph 中的**certificateAuthority** 。 属性差异如下所示。

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **authorityType** | &nbsp;-beta&nbsp;**isRootAuthority**<br> &nbsp; **** v1.0 isRootAuthority &nbsp; - | 此属性的类型也已更改为布尔值。 之前，必须将此属性设置为 "RootAuthority" 或 "IntermediateAuthority"。 将 new 属性设置为**true**等效于 "RootAuthority"。 |
| **crlDistributionPoint** | &nbsp;-beta&nbsp;**certificateRevocationListUrl** <br> &nbsp;**** v1.0 certificateRevocationListUrl&nbsp;- | |
| **deltaCrlDistributionPoint** | &nbsp;-beta&nbsp;**deltaCertificateRevocationListUrl** <br> &nbsp;**** v1.0 deltaCertificateRevocationListUrl&nbsp;- | |
| **trustedCertificate** | 试用&nbsp;-&nbsp;版**证书** <br> &nbsp;**** v1.0 deltaCertificateRevocationListUrl&nbsp;- | |
| **trustedIssuer** | &nbsp;-beta&nbsp;**颁发者**<br> &nbsp;**** v1.0&nbsp;- | |
| **trustedIssuerSki** | &nbsp;-beta&nbsp;**issuerSki**<br> &nbsp; **** v1.0 issuerSki &nbsp; - | |

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Graph 与 Microsoft Graph 之间的[方法差异](migrate-azure-ad-graph-method-differences.md)。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
