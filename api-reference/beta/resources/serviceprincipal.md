---
title: servicePrincipal 资源类型
description: 表示目录中的一个应用程序实例。 继承自 directoryObject。
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 8c23a8d87f9f1500e280e5185cd97a70a41fad12
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61321846"
---
# <a name="serviceprincipal-resource-type"></a>servicePrincipal 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示目录中的一个应用程序实例。 继承自 [directoryObject](directoryobject.md)。

该资源支持通过提供 [delta](../api/serviceprincipal-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。 此资源是允许传入其他属性的开放类型。

## <a name="methods"></a>Methods

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[List servicePrincipals](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md) 集合 | 检索 servicePrincipal 对象列表。 |
|[创建 servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md)| [servicePrincipal](serviceprincipal.md) | 创建一个新的 servicePrincipal 对象。 |
|[Get servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |读取 servicePrincipal 对象的属性和关系。|
|[更新 servicePrincipal](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |更新 servicePrincipal 对象。 |
|[删除 servicePrincipal](../api/serviceprincipal-delete.md) | 无 |删除 servicePrincipal 对象。|
|[List createdObjects](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md) 集合| 获取 createdObject 对象集合。|
|[List ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |[directoryObject](directoryobject.md) 集合| 获取 ownedObject 对象集合。|
|[delta](../api/serviceprincipal-delta.md)|servicePrincipal 集合| 获取服务主体的增量更改。 |
|**应用角色分配**| | |
|[列出 appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md) 集合| 获取已分配到此服务主体的应用角色。|
|[添加 appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| 向此服务主体分配一个应用角色。|
|[删除 appRoleAssignment](../api/serviceprincipal-delete-approleassignments.md) | 无 | 从此服务主体中删除一个应用角色分配。|
|[列出 appRoleAssignedTo](../api/serviceprincipal-list-approleassignedto.md) |[appRoleAssignment](approleassignment.md) 集合| 获取用户、组和服务主体为此服务主体分配的应用角色。|
|[添加 appRoleAssignedTo](../api/serviceprincipal-post-approleassignedto.md) |[appRoleAssignment](approleassignment.md)| 向用户、组或服务主体分配此服务主体的应用角色。|
|[移除 appRoleAssignedTo](../api/serviceprincipal-delete-approleassignedto.md) | 无 | 从用户、组或服务主体中移除此服务主体的应用角色分配。|
|**证书和密码**| | |
|[添加密码](../api/serviceprincipal-addpassword.md)|[passwordCredential](passwordcredential.md)|向 servicePrincipal 添加强密码。|
|[添加 tokenSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md)|[selfSignedCertificate](../resources/selfsignedcertificate.md)| 向服务主体添加自签名证书。 主要用于从 Azure AD 库中 [基于 SAML 的 SSO](/azure/active-directory/saas-apps/tutorial-list)。
|[删除密码](../api/serviceprincipal-removepassword.md)|[passwordCredential](passwordcredential.md)|从 servicePrincipal 中移除密码。|
|[加号键](../api/serviceprincipal-addkey.md)|[keyCredential](keycredential.md)|向 servicePrincipal 添加密钥凭据。|
|[删除键](../api/serviceprincipal-removekey.md)|无|从 servicePrincipal 中移除密钥凭据。|
|**委派权限分类**| | |
|[列出委派权限分类](../api/serviceprincipal-list-delegatedpermissionclassifications.md) |[delegatedPermissionClassification](delegatedpermissionclassification.md) 集合| 获取此服务主体公开的委派权限的权限分类。|
|[添加委派权限分类](../api/serviceprincipal-post-delegatedpermissionclassifications.md) |[delegatedPermissionClassification](delegatedpermissionclassification.md) | 添加此服务主体公开的委派权限的权限分类。 |
|[删除委派权限分类](../api/serviceprincipal-delete-delegatedpermissionclassifications.md) | 无 | 删除此服务主体公开的委派权限的权限分类。|
|**委派权限授予**| | |
|[List oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合| 获取授权此服务主体代表已登录用户访问 API 的委派权限授予。|
|**Membership**| | |
|[List memberOf](../api/serviceprincipal-list-memberof.md) |[directoryObject](directoryobject.md) 集合| 从 memberOf 导航属性中获取此服务主体是其直接成员的组。|
|[列出 transitive memberOf](../api/serviceprincipal-list-transitivememberof.md) |[directoryObject](directoryobject.md) 集合| 列出此服务主体所属的组。 此操作是可传递的，并包括此服务主体以嵌套方式所属的组。 |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|String 集合|检查指定组列表中的成员身份。|
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md)|String 集合|检查组、目录角色或管理单元对象指定列表中的成员身份。|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|String 集合|获取此服务主体所属的组列表。|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String collection|获取此服务主体所属的组、管理单元和目录角色的列表。|
|**Owners**| | |
|[List owners](../api/serviceprincipal-list-owners.md) |[directoryObject](directoryobject.md) 集合| 获取所有者对象集合。|
|[添加所有者](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| 通过发布到所有者集合创建新的所有者。|
|[Remove owner](../api/serviceprincipal-delete-owners.md) |无| 从 serviceprincipal 中移除所有者。|
|**策略**| | |
|[分配 claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md)| [claimsMappingPolicy](claimsmappingpolicy.md) 集合| 向此对象分配 claimsMappingPolicy。|
|[列出 claimsMappingPolicies](../api/serviceprincipal-list-claimsmappingpolicies.md)| [claimsMappingPolicy](claimsmappingpolicy.md) 集合| 为此对象分配的 claimsMappingPolicies。|
|[删除 claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md)| [claimsMappingPolicy](claimsmappingpolicy.md) 集合| 从此对象中移除 claimsMappingPolicy。|
|[分配 homeRealmDiscoveryPolicy](../api/serviceprincipal-post-homerealmdiscoverypolicies.md)| [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) 集合| 向此对象分配 homeRealmDiscoveryPolicy。|
|[列出 homeRealmDiscoveryPolicy](../api/serviceprincipal-list-homerealmdiscoverypolicies.md)| [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) 集合| 为此对象分配的 homeRealmDiscoveryPolicies。|
|[删除 homeRealmDiscoveryPolicy](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md)| [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) 集合| 从此对象中删除 homeRealmDiscoveryPolicy。|
|[分配 tokenIssuancePolicy](../api/application-post-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) 集合| 分配 tokenIssuancePolicy 至此对象。|
|[列出 tokenIssuancePolicies](../api/application-list-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) 集合| 获取已分配至此对象的所有 tokenIssuancePolicies。|
|[删除 tokenIssuancePolicy](../api/application-delete-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) 集合| 从此对象中删除 tokenIssuancePolicy。|
|[分配 tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md)| [tokenLifetimePolicy](tokenlifetimepolicy.md) 集合| 向此对象分配 tokenLifetimePolicy。|
|[列出 tokenLifetimePolicies](../api/application-list-tokenlifetimepolicies.md)| [tokenLifetimePolicy](tokenlifetimepolicy.md) 集合| 获取已分配至此对象的所有 tokenLifetimePolicies。|
|[删除 tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md)| [tokenLifetimePolicy](tokenlifetimepolicy.md) 集合| 从此对象中删除 tokenLifetimePolicy。|
|**单一登录**| | |
|[createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|为正文中指定的用户或组创建凭据集。|
|[getPasswordSingleSignOnCredentials](../api/serviceprincipal-getpasswordsinglesignoncredentials.md)|[passwordSingleSignOnCredentialSet](passwordsinglesignoncredentialset.md)|为正文中指定的用户或组获取凭据集。|
|[updatePasswordSingleSignOnCredentials](../api/serviceprincipal-updatepasswordsinglesignoncredentials.md)|无|为正文中指定的用户或组更新凭据集。|
|[deletePasswordSingleSignOnCredentials](../api/serviceprincipal-deletepasswordsinglesignoncredentials.md)|无|删除正文中指定的用户或组的凭据集。|

## <a name="properties"></a>属性

> [!IMPORTANT]
> 仅当使用设置为 `eventual` 和 `$count` 的 **ConsistencyLevel** 标头时，才支持 `$filter` 和 `$search` 查询参数的特定用法。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries#service-principal-properties)。

| 属性     | 类型 |说明|
|:---------------|:--------|:----------|
| accountEnabled |Boolean| 如果已启用服务主体帐户，则为 `true`；否则，为 `false`。 支持 `$filter`（`eq`、`ne`、`not`、`in`）。 |
| addIns | [addIn](addin.md) 集合 | 定义使用服务可用于调用特定上下文中的应用的自定义行为。 例如，呈现文件流的应用程序可能会为其“FileHandler”功能[设置 addIns 属性](/onedrive/developer/file-handlers/)。 这将使 Microsoft 365 之类的服务在用户正在处理的文档上下文中调用应用程序。|
|alternativeNames|字符串集合| 用于按订阅、标识资源组和[托管标识](https://aka.ms/azuremanagedidentity)的完整资源 ID 检索服务主体。 支持 `$filter`（`eq`、`not`、`ge`、`le`、`startsWith`）。|
|应用说明|String|相关应用程序公开的说明。|
|appDisplayName|String|关联应用程序公开的显示名称。|
|appId|String|关联应用程序的唯一标识符（其 **appId** 属性）。 支持 `$filter` （`eq`、 `ne`、 `not`、 `in`、 `startsWith`）。|
|applicationTemplateId|String|创建 servicePrincipal 的 applicationTemplate 的唯一标识符。 只读。 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `startsWith`）。|
|appOwnerOrganizationId|String|包含注册应用程序的租户 ID。 这仅适用于应用程序支持的服务主体。支持 `$filter`（`eq`、`ne`、`NOT`、`ge`、`le`）。|
|appRoleAssignmentRequired|布尔|指定在用户登录或应用可以获取令牌前，是否需要先向用户或其他服务主体授予此服务主体的应用角色分配。 默认值为 `false`。 不可为空。 <br><br>支持 `$filter`（`eq`、`ne`、`NOT`）。 |
|appRoles|[appRole](approle.md) 集合|该服务主体代表的应用程序公开的角色。 有关详细信息，请参阅 [应用程序](application.md)实体上的 **appRoles** 属性定义。 不可为空。 |
|customSecurityAttributes|[customSecurityAttributeValue](../resources/customsecurityattributevalue.md)|保留分配给目录对象的自定义安全属性的值的开放式复杂类型。 可为 NULL。 <br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not`、 `startsWith`）。|
| deletedDateTime | DateTimeOffset | 删除服务主体的日期和时间。只读。 |
| 说明 | 字符串 | 免费文本字段，提供面向内部最终用户的服务主体说明。 "MyApps ["](/azure/active-directory/user-help/my-apps-portal-end-user-access) 等最终用户门户将在此字段中显示应用程序说明。 最大允许大小为 1024 个字符。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`startsWith`）和 `$search`。|
| disabledByMicrosoftStatus | String | 指定 Microsoft 是否已禁用已注册的应用程序。可能的值为：`null`（默认值）、`NotDisabled` 和 `DisabledDueToViolationOfServicesAgreement`（原因可能包括可疑、滥用或恶意活动或违反 Microsoft 服务协议）。 <br><br> 支持 `$filter`（`eq`、`ne`、`not`）。  |
|displayName|String|服务主体的显示名称。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）、`$search` 和 `$orderBy`。 |
|errorUrl|String|已弃用。 请勿使用。|
|homepage|String|应用程序的主页或登录页面。|
| id | String | 服务主体的唯一标识符。 继承自 [directoryObject](directoryobject.md)。 键。 不可为 null。 只读。 支持 `$filter` （`eq`、 `ne`、 `not`、 `in`）。 |
| info | [informationalUrl](informationalurl.md) | 所获取应用程序的基本配置文件信息，如应用的市场营销、支持、服务条款和隐私声明 URL。 服务条款和隐私声明通过用户同意体验展示给用户。 有关详细信息，请参阅[如何：为已注册的 Azure AD 应用添加服务条款和隐私声明](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement)。 <br><br>支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le` 和 `null` 值上的 `eq`）。  |
|keyCredentials|[keyCredential](keycredential.md) 集合|与服务帐户关联的密钥凭据集合。 不可为 null。 支持 `$filter`（`eq`、`not`、`ge`、`le`）。            |
|loginUrl|String|指定服务提供商将用户重定向到 Azure AD 进行身份验证的 URL。 Azure AD 使用 URL 从 Microsoft 365 或Azure AD My Apps 启动应用程序。 该选项为空时，Azure AD 将对使用“[基于 SAML 的单一登录](/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso)”配置的应用程序执行 IdP 启动的登录。 用户从 Microsoft 365、Azure AD My Apps 或Azure AD SSO URL 启动应用程序。|
|logoutUrl|String| 指定 Microsoft 授权服务使用 OpenId Connect [正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。|
|notes|String|免费文本字段，用于捕获有关服务主体的信息，通常用于操作。最大允许大小为 1024 个字符。|
|notificationEmailAddresses|字符串集合|指定在活动证书临近到期日期时，Azure AD 在其中发送通知的电子邮件地址列表。 这仅适用于用于签署为 Azure AD 库应用程序发行的 SAML 令牌的证书。|
|passwordCredentials|[passwordCredential](passwordcredential.md) 集合|与服务帐户关联的密码凭据集合。不可为空。 |
|passwordSingleSignOnSettings|[passwordSingleSignOnSettings](passwordsinglesignonsettings.md)|有关密码单一登录的设置的集合。 使用 `$select=passwordSingleSignOnSettings` 读取属性。 对 [applicationTemplates](applicationTemplate.md)（自定义 applicationTemplates 除外）只读。 |
|preferredSingleSignOnMode|string|指定为此应用程序配置的单一登录模式。 Azure AD 使用首选单一登录模式从 Microsoft 365 或Azure AD My Apps 启动应用程序。 支持的值是：`password`、`saml`、`notSupported` 和 `oidc`。|
|preferredTokenSigningKeyEndDateTime|DateTimeOffset|指定用于令牌签名的 keyCredential 的到期日期，由 **preferredTokenSigningKeyThumbprint** 标记。|
|preferredTokenSigningKeyThumbprint|String|仅供内部使用。 请勿写入属性，否则将依赖该属性。 可能会在未来版本中删除。 |
|publishedPermissionScopes|[permissionScope](permissionscope.md) 集合|应用程序公开的委派权限。 有关详细信息，请参阅 [应用程序](application.md)实体上的 **api** 属性的 **oauth2PermissionScopes** 属性。 不可为 null。|
|replyUrls|String 集合|向其发送用户令牌以使用关联应用程序登录的 URL，或者为关联应用程序向其发送 OAuth 2.0 授权代码和访问令牌的重定向 URI。不可为 null。 |
|samlMetadataUrl|String|服务用于公开联合身份验证的 SAML 元数据的 URL。|
|samlSingleSignOnSettings|[samlSingleSignOnSettings](samlsinglesignonsettings.md)|有关 saml 单一登录的设置的集合。|
|servicePrincipalNames|字符串集合|包含从关联的 [应用程序](application.md)中复制的 **identifiersUris** 列表。 可以将其他值添加到混合应用程序。 这些值可用于标识此应用程序在 Azure AD 中公开的权限。 例如，<ul><li>客户端应用可以指定基于此属性的值的资源 URI（即“aud”声明中返回的 URI），以获取访问令牌。</li></ul><br>多值属性上的筛选器表达式需要 any 运算符。不可为 NULL。<br><br> 支持 `$filter`（`eq`、`not`、`ge`、`le`、`startsWith`）。|
|servicePrincipalType|String|标识服务主体是表示应用程序还是托管标识。 这是由 Azure AD 内部设置的。 对于表示 [应用程序](./application.md)的服务主体，此选项设置为“__Application__”。 对于表示 [托管标识](/azure/active-directory/managed-identities-azure-resources/overview)的服务主体，此选项设置为“__ManagedIdentity__”。 __SocialIdp__ 类型供内部使用。 |
| signInAudience | String | 指定当前应用程序支持的 Microsoft 帐户。只读。 <br><br>支持的值为：<ul><li>`AzureADMyOrg`：在我的组织的 Azure AD 租户（即单租户）中拥有 Microsoft 工作或学校帐户的用户</li><li>`AzureADMultipleOrgs`：在任何组织的 Azure AD 租户（多租户）中拥有 Microsoft 工作或学校帐户的用户。</li><li>`AzureADandPersonalMicrosoftAccount`：拥有个人 Microsoft 帐户或任意组织的 Azure AD 租户中的工作或学校帐户的用户。</li><li>`PersonalMicrosoftAccount`：仅限拥有个人 Microsoft 帐户的用户。</li></ul> |
|tags|String collection| 可用于对服务主体进行分类和识别的自定义字符串。不可为空。<br><br>支持 `$filter`（`eq`、`not`、`ge`、`le`、`startsWith`）。|
|tokenEncryptionKeyId|String|指定 keyCredentials 集合中的公共密钥的 keyId。 配置后，Azure AD 为此应用程序发布使用此属性指定的密钥加密的令牌。 接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。|
| verifiedPublisher          | [verifiedPublisher](verifiedPublisher.md)                            | 指定该服务主体代表的应用程序的已验证发布者。|

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|appManagementPolicies|[appManagementPolicy](../resources/appManagementPolicy.md) 集合| 应用到此服务主体的 appManagementPolicy。|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|此应用或服务的应用角色分配，已授予用户、组和其他服务主体。支持 `$expand`。|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) 集合|另一个应用或服务的应用角色分配，已授予此服务主体的。 支持 `$expand`。|
|claimsMappingPolicies|[claimsMappingPolicy](claimsmappingpolicy.md) 集合|为此服务主体分配的 claimsMappingPolicies。 支持 `$expand`。|
|createdObjects|[directoryObject](directoryobject.md) collection|由此服务主体创建的目录对象。只读。空。|
|delegatedPermissionClassifications|[delegatedPermissionClassification](delegatedpermissionclassification.md) 集合|此服务主体公开的委派权限的权限分类。 支持 `$expand`。|
|endpoints|[endpoint](endpoint.md) 集合|可用于发现的终结点。SharePoint 等服务使用特定于租户的 SharePoint 终结点填充此属性，其他应用程序可在这些终结点的体验中发现和使用。|
|homeRealmDiscoveryPolicies|[homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) 集合|为此服务主体分配的 homeRealmDiscoveryPolicies。 支持 `$expand`。|
|memberOf|[directoryObject](directoryobject.md) 集合|此服务主体所属的角色。 HTTP 方法：GET 只读。 可为空。 支持 `$expand`。|
|oauth2PermissionGrants|[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合|委派权限授予设置此服务主体以代表已登录用户访问 API 的权限。只读。可为空。|
|ownedObjects|[directoryObject](directoryobject.md) 集合|此服务主体所拥有的目录对象。 只读。 可为空。 支持 `$expand`。|
|owners|[directoryObject](directoryobject.md) 集合|servicePrincipal 所述的目录对象。 所有者是一组允许修改此对象的非管理员用户或 servicePrincipal。 只读。 可为空。 支持 `$expand`。|
|tokenIssuancePolicies|[tokenIssuancePolicy](tokenissuancepolicy.md) 集合|为此服务主体分配的 tokenIssuancePolicies。 支持 `$expand`。|
|tokenLifetimePolicies|[tokenLifetimePolicy](tokenlifetimepolicy.md) 集合|为此服务主体分配的 tokenLifetimePolicies。 支持 `$expand`。|

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignedTo",
    "appRoleAssignments",
    "createdObjects",
    "createdOnBehalfOf",
    "endpoints",
    "memberOf",
    "oauth2PermissionGrants",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.servicePrincipal"
}-->

```json
{
  "accountEnabled": true,
  "addIns": [{"@odata.type": "microsoft.graph.addIn"}],
  "alternativeNames": "string",
  "appDisplayName": "string",
  "appId": "string",
  "appOwnerOrganizationId": "guid",
  "applicationTemplateId": "string",
  "appRoleAssignmentRequired": true,
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "customSecurityAttributes": {
    "@odata.type": "microsoft.graph.customSecurityAttributeValue"
  },
  "disabledByMicrosoftStatus": "string",
  "displayName": "string",
  "errorUrl": "string",
  "homepage": "string",
  "id": "string (identifier)",
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "loginUrl": "string",
  "logoutUrl": "string",
  "notes": "String",
  "notificationEmailAddresses": ["string"],
  "publishedPermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "passwordSingleSignOnSettings": {"@odata.type": "microsoft.graph.passwordSingleSignOnSettings"},
  "preferredSingleSignOnMode": "string",
  "preferredTokenSigningKeyEndDateTime": "DateTime",
  "preferredTokenSigningKeyThumbprint": "string",
  "replyUrls": ["string"],
  "samlMetadataUrl": "string",
  "samlSingleSignOnSettings": "microsoft.DirectoryServices.SamlSingleSignOnSettings",
  "servicePrincipalNames": ["string"],
  "servicePrincipalType": "string",
  "signInAudience": "String",
  "tags": ["string"],
  "tokenEncryptionKeyId": "String",
  "useCustomTokenSigningKey": false,
  "verifiedPublisher": {"@odata.type": "microsoft.graph.verifiedPublisher"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


