---
title: Azure AD Graph 与 Microsoft Graph 之间的属性差异
description: 介绍了 Azure AD Graph 资源（实体）与 Microsoft Graph 之间的属性差异，以便帮助您相应地迁移应用。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6ce8cda894006830db456e30f1809d66ccc24025
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863864"
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
| **deletedTimestamp**| beta &nbsp; - &nbsp; **deletedDateTime** <br> v1.0 &nbsp; - &nbsp; **deletedDateTime** | |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | beta &nbsp; - &nbsp; **faxNumber** <br> v1.0 &nbsp; - &nbsp; **faxNumber** | |
| **immutableId** | beta &nbsp; - &nbsp; **onPremisesImmutableId** <br> v1.0 &nbsp; - &nbsp; **onPremisesImmutableId**  | |
| **isCompromised** | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_ | Microsoft Graph[标识保护](/graph/api/resources/identityprotection-root?view=graph-rest-beta)API 提供了更复杂的功能。 |
| **lastDirSyncDateTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **mobile** | beta &nbsp; - &nbsp; **mobilePhone** <br> v1.0 &nbsp; - &nbsp; **mobilePhone** | |
| **provisioningErrors** | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_ | 此属性及其信息已被弃用。  但是，可以在**onPremisesProvisioningErrors**中找到描述任何 AD Connect 相关设置错误的新属性。 |
| **refreshTokensValidFromDateTime** | beta &nbsp; - &nbsp; **signinSessionsValidFromDateTime**<br>v1.0 &nbsp; - &nbsp; **signinSessionsValidFromDateTime** | |
| **signinNames** | beta &nbsp; - &nbsp; **标识/signInType** <br> 1.0 版 &nbsp; - &nbsp; **标识/signInType** | 此属性现在是[objectIdentity](/graph/api/resources/objectIdentity?view=graph-rest-1.0)资源的一部分。|
| **telephoneNumber** | beta &nbsp; - &nbsp; **businessPhones** <br> v1.0 &nbsp; - &nbsp; **businessPhones** | |
| **thumbnailPhoto** | beta &nbsp; - &nbsp; **照片**、照片 <br> v1.0 &nbsp; - &nbsp; **照片**，照片 | Azure AD 缩略图照片在 Microsoft Graph 中不可用。  改为使用[照片 API](/graph/api/resources/profilephoto?view=graph-rest-1.0) 。 |
| **userIdentities** | beta &nbsp; - &nbsp; **标识** <br> 1.0 版 &nbsp; - &nbsp; **标识** | 有关更多详细信息，请参阅[objectIdentity](/graph/api/resources/objectIdentity?view=graph-rest-1.0)资源类型。|
| **userState** | beta &nbsp; - &nbsp; **externalUserState** <br> v1.0 &nbsp; - &nbsp; **externalUserState** | |
| **userStateChangedOn** | beta &nbsp; - &nbsp; **externalUserStateChangeDateTime**<br>v1.0 &nbsp; - &nbsp; **externalUserStateChangeDateTime** | |

## <a name="group-property-differences"></a>组属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **immutableId** | beta &nbsp; - &nbsp; **onPremisesImmutableId** <br> v1.0 &nbsp; - &nbsp; **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime**<br>v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **provisioningErrors** | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_ | 此属性及其信息已被弃用。  但是，可以在**onPremisesProvisioningErrors**中找到描述任何 AD Connect 相关设置错误的新属性。 |

## <a name="application-property-differences"></a>应用程序属性差异

| Azure AD Graph <br>（v 1.6）属性 | Microsoft Graph<br> property                                                                                                                          | 备注                                                                                                                                                                                                                                                                                                                     |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **acceptMappedClaims**             | beta &nbsp; - &nbsp; **api/acceptMappedClaims** <br> v1.0 &nbsp; - &nbsp; **api/acceptMappedClaims**                                                       | acceptMappedClaims 现在是新 api 资源的一部分。                                                                                                                                                                                                                                                                      |
| **命名**        | beta &nbsp; - &nbsp; **signInAudience** <br> v1.0 &nbsp; - &nbsp; **signInAudience**                                                                      |                                                                                                                                                                                                                                                                                                                              |
| **errorUrl**                       | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_                                                                              | 此属性已被弃用。                                                                                                                                                                                                                                                                                                 |
| **首页**                       | beta &nbsp; - &nbsp; **web/homePageUrl** <br> v1.0 &nbsp; - &nbsp; **web/homePageUrl**                                                                     | 主页现在是新 web 资源的一部分。                                                                                                                                                                                                                                                                                |
| **informationalUrls**              | beta &nbsp; - &nbsp; **信息** <br> 1.0 版 &nbsp; - &nbsp; **信息**                                                                                           |                                                                                                                                                                                                                                                                                                                              |
| **knownClientApplications**        | beta &nbsp; - &nbsp; **api/knownClientApplications** <br> v1.0 &nbsp; - &nbsp; **api/knownClientApplications**                                               | knownClientApplications 现在是新 api 资源的一部分。                                                                                                                                                                                                                                                                 |
| **logoutUrl**                      | beta &nbsp; - &nbsp; **web/logoutUrl** <br> v1.0 &nbsp; - &nbsp; **web/logoutUrl**                                                                         | logoutUrl 现在是 web 资源的一部分。                                                                                                                                                                                                                                                                                   |
| **logoUrl**                        | beta &nbsp; - &nbsp; **信息/logoUrl** <br> v1.0 1.0 &nbsp; - &nbsp; **info/logoUrl**                                                                           | logoUrl 现在是新的 info 资源的一部分。                                                                                                                                                                                                                                                                                |
| **mainLogo**                       | beta &nbsp; - &nbsp; **徽标** <br> 1.0 版 &nbsp; - &nbsp; **徽标**                                                                                            |                                                                                                                                                                                                                                                                                                                              |
| **oauth2AllowIdTokenImplicitFlow** | beta &nbsp; - &nbsp; **web/implicitGrantSettings/enableIdTokenIssuance**<br>v1.0 &nbsp; - &nbsp; **web/implicitGrantSettings/enableIdTokenIssuance**         | 重命名，现在是新的 implicitGrantSettings 资源的一部分。                                                                                                                                                                                                                                                             |
| **oauth2AllowImplicitFlow**        | beta &nbsp; - &nbsp; **web/implicitGrantSettings/enableAccessTokenIssuance**<br>v1.0 &nbsp; - &nbsp; **web/implicitGrantSettings/enableAccessTokenIssuance** | 重命名，现在是新的 implicitGrantSettings 资源的一部分。                                                                                                                                                                                                                                                             |
| **oauth2AllowUrlPathMatching**     | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_                                                                              | 此属性已被弃用。                                                                                                                                                                                                                                                                                                 |
| **oauth2Permissions**              | beta &nbsp; - &nbsp; **api/oauth2PermissionScopes**<br> v1.0 &nbsp; - &nbsp; **api/oauth2PermissionScopes**                                                  | 重命名，现在是新 api 资源的一部分。                                                                                                                                                                                                                                                                                |
| **publicClient**                   | beta &nbsp; - &nbsp; **isFallbackPublicClient** <br> v1.0 &nbsp; - &nbsp; **isFallbackPublicClient**                                                      | 此属性现在具有一个新的含义， &nbsp; - &nbsp; 它包含像 redirectUris 这样的公共客户端设置。 现在，使用 isFallbackPublicClient 属性处理一个不能自动确定的特殊情况，来确定应用是否为公用或机密客户端。 |
| **recordConsentConditions**        | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_                                                                              | 此属性已被弃用。                                                                                                                                                                                                                                                                                                 |
| **replyUrls**                      | beta &nbsp; - &nbsp; **web/redirectUris**、 **publicclient 重命名/redirectUris**<br> v1.0 &nbsp; - &nbsp; **web/redirectUris**、 **publicclient 重命名/redirectUris**        | 除了重命名，redirectUris 现在也是新的 web 和 Publicclient 重命名资源的一部分。 这样，开发人员就可以使用其 web 和公共客户端的特定 Uri （例如，在桌面设备上安装的应用程序）。                                                                                           |
| **samlMetadataUrl**                | beta &nbsp; - &nbsp; _尚不可用_  <br> v1.0 &nbsp; - &nbsp; _尚不可用_                                                                  |                                                                                                                                                                                                                                                                                                                              |
| **serviceEndpoints**               | beta &nbsp; - &nbsp; _不可用_  <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_                                                                          | 此属性已弃用，但计划用于 servicePrincipal。                                                                                                                                                                                                                                                            |

## <a name="approleassignment-differences"></a>AppRoleAssignment 差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **creationTimestamp** | beta &nbsp; - &nbsp; **creationTimestamp** <br> v1.0 &nbsp; - &nbsp; **createdDateTime** | |
| **id** | beta &nbsp; - &nbsp; **appRoleId** <br> v1.0 &nbsp; - &nbsp; **appRoleId** | |

## <a name="contact-property-differences"></a>联系人属性差异

Azure AD Graph 联系人资源已重命名为 Microsoft Graph 中的 orgContact。  属性差异如下所示：

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **城市** | beta &nbsp; - &nbsp; **地址（城市）** <br> v1.0 &nbsp; - &nbsp; **地址（城市）**  | City 属性是 "地址" 资源集合的一部分。 |
| **家** | beta &nbsp; - &nbsp; **地址** &nbsp; **（countryOrRegion）**<br> 1.0 版 &nbsp; - &nbsp; **地址** &nbsp; **（countryOrRegion）**  | CountryOrRegion 属性是 "地址" 资源集合的一部分。 |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled**   | |
| **facsimileTelephoneNumber** | beta &nbsp; - &nbsp; **手机** &nbsp; **（businessFax）** <br> v1.0 &nbsp; - &nbsp; **电话** &nbsp; **（businessFax）** | 现在是电话集合的一部分，它支持移动、商业和 businessFax。 |
| **physicalDeliveryOfficeName** | beta &nbsp; - &nbsp; **officeLocation** <br> v1.0 &nbsp; - &nbsp; **officeLocation** | |
| **postalCode** | beta &nbsp; - &nbsp; **地址** &nbsp; **（邮政编码）**<br> 1.0 版 &nbsp; - &nbsp; **地址** &nbsp; **（邮政编码）** | "邮政编码" 属性是 "地址" 资源集合的一部分。 |
| **provisioningErrors** | beta &nbsp; - &nbsp; 不可用 <br> v1.0 1.0 &nbsp; - &nbsp; 不可用 | 此属性及其信息已被弃用。  但是，可以在**onPremisesProvisioningErrors**中找到描述任何 AD Connect 相关设置错误的新属性。 目前仅在 beta 版中提供此功能。 |
| **sipProxyAddress** |  beta &nbsp; - &nbsp; **imAddresses**<br> v1.0 &nbsp; - &nbsp; **imAddresses**  | |
| **state** | beta &nbsp; - &nbsp; **地址** &nbsp; **（状态）**<br> 1.0 版 &nbsp; - &nbsp; **地址** &nbsp; **（状态）**  | State 属性是 "addresses" 资源集合的一部分。 |
| **streetAddress** | beta &nbsp; - &nbsp; **地址** &nbsp; **（街道）**<br> v1.0 &nbsp; - &nbsp; **地址** &nbsp; **（街道）**  | "街道" 属性是 "地址" 资源集合的一部分。 |
| **telephoneNumber** | beta &nbsp; - &nbsp; **手机** &nbsp; **（业务）** <br> v1.0 &nbsp; - &nbsp; **电话** &nbsp; **（企业版）** | 现在是电话集合的一部分，它支持移动、商业和 businessFax。 |
| **thumbnailPhoto** | beta &nbsp; - &nbsp; _ &nbsp; 尚 &nbsp; 不可用_&nbsp;<br> v1.0 &nbsp; - &nbsp; _尚不可用_ | |

## <a name="contract-property-differences"></a>协定属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **customerContextId** | beta &nbsp; - &nbsp; **customerId** <br> v1.0 &nbsp; - &nbsp; **customerId**  |  |

## <a name="device-property-differences"></a>设备属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **approximateLastLogonTimestamp** | beta &nbsp; - &nbsp; **approximateLastSignInDateTime** <br> v1.0 &nbsp; - &nbsp; **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | beta &nbsp; - &nbsp; **complianceExpirationDateTime** <br> v1.0 &nbsp; - &nbsp; **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  beta &nbsp; - &nbsp; **deviceVersion** <br> v1.0 &nbsp; - &nbsp; **deviceVersion** |  |
| **deviceOSType** | beta &nbsp; - &nbsp; **操作系统** <br> 1.0 版 &nbsp; - &nbsp; **操作系统** |  |
| **deviceOSVersion** | beta &nbsp; - &nbsp; **operatingSystemVersion** <br> v1.0 &nbsp; - &nbsp; **operatingSystemVersion** |  |
| **devicePhysicalIds** | beta &nbsp; - &nbsp; **physicalIds** <br> v1.0 &nbsp; - &nbsp; **physicalIds** |  |
| **deviceTrustType** | beta &nbsp; - &nbsp; **trustType** <br> v1.0 &nbsp; - &nbsp; **trustType** |  |
| **dirSyncEnabled** |  beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |

## <a name="directoryobjectreference-property-differences"></a>DirectoryObjectReference 属性差异

Azure AD Graph directoryObjectReference 资源已重命名为 Microsoft Graph 中的 directoryObjectPartnerReference。  属性差异如下所示：

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **externalContextId** | beta &nbsp; - &nbsp; **externalPartnerTenantId** <br> v1.0 &nbsp; - &nbsp; **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>域属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **name** | beta &nbsp; - &nbsp; **id** <br> 1.0 版 &nbsp; - &nbsp; **id** | 在 Microsoft Graph 中，唯一标识符（id）包含域名称;`name`属性不存在。 |
| **forceDeleteState** |  beta &nbsp; - &nbsp; **状态** <br> 1.0 版 &nbsp; - &nbsp; **状态** | 在 Azure AD Graph 中，存在单独的 forceDelete 和域状态属性。  在 Microsoft Graph 中，所有域的状态都由 state 属性处理。 |
| **isDefaultForCloudRedirections** | beta &nbsp; - &nbsp; _ &nbsp; 尚 &nbsp; 不可用_&nbsp;<br> v1.0 &nbsp; - &nbsp; _尚不可用_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>OAuth2PermissionsGrant 属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **expiryTime** | beta &nbsp; - &nbsp; **expiryTime** <br> 1.0 版 &nbsp; - &nbsp; _已删除_ | 此属性不使用，在 Microsoft Graph v1.0 中将被删除。 |
| **startTime** | beta 版 &nbsp; - &nbsp; **startTime** <br> 1.0 版 &nbsp; - &nbsp; _已删除_  | 此属性不使用，在 Microsoft Graph v1.0 中将被删除。 |

## <a name="policy-property-differences"></a>策略属性差异

在 Microsoft Graph 中，有命名的策略类型（如 tokenIssuancePolicy 或 tokenLifetimePolicy），而不是通用策略资源类型。 [策略概述](/graph/api/resources/policy-overview?view=graph-rest-1.0)中提供了更多详细信息。

## <a name="serviceendpoint-property-differences"></a>ServiceEndpoint 属性差异

Azure AD Graph ServiceEndpoint 资源已重命名为 Microsoft Graph 中的终结点。

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **serviceId** | beta &nbsp; - &nbsp; **providerId**<br> 1.0 版 &nbsp; - &nbsp; **providerId** | |
| **serviceName** | beta &nbsp; - &nbsp; **providerName**<br> v1.0 1.0 &nbsp; - &nbsp; **providerName** | |
| **resourceId** | beta &nbsp; - &nbsp; **providerResourceId**<br> v1.0 &nbsp; - &nbsp; **providerResourceId** | |

## <a name="serviceprincipal-property-differences"></a>ServicePrincipal 属性差异

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **appOwnerTenantId** | beta &nbsp; - &nbsp; **appOwnerOrganizationId** <br> v1.0 &nbsp; - &nbsp; **appOwnerOrganizationId** | 更名. |
| **informationalUrls**| beta &nbsp; - &nbsp; **信息** <br> 1.0 版 &nbsp; - &nbsp; **信息** | |
| **oauth2Permissions** | beta &nbsp; - &nbsp; **publishedPermissionScopes** <br> v1.0 &nbsp; - &nbsp; **oauth2PermissionScopes** | 更名. |
| **preferredTokenSigningKeyEndDateTime** | beta &nbsp; - &nbsp; _尚不可用_ <br> v1.0 &nbsp; -  _尚不可用_ | |
| **signInAudience** | beta &nbsp; - &nbsp; _尚不可用_ <br> v1.0 &nbsp; -  _尚不可用_ | |
| **serviceEndpoints** | beta &nbsp; - &nbsp; **终结点** <br> v1.0 &nbsp; - &nbsp; **终结点** | 更名. |

## <a name="tenantdetails-property-differences"></a>TenantDetails 属性差异

在 Microsoft Graph 中，Azure AD Graph TenantDetails 资源被重命名为 "组织"。  属性差异如下所示：

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **companyLastDirSyncTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **provisioningErrors** | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_ | 此属性及其信息已被弃用。|
| **telephoneNumber** | beta &nbsp; - &nbsp; **businessPhones** <br> v1.0 &nbsp; - &nbsp; **businessPhones** |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>TrustedCasForPasswordlessAuth 属性差异

Azure AD Graph TrustedCasForPasswordlessAuth 资源已重命名为[certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration?view=graph-rest-beta)，并且仅在 Microsoft Graph beta 终结点中可用。 没有属性差异;但是， **certificateAuthorities**属性使用的**certificateAuthority**资源类型存在差异。

### <a name="certificateauthorityinformation"></a>CertificateAuthorityInformation

将 Azure AD Graph CertificateAuthorityInformation 重命名为 Microsoft Graph 中的**certificateAuthority** 。 属性差异如下所示。

|Azure AD Graph <br>（v 1.6）属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **authorityType** | beta &nbsp; - &nbsp; **isRootAuthority**<br> v1.0 &nbsp; - &nbsp; **isRootAuthority** | 此属性的类型也已更改为布尔值。 之前，必须将此属性设置为 "RootAuthority" 或 "IntermediateAuthority"。 将 new 属性设置为**true**等效于 "RootAuthority"。 |
| **crlDistributionPoint** | beta &nbsp; - &nbsp; **certificateRevocationListUrl** <br> v1.0 &nbsp; - &nbsp; **certificateRevocationListUrl** | |
| **deltaCrlDistributionPoint** | beta &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** <br> v1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedCertificate** | 试用版 &nbsp; - &nbsp; **证书** <br> v1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedIssuer** | beta &nbsp; - &nbsp; **颁发者**<br> v1.0 &nbsp; - &nbsp; **颁发者** | |
| **trustedIssuerSki** | beta &nbsp; - &nbsp; **issuerSki**<br> v1.0 &nbsp; - &nbsp; **issuerSki** | |

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Graph 与 Microsoft Graph 之间的[方法差异](migrate-azure-ad-graph-method-differences.md)。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
