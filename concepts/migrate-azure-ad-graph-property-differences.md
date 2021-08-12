---
title: Azure AD Graph 和 Microsoft Graph
description: 介绍 Azure AD Graph实体 (Azure AD) 和 Microsoft Graph 之间的属性差异，以帮助相应地迁移应用。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: f49bd3382af0f16999b89cb67b582027b2f24c7c67f31763fe6b5c91df86046a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205170"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph 和 Microsoft Graph

本文是步骤 *1：查看迁移应用的* 过程的 API [差异的一部分](migrate-azure-ad-graph-planning-checklist.md)。

通常，将 Azure AD Graph API 与 Microsoft Graph 进行对比的最佳方法就是比较每个服务的基础元数据，尤其是资源说明：

- [Azure AD Graph元数据](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Microsoft Graph beta 元数据](https://graph.microsoft.com/beta/$metadata)
- [Microsoft Graph v1.0 元数据](https://graph.microsoft.com/v1.0/$metadata)

此处突出显示了资源之间的属性差异。 如果属性未在此列表中显示，则它已在[v1.0](/graph/api/overview)版本的 Microsoft Graph 中可用，其名称与 Azure AD Graph。

由于用户和组使用得非常频繁，因此这些资源首先出现。  其他资源按字母顺序显示。

## <a name="user-property-differences"></a>用户属性差异

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br>property|备注|
|---|---|---|
| **deletedTimestamp**| beta &nbsp; - &nbsp; **deletedDateTime** <br> v1.0 &nbsp; - &nbsp; **deletedDateTime** | |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | beta &nbsp; - &nbsp; **faxNumber** <br> v1.0 &nbsp; - &nbsp; **faxNumber** | |
| **immutableId** | beta &nbsp; - &nbsp; **onPremisesImmutableId** <br> v1.0 &nbsp; - &nbsp; **onPremisesImmutableId**  | |
| **isComprom一** | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; _不可用_ | Microsoft Graph[标识保护](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true)API 提供了更复杂的功能。 |
| **lastDirSyncDateTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **mobile** | beta &nbsp; - &nbsp; **mobilePhone** <br> v1.0 &nbsp; - &nbsp; **mobilePhone** | |
| **provisioningErrors** | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; _不可用_ | 此属性及其信息已弃用。  但是，可以在 **onPremisesProvisioningErrors** 连接描述任何 AD 或相关设置错误的新属性 |
| **refreshTokensValidFromDateTime** | beta &nbsp; - &nbsp; **signinSessionsValidFromDateTime**<br>v1.0 &nbsp; - &nbsp; **signinSessionsValidFromDateTime** | |
| **signinNames** | beta &nbsp; - &nbsp; **标识/signInType** <br> v1.0 &nbsp; - &nbsp; **标识/signInType** | 此属性现在是 [objectIdentity 资源的一](/graph/api/resources/objectIdentity) 部分。|
| **telephoneNumber** | beta &nbsp; - &nbsp; **businessPhones** <br> v1.0 &nbsp; - &nbsp; **businessPhones** | |
| **thumbnailPhoto** | beta &nbsp; - &nbsp; **照片**， 照片 <br> v1.0 &nbsp; - &nbsp; **照片**， 照片 | Azure AD 缩略图照片无法通过 Microsoft Graph。  请[改为使用照片 API。](/graph/api/resources/profilephoto) |
| **userIdentities** | beta &nbsp; - &nbsp; **标识** <br> v1.0 &nbsp; - &nbsp; **标识** | 有关详细信息 [，请参阅 objectIdentity](/graph/api/resources/objectIdentity) 资源类型。|
| **userState** | beta &nbsp; - &nbsp; **externalUserState** <br> v1.0 &nbsp; - &nbsp; **externalUserState** | |
| **userStateChangedOn** | beta &nbsp; - &nbsp; **externalUserStateChangeDateTime**<br>v1.0 &nbsp; - &nbsp; **externalUserStateChangeDateTime** | |

## <a name="group-property-differences"></a>组属性差异

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** | |
| **immutableId** | beta &nbsp; - &nbsp; **onPremisesImmutableId** <br> v1.0 &nbsp; - &nbsp; **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime**<br>v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** | |
| **provisioningErrors** | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; _不可用_ | 此属性及其信息已弃用。  但是，可以在 **onPremisesProvisioningErrors** 连接描述任何 AD 或相关设置错误的新属性 |

## <a name="application-property-differences"></a>应用程序属性差异

| Azure AD Graph <br> (v1.6) 属性 | Microsoft Graph<br> property                                                                                                                          | 备注                                                                                                                                                                                                                                                                                                                     |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **acceptMappedClaims**             | beta &nbsp; - &nbsp; **api/acceptMappedClaims** <br> v1.0 &nbsp; - &nbsp; **api/acceptMappedClaims**                                                       | acceptMappedClaims 现在是新 api 资源的一部分。                                                                                                                                                                                                                                                                      |
| **availableToOtherTenants**        | beta &nbsp; - &nbsp; **signInAudience** <br> v1.0 &nbsp; - &nbsp; **signInAudience**                                                                      |                                                                                                                                                                                                                                                                                                                              |
| **errorUrl**                       | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; _不可用_                                                                              | 此属性已弃用。                                                                                                                                                                                                                                                                                                 |
| **homepage**                       | beta &nbsp; - &nbsp; **web/homePageUrl** <br> v1.0 &nbsp; - &nbsp; **web/homePageUrl**                                                                     | homepage 现在是新 Web 资源的一部分。                                                                                                                                                                                                                                                                                |
| **informationalUrls**              | beta &nbsp; - &nbsp; **信息** <br> v1.0 &nbsp; - &nbsp; **信息**                                                                                           |                                                                                                                                                                                                                                                                                                                              |
| **knownClientApplications**        | beta &nbsp; - &nbsp; **api/knownClientApplications** <br> v1.0 &nbsp; - &nbsp; **api/knownClientApplications**                                               | knownClientApplications 现在是新 api 资源的一部分。                                                                                                                                                                                                                                                                 |
| **logoutUrl**                      | beta &nbsp; - &nbsp; **web/logoutUrl** <br> v1.0 &nbsp; - &nbsp; **web/logoutUrl**                                                                         | logoutUrl 现在是 Web 资源的一部分。                                                                                                                                                                                                                                                                                   |
| **logoUrl**                        | beta &nbsp; - &nbsp; **info/logoUrl** <br> v1.0 &nbsp; - &nbsp; **info/logoUrl**                                                                           | logoUrl 现在是新信息资源的一部分。                                                                                                                                                                                                                                                                                |
| **mainLogo**                       | beta &nbsp; - &nbsp; **徽标** <br> v1.0 &nbsp; - &nbsp; **徽标**                                                                                            |                                                                                                                                                                                                                                                                                                                              |
| **oauth2AllowIdTokenImplicitFlow** | beta &nbsp; - &nbsp; **web/implicitGrantSettings/enableIdTokenIssuance**<br>v1.0 &nbsp; - &nbsp; **web/implicitGrantSettings/enableIdTokenIssuance**         | 重命名，现在是新 implicitGrantSettings 资源的一部分。                                                                                                                                                                                                                                                             |
| **oauth2AllowImplicitFlow**        | beta &nbsp; - &nbsp; **web/implicitGrantSettings/enableAccessTokenIssuance**<br>v1.0 &nbsp; - &nbsp; **web/implicitGrantSettings/enableAccessTokenIssuance** | 重命名，现在是新 implicitGrantSettings 资源的一部分。                                                                                                                                                                                                                                                             |
| **oauth2AllowUrlPathMatching**     | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; _不可用_                                                                              | 此属性已弃用。                                                                                                                                                                                                                                                                                                 |
| **oauth2Permissions**              | beta &nbsp; - &nbsp; **api/oauth2PermissionScopes**<br> v1.0 &nbsp; - &nbsp; **api/oauth2PermissionScopes**                                                  | 重命名，现在是新 api 资源的一部分。                                                                                                                                                                                                                                                                                |
| **publicClient**                   | beta &nbsp; - &nbsp; **isFallbackPublicClient** <br> v1.0 &nbsp; - &nbsp; **isFallbackPublicClient**                                                      | 此属性现在具有一个新含义 &nbsp; - &nbsp; ，即它包含 redirectUris 等公共客户端设置。 现在将自动确定应用是公共客户端还是机密客户端，使用 isFallbackPublicClient 属性处理无法自动确定的一个特殊情况。 |
| **recordConsentConditions**        | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; _不可用_                                                                              | 此属性已弃用。                                                                                                                                                                                                                                                                                                 |
| **replyUrls**                      | beta &nbsp; - &nbsp; **web/redirectUris** **、publicClient/redirectUris**<br> v1.0 &nbsp; - &nbsp; **web/redirectUris** **、publicClient/redirectUris**        | 除了重命名，redirectUris 现在是新 Web 和 publicClient 资源的一部分。 这允许开发人员为 Web 和公共客户端使用特定 URI (如桌面设备上已安装的应用程序) 。                                                                                           |
| **samlMetadataUrl**                | beta &nbsp; - &nbsp; _尚不可用_  <br> v1.0 &nbsp; - &nbsp; _尚不可用_                                                                  |                                                                                                                                                                                                                                                                                                                              |
| **serviceEndpoints**               | beta &nbsp; - &nbsp; _不可用_  <br> v1.0 &nbsp; - &nbsp; _不可用_                                                                          | 此属性已弃用，但已针对 servicePrincipal 进行规划。                                                                                                                                                                                                                                                            |

## <a name="approleassignment-differences"></a>AppRoleAssignment 差异

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **creationTimestamp** | beta &nbsp; - &nbsp; **creationTimestamp** <br> v1.0 &nbsp; - &nbsp; **createdDateTime** | |
| **id** | beta &nbsp; - &nbsp; **appRoleId** <br> v1.0 &nbsp; - &nbsp; **appRoleId** | |

## <a name="contact-property-differences"></a>联系人属性差异

Azure AD Graph Contact 资源已重命名为 Microsoft Graph 中的 orgContact。  以下是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **城市** | 城市 &nbsp; - &nbsp; **(beta)** <br> v1.0 &nbsp; - &nbsp; **地址 (城市)**  | city 属性是 addresses 资源集合的一部分。 |
| **country** | &nbsp; - &nbsp;  &nbsp; **countryOrRegion (beta)**<br> v1.0 &nbsp; - &nbsp; **地址** &nbsp; **(countryOrRegion)**  | countryOrRegion 属性是 addresses 资源集合的一部分。 |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled**   | |
| **facsimileTelephoneNumber** | beta &nbsp; - &nbsp; **phones** &nbsp; **(businessFax)** <br> v1.0 &nbsp; - &nbsp; **(** &nbsp; **businessFax)** | 现在是手机集合的一部分，支持移动、业务和 businessFax。 |
| **physicalDeliveryOfficeName** | beta &nbsp; - &nbsp; **officeLocation** <br> v1.0 &nbsp; - &nbsp; **officeLocation** | |
| **postalCode** | &nbsp; - &nbsp;  &nbsp; **postalCode (beta)**<br> v1.0 &nbsp; - &nbsp; **addresses** &nbsp; **(postalCode)** | postalCode 属性是 addresses 资源集合的一部分。 |
| **provisioningErrors** | beta &nbsp; - &nbsp; 不可用 <br> v1.0 &nbsp; - &nbsp; 不可用 | 此属性及其信息已弃用。  但是，可以在 **onPremisesProvisioningErrors** 连接描述任何 AD 或相关设置错误的新属性。 目前，这仅在 beta 版中可用。 |
| **sipProxyAddress** |  beta &nbsp; - &nbsp; **imAddresses**<br> v1.0 &nbsp; - &nbsp; **imAddresses**  | |
| **state** | beta &nbsp; - &nbsp; **addresses** &nbsp; **(state)**<br> v1.0 &nbsp; - &nbsp; **地址** &nbsp; **(状态)**  | state 属性是 addresses 资源集合的一部分。 |
| **streetAddress** | beta &nbsp; - &nbsp; **addresses** &nbsp; **(street)**<br> v1.0 &nbsp; - &nbsp; **地址** &nbsp; **(街道)**  | street 属性是 addresses 资源集合的一部分。 |
| **telephoneNumber** | beta &nbsp; - &nbsp; **phones** &nbsp; **(business)** <br> v1.0 &nbsp; - &nbsp; **电话** &nbsp; **(商业)** | 现在是手机集合的一部分，支持移动、业务和 businessFax。 |
| **thumbnailPhoto** | beta &nbsp; - &nbsp; _&nbsp; 尚 &nbsp; 不可用_&nbsp;<br> v1.0 &nbsp; - &nbsp; _尚不可用_ | |

## <a name="contract-property-differences"></a>合同属性差异

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **customerContextId** | beta &nbsp; - &nbsp; **customerId** <br> v1.0 &nbsp; - &nbsp; **customerId**  |  |

## <a name="device-property-differences"></a>设备属性差异

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **approximateLastLogonTimestamp** | beta &nbsp; - &nbsp; **approximateLastSignInDateTime** <br> v1.0 &nbsp; - &nbsp; **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | beta &nbsp; - &nbsp; **complianceExpirationDateTime** <br> v1.0 &nbsp; - &nbsp; **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  beta &nbsp; - &nbsp; **deviceVersion** <br> v1.0 &nbsp; - &nbsp; **deviceVersion** |  |
| **deviceOSType** | beta &nbsp; - &nbsp; **operatingSystem** <br> v1.0 &nbsp; - &nbsp; **operatingSystem** |  |
| **deviceOSVersion** | beta &nbsp; - &nbsp; **operatingSystemVersion** <br> v1.0 &nbsp; - &nbsp; **operatingSystemVersion** |  |
| **devicePhysicalIds** | beta &nbsp; - &nbsp; **physicalIds** <br> v1.0 &nbsp; - &nbsp; **physicalIds** |  |
| **deviceTrustType** | beta &nbsp; - &nbsp; **trustType** <br> v1.0 &nbsp; - &nbsp; **trustType** |  |
| **dirSyncEnabled** |  beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |

## <a name="directoryobjectreference-property-differences"></a>DirectoryObjectReference 属性差异

Azure AD Graph directoryObjectReference 资源已重命名为 Microsoft Graph 中的 directoryObjectPartnerReference。  以下是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **externalContextId** | beta &nbsp; - &nbsp; **externalPartnerTenantId** <br> v1.0 &nbsp; - &nbsp; **externalPartnerTenantId** |  |

## <a name="domain-property-differences"></a>域属性差异

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **名称** | beta &nbsp; - &nbsp; **id** <br> v1.0 &nbsp; - &nbsp; **id** | 在 Microsoft Graph 中，id (的唯) 包含域名;`name`属性不存在。 |
| **forceDeleteState** |  beta &nbsp; - &nbsp; **状态** <br> v1.0 &nbsp; - &nbsp; **状态** | 在 Azure AD Graph，有单独的 forceDelete 和域状态属性。  在 Microsoft Graph中，所有域状态都由 state 属性处理。 |
| **isDefaultForCloudRedirections** | beta &nbsp; - &nbsp; _&nbsp; 尚 &nbsp; 不可用_&nbsp;<br> v1.0 &nbsp; - &nbsp; _尚不可用_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>OAuth2PermissionsGrant 属性差异

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **expiryTime** | beta &nbsp; - &nbsp; **expiryTime** <br> v1.0 &nbsp; - &nbsp; _已删除_ | 在 Microsoft v1.0 中，不Graph此属性。 |
| **startTime** | beta &nbsp; - &nbsp; **startTime** <br> v1.0 &nbsp; - &nbsp; _已删除_  | 在 Microsoft v1.0 中，不Graph此属性。 |

## <a name="policy-property-differences"></a>策略属性差异

在 Microsoft Graph有一些已命名的策略类型 (如 tokenIssuancePolicy 或 tokenLifetimePolicy) ，而不是通用策略资源类型。 有关更多详细信息，请参阅 [策略概述](/graph/api/resources/policy-overview)。

## <a name="serviceendpoint-property-differences"></a>ServiceEndpoint 属性差异

Azure AD Graph ServiceEndpoint 资源重命名为 Microsoft Graph 中的终结点。

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **服务 Id** | beta &nbsp; - &nbsp; **providerId**<br> v1.0 &nbsp; - &nbsp; **providerId** | |
| **serviceName** | beta &nbsp; - &nbsp; **providerName**<br> v1.0 &nbsp; - &nbsp; **providerName** | |
| **resourceId** | beta &nbsp; - &nbsp; **providerResourceId**<br> v1.0 &nbsp; - &nbsp; **providerResourceId** | |

## <a name="serviceprincipal-property-differences"></a>ServicePrincipal 属性差异

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **appOwnerTenantId** | beta &nbsp; - &nbsp; **appOwnerOrganizationId** <br> v1.0 &nbsp; - &nbsp; **appOwnerOrganizationId** | 重命名。 |
| **informationalUrls**| beta &nbsp; - &nbsp; **信息** <br> v1.0 &nbsp; - &nbsp; **信息** | |
| **oauth2Permissions** | beta &nbsp; - &nbsp; **publishedPermissionScopes** <br> v1.0 &nbsp; - &nbsp; **oauth2PermissionScopes** | 重命名。 |
| **preferredTokenSigningKeyEndDateTime** | beta &nbsp; - &nbsp; _尚不可用_ <br> v1.0 &nbsp; -  _尚不可用_ | |
| **signInAudience** | beta &nbsp; - &nbsp; _尚不可用_ <br> v1.0 &nbsp; -  _尚不可用_ | |
| **serviceEndpoints** | beta &nbsp; - &nbsp; **终结点** <br> v1.0 &nbsp; - &nbsp; **终结点** | 重命名。 |

## <a name="tenantdetails-property-differences"></a>TenantDetails 属性差异

Azure AD Graph TenantDetails 资源在 Microsoft Graph 中重命名为组织。  以下是属性差异：

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **companyLastDirSyncTime** | beta &nbsp; - &nbsp; **onPremisesLastSyncDateTime** <br> v1.0 &nbsp; - &nbsp; **onPremisesLastSyncDateTime** |  |
| **dirSyncEnabled** | beta &nbsp; - &nbsp; **onPremisesSyncEnabled** <br> v1.0 &nbsp; - &nbsp; **onPremisesSyncEnabled** |  |
| **provisioningErrors** | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; _不可用_ | 此属性及其信息已弃用。|
| **telephoneNumber** | beta &nbsp; - &nbsp; **businessPhones** <br> v1.0 &nbsp; - &nbsp; **businessPhones** |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>TrustedCasForPasswordlessAuth 属性差异

Azure AD Graph TrustedCasForPasswordlessAuth 资源已重命名为[certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedauthconfiguration)。 没有属性差异;但是 **，certificateAuthorities** 属性使用的 **certificateAuthority** 资源类型存在差异。

### <a name="certificateauthorityinformation"></a>CertificateAuthorityInformation

Azure AD Graph CertificateAuthorityInformation 在 Microsoft Graph 中重命名为 **certificateAuthority。** 以下是属性差异。

|Azure AD Graph <br> (v1.6) 属性 |Microsoft Graph<br> property|备注|
|---|---|---|
| **authorityType** | beta &nbsp; - &nbsp; **isRootAuthority**<br> v1.0 &nbsp; - &nbsp; **isRootAuthority** | 此属性的类型也已更改为 Boolean。 以前，此属性必须设置为"RootAuthority"或"IntermediateAuthority"。 将新属性设置为 **true** 等效于"RootAuthority"。 |
| **crlDistributionPoint** | beta &nbsp; - &nbsp; **certificateRevocationListUrl** <br> v1.0 &nbsp; - &nbsp; **certificateRevocationListUrl** | |
| **deltaCrlDistributionPoint** | beta &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** <br> v1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedCertificate** | beta &nbsp; - &nbsp; **证书** <br> v1.0 &nbsp; - &nbsp; **deltaCertificateRevocationListUrl** | |
| **trustedIssuer** | beta &nbsp; - &nbsp; **颁发者**<br> v1.0 &nbsp; - &nbsp; **颁发者** | |
| **trustedIssuerSki** | beta &nbsp; - &nbsp; **issuerSki**<br> v1.0 &nbsp; - &nbsp; **issuerSki** | |

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD [Graph](migrate-azure-ad-graph-method-differences.md)和 Microsoft Graph 之间的方法差异。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。

