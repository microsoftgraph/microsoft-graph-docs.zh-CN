---
title: 应用程序资源类型
description: 表示应用程序。
ms.localizationpriority: high
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 04f8f16b6c83c97708a2e56cc77474f24b075274
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333664"
---
# <a name="application-resource-type"></a>应用程序资源类型

命名空间：microsoft.graph

表示应用程序。 任何将身份验证外包到 Azure Active Directory (Azure AD) 的应用程序都必须在目录中注册。 应用程序注册涉及告知 Azure AD 有关应用程序的信息，包括其所在的 URL、身份验证后发送回复的 URL、标识应用程序的 URI 等。 有关详细信息，请参阅[在 Azure AD 中注册应用程序的基础知识](/azure/active-directory/develop/authentication-vs-authorization#basics-of-registering-an-application-in-azure-ad)。 继承自 [directoryObject](directoryobject.md)。

该资源支持通过提供 [delta](../api/application-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。 此资源是允许传入其他属性的开放类型。

## <a name="methods"></a>Methods

| 方法 | 返回类型 | Description |
|:---------------|:--------|:----------|
|[列出应用程序](../api/application-list.md) | [application](application.md) 集合 | 检索该组织中应用程序的列表。 |
|[创建应用程序](../api/application-post-applications.md) | [application](application.md) | 创建（注册）新应用程序。|
|[获取应用程序](../api/application-get.md) | [application](application.md) |读取 application 对象的属性和关系。|
|[更新应用程序](../api/application-update.md) | 无 |更新 application 对象。 |
|[删除应用程序](../api/application-delete.md) | 无 |删除 application 对象。 |
|[Get delta](../api/application-delta.md)|[application](application.md)|获得新建、更新或删除的应用，无需完全读取整个资源集合。|
|[列出已删除的应用程序](../api/directory-deleteditems-list.md) | [directoryObject](directoryobject.md) 集合 | 检索最近删除的应用程序的列表。 |
| [列出用户拥有的已删除应用程序](../api/directory-deleteditems-user-owned.md) | [directoryObject](directoryobject.md) 集合 | 检索租户中最近 30 天内删除的应用程序以及用户拥有的应用程序。 |
|[获取已删除的应用程序](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | 检索最近删除的应用程序的属性。 |
|[永久删除应用程序](../api/directory-deleteditems-delete.md) | 无 | 永久删除应用程序。 |
|[还原已删除的应用程序](../api/directory-deleteditems-restore.md) | [directoryObject](directoryobject.md) | 还原最近删除的应用程序。 |
|**证书和密码**| | |
|[添加密码](../api/application-addpassword.md)|[passwordCredential](passwordcredential.md)|向应用程序添加强密码。|
|[删除密码](../api/application-removepassword.md)|[passwordCredential](passwordcredential.md)|从应用程序删除密码。|
|[加号键](../api/application-addkey.md)|[keyCredential](keycredential.md)|向应用程序添加密钥凭据。|
|[删除键](../api/application-removekey.md)|无|从应用程序中删除密钥凭据。|
|**Extensions**| | |
| [列出 extensionProperties](../api/application-list-extensionproperty.md) | [extensionProperty](extensionProperty.md) 集合 | 列出应用程序对象上的扩展属性。 |
| [创建 extensionProperties](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | 在应用程序对象上创建扩展属性。 |
| [获取 extensionProperty](../api/extensionproperty-delete.md) | None | 从应用程序对象获取扩展属性。 |
| [删除 extensionProperty](../api/extensionproperty-delete.md) | 无 | 从应用程序对象删除扩展属性。 |
|[获取可用扩展属性](../api/directoryobject-getavailableextensionproperties.md)|[extensionProperty](../resources/extensionproperty.md) 集合|获取已在目录中注册的目录扩展属性的所有或筛选列表。|
|**Owners**| | |
|[List owners](../api/application-list-owners.md) |[directoryObject](directoryobject.md) 集合| 获取所有者对象集合。|
|[添加所有者](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| 通过发布到所有者集合添加所有者。|
|[删除所有者](../api/application-delete-owners.md) |无| 从应用程序删除所有者。|
|**策略**| | |
|[分配 tokenIssuancePolicy](../api/application-post-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) 集合| 分配 tokenIssuancePolicy 至此对象。|
|[列出 tokenIssuancePolicies](../api/application-list-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) 集合| 获取已分配至此对象的所有 tokenIssuancePolicies。|
|[删除 tokenIssuancePolicy](../api/application-delete-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) 集合| 从此对象中删除 tokenIssuancePolicy。|
|[分配 tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md)| [tokenLifetimePolicy](tokenlifetimepolicy.md) 集合| 向此对象分配 tokenLifetimePolicy。|
|[列出 tokenLifetimePolicies](../api/application-list-tokenlifetimepolicies.md)| [tokenLifetimePolicy](tokenlifetimepolicy.md) 集合| 获取已分配至此对象的所有 tokenLifetimePolicies。|
|[删除 tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md)| [tokenLifetimePolicy](tokenlifetimepolicy.md) 集合| 从此对象中删除 tokenLifetimePolicy。|
|**已验证发布者**| | |
|[设置已验证发布者](../api/application-setverifiedpublisher.md)| 无 | 设置应用程序的已验证发布者。|
|[取消设置已验证发布者](../api/application-unsetverifiedpublisher.md)| 无 | 取消设置应用程序的已验证发布者。|

## <a name="properties"></a>属性

> [!IMPORTANT]
> 仅当使用设置为 `eventual` 和 `$count` 的 **ConsistencyLevel** 标头时，才支持 `$filter` 和 `$search` 查询参数的特定用法。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries#application-properties)。

| 属性 | 类型 | Description |
|:---------------|:--------|:----------|
| addIns | [addIn](addin.md) 集合| 定义使用服务可用于调用特定上下文中的应用的自定义行为。 例如，呈现文件流的应用程序可能会为其“FileHandler”功能[设置 addIns 属性](/onedrive/developer/file-handlers)。 这将使 Office 365 之类的服务在用户正在处理的文档上下文中调用应用程序。 |
| api | [apiApplication](apiapplication.md) | 指定实现 Web API 的应用程序的设置。 |
| appId | String | Azure AD 分配给应用程序的唯一标识符。不可为 Null。只读。 |
| applicationTemplateId | String | 应用程序模板的唯一标识符。 支持 `$filter`（`eq`、`not`、`ne`）。|
| appRoles | [appRole](approle.md) 集合 | 分配给应用程序的角色的集合。 使用[应用角色分配](approleassignment.md)，可将这些角色分配给与其他应用程序关联的用户、组或服务主体。 不可为空。 |
| createdDateTime | DateTimeOffset | 注册应用程序的日期和时间。DateTimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。只读。 <br><br> 支持 `$filter` (`eq`、`ne`、`not`、`ge`、`le`、`in` 和 `null` 值上的 `eq`) 和 `$orderBy`。 |
| deletedDateTime | DateTimeOffset | 删除应用程序的日期和时间。DateTimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。只读。 |
| 说明 | String | 用于向最终用户提供应用程序对象说明的空闲文本字段。 最大允许大小为 1024 个字符。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`startsWith`）和 `$search`。 |
| disabledByMicrosoftStatus | String | 指定 Microsoft 是否已禁用已注册的应用程序。可能的值为：`null`（默认值）、`NotDisabled` 和 `DisabledDueToViolationOfServicesAgreement`（原因可能包括可疑、滥用或恶意活动或违反 Microsoft 服务协议）。 <br><br> 支持 `$filter`（`eq`、`ne`、`not`）。 |
| displayName | String | 应用程序的显示名称。 支持 `$filter` (`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`)、`$search` 和 `$orderBy`。 |
| groupMembershipClaims | String | 配置应用程序预期的用户或 OAuth 2.0 访问令牌中发出的 `groups` 声明。要设置此属性，请使用以下有效字符串值之一：`None`、`SecurityGroup`（对于安全组和 Azure AD 角色）和 `All`（这将获取登录用户所属的所有安全组、通讯组和 Azure AD 目录角色）。 |
| id | String | 应用程序的唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥。不可为 null。只读。支持 `$filter`（`eq`、`ne`、`not`、`in`）|
| identifierUris | String collection | 也称为应用 ID URI，此值在将应用程序用作资源应用时设置。 identifierUris 可充当你将在 API 代码中引用的范围的前缀，必须具有全局唯一性。 可以使用提供的默认值（采用 `api://<application-client-id>` 形式）或指定更具有可读性的 URI（如 `https://contoso.com/api`）。 有关有效 identifierUris 模式和最佳做法的信息，请参阅 [Azure AD 应用程序注册安全性最佳做法](/azure/active-directory/develop/security-best-practices-for-app-registration#appid-uri-configuration)。 不可为 null。 <br><br>支持 `$filter`（`eq`、`ne`、`ge`、`le`、`startsWith`）。|
| info | [informationalUrl](informationalurl.md) | 应用程序的基本配置文件信息，如应用的市场营销、支持、服务条款和隐私声明 URL。 服务条款和隐私声明通过用户同意体验展示给用户。 有关详细信息，请参阅[如何：为已注册的 Azure AD 应用添加服务条款和隐私声明](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement)。 <br><br>支持 `$filter` (`eq`、`ne`、`not`、`ge`、`le` 和 `null` 值上的 `eq`)。 |
| isDeviceOnlyAuthSupported | 布尔值 | 指定此应用程序是否支持在无用户的情况下进行设备身份验证。默认值为 `false`。  |
| isFallbackPublicClient | Boolean | 将回退应用程序类型指定为公共客户端，例如在移动设备上运行的已安装应用程序。 默认值为 `false`，这意味着，回退应用程序类型为机密客户端，例如 Web 应用。 某些情况下，Azure AD 无法确定客户端应用程序类型。 例如，在未指定重定向 URI 的情况下配置它的 [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) 流。 在这种情况下，Azure AD 将基于此属性的值解释应用程序类型。|
| keyCredentials | [keyCredential](keycredential.md) 集合 | 与应用程序关联的密钥凭据集合。不可为 Null。支持 `$filter`（`eq`、`not`、`ge`、`le`）。 |
| logo | Stream | 应用程序的主徽标。不可为 Null。 |
| notes | String | 与应用程序管理相关的备注。 |
| oauth2RequiredPostResponse | Boolean | 指定在 OAuth 2.0 令牌请求过程中，Azure AD 是否允许与 GET 请求相反的 POST 请求。 默认值为 `false`，即指定只允许 GET 请求。 |
| optionalClaims | [optionalClaims](optionalclaims.md) | 应用程序开发人员可以在其 Azure AD 应用程序中配置可选声明，以指定由 Microsoft security token service 发送到其应用程序的声明。有关详细信息，请参阅 [如何：向应用提供可选声明](/azure/active-directory/develop/active-directory-optional-claims)。|
| parentalControlSettings | [parentalControlSettings](parentalcontrolsettings.md) |指定应用程序的家长控制设置。 |
| passwordCredentials | [passwordCredential](passwordcredential.md) 集合|与应用程序关联的密码凭据集合。不可为 Null。|
| publicClient | [publicClientApplication](publicclientapplication.md) | 指定已安装客户端（如台式设备或移动设备）的设置。 |
| publisherDomain | String | 应用程序的已验证发布者域。 只读。 有关更多信息，请参阅[操作指南：配置应用程序的发布者域](/azure/active-directory/develop/howto-configure-publisher-domain)。 支持 `$filter`（`eq`、`ne`、`ge`、`le`、`startsWith`）。|
| requiredResourceAccess |[requiredResourceAccess](requiredresourceaccess.md) 集合| 指定应用程序需要访问的资源。 此属性还指定每个资源所需的委派权限和应用程序角色的集合。 该配置对所需的资源的访问将推动许可体验。 可配置的资源服务 (API) 不能超过 50 个。 从 2021 年 10 月中旬开始，所需权限总数不得超过 400 个。 不可为 null。 <br><br>支持 `$filter`（`eq`、`not`、`ge`、`le`）。|
| signInAudience | String | 指定当前应用程序支持的 Microsoft 帐户。 可能的值是：`AzureADMyOrg`、`AzureADMultipleOrgs`、`AzureADandPersonalMicrosoftAccount`（默认）和 `PersonalMicrosoftAccount`。 请参阅下表中的 [，了解](#signinaudience-values)。 <br><br>支持 `$filter`（`eq`、`ne`、`not`）。|
| spa                     | [spaApplication](../resources/spaapplication.md)                            | 指定单页应用程序的设置，包括注销 URL 并重定向授权代码和访问令牌的 URI。 |
| 标记 |字符串集合| 可用于分类和标识应用程序的自定义字符串。不可为 null。<br><br>支持 `$filter`（`eq`、`not`、`ge`、`le`、`startsWith`）。|
| tokenEncryptionKeyId |字符串|指定 keyCredentials 集合中的公共密钥的 keyId。 配置后，Azure AD 将使用此属性指向的密钥对其发出的所有令牌进行加密。 接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。|
| verifiedPublisher          | [verifiedPublisher](verifiedPublisher.md)                            | 指定应用程序的已验证发布者。有关发布者验证如何帮助支持应用程序安全性、可信度和合规性的详细信息，请参阅 [发布者验证](/azure/active-directory/develop/publisher-verification-overview)。|
| web |[webApplication](webapplication.md)| 指定 Web 应用程序的设置。 |

### <a name="signinaudience-values"></a>signInAudience 值

| 值 | 说明 |
|:---------------|:--------|
|AzureADMyOrg|在我的组织的 Azure AD 租户（单租户）中拥有 Microsoft 工作或学校帐户的用户。|
|AzureADMultleOrgs|拥有任何组织的 Azure AD 租户（多租户）中 Microsoft 工作或学校帐户的用户。|
|AzureADandPersonalMicrosoftAccount|具有个人 Microsoft 帐户或任何组织的 Azure AD 租户中的工作或学校帐户的用户。 要使用 Azure Active Directory B2C 用户流程对用户进行身份验证，请使用 `AzureADandPersonalMicrosoftAccount`。 该值允许最广泛的用户标识集，包括本地账户和 Microsoft、Facebook、谷歌、Twitter 或任何 OpenID Connect 提供商的用户标识。 这是 **signInAudience** 属性的默认值。 |
|PersonalMicrosoftAccount|仅具有个人 Microsoft 帐户的用户。|

## <a name="relationships"></a>关系

| 关系 | 类型 | Description |
|:---------------|:--------|:----------|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| 只读。|
|extensionProperties|[extensionProperty](extensionproperty.md) 集合| 只读。可为 Null。|
|owners|[directoryObject](directoryobject.md) 集合|拥有此应用程序的目录对象。只读。可为 Null。支持 `$expand`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "createdOnBehalfOf",
    "owners"
  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "addIns": [{"@odata.type": "microsoft.graph.addIn"}],
  "api": {"@odata.type": "microsoft.graph.apiApplication"},
  "appId": "String",
  "applicationTemplateId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "disabledByMicrosoftStatus": "String",
  "displayName": "String",
  "groupMembershipClaims": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isDeviceOnlyAuthSupported": false,
  "isFallbackPublicClient": false,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "notes": "String",
  "oauth2RequiredPostResponse": false,
  "optionalClaims": {"@odata.type": "microsoft.graph.optionalClaims"},
  "parentalControlSettings": {"@odata.type": "microsoft.graph.parentalControlSettings"},
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "signInAudience": "String",
  "spa": {"@odata.type": "microsoft.graph.spaApplication"},
  "tags": ["String"],
  "tokenEncryptionKeyId": "String",
  "verifiedPublisher": {"@odata.type": "microsoft.graph.verifiedPublisher"},
  "web": {"@odata.type": "microsoft.graph.webApplication"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
