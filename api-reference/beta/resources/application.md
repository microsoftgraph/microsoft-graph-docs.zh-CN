---
title: 应用程序资源类型
description: '表示应用程序。 任何将身份验证外包到 Azure Active Directory (Azure AD) 的应用程序都必须在目录中注册。 应用程序注册涉及告知 Azure AD 有关应用程序的信息，包括其所在的 URL、身份验证后发送回复的 URL、标识应用程序的 URI 等。 有关详细信息，请参阅“在 Azure AD 中注册应用程序的基础知识”。 继承自 directoryObject。 '
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 694f6b12dd8fe1fd59f12cafebd47c842a4077cb
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641552"
---
# <a name="application-resource-type"></a>应用程序资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示应用程序。 任何将身份验证外包到 Azure Active Directory (Azure AD) 的应用程序都必须在目录中注册。 应用程序注册涉及告知 Azure AD 有关应用程序的信息，包括其所在的 URL、身份验证后发送回复的 URL、标识应用程序的 URI 等。 有关详细信息，请参阅[在 Azure AD 中注册应用程序的基础知识](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad)。 继承自 [directoryObject](directoryobject.md)。 

> **注意：** 对应用程序资源类型的更改目前正在开发中。 有关详细信息，请参阅 [Microsoft Graph 的已知问题](/graph/known-issues#application-and-serviceprincipal-api-changes)。

该资源支持：

- 通过提供 [delta](../api/application-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[获取应用程序](../api/application-get.md) | 应用程序 |读取 application 对象的属性和关系。|
|[创建应用程序](../api/application-post-applications.md) | 应用程序 | 创建（注册）新应用程序。|
|[列出应用程序](../api/application-list.md) | 应用程序 | 检索该组织中应用程序的列表。 |
|[更新应用程序](../api/application-update.md) | 应用程序 |更新 application 对象。 |
|[删除应用程序](../api/application-delete.md) | 无 |删除 application 对象。 |
|[列出已分配策略](../api/policy-list-assigned.md)| [policy](policy.md) 集合| 获取已分配至此对象的所有策略。|
|[创建所有者](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| 通过发布到所有者集合创建新的所有者。|
|[列出所有者](../api/application-list-owners.md) |[directoryObject](directoryobject.md) 集合| 获取所有者对象集合。|
|[delta](../api/application-delta.md)|应用程序集合| 获取应用程序的增量更改。 |
|[创建调用](../api/application-post-calls.md)|[call](call.md)|通过发布到调用集合创建新的调用。|
|[创建在线会议](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|通过发布到 onlineMeetings 集合创建新的在线会议。|

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|api|[api](api.md)| 指定 API 应用程序的设置。 |
|appId| String | Azure AD 分配给应用程序的应用程序唯一标识符。 不可为 Null。 只读。 |
|appRoles|[appRole](approle.md) 集合|应用程序可声明的应用程序角色的集合。 这些角色可以分配给用户、组或服务主体。 不可为 Null。|
|createdDateTime|DateTimeOffset| 注册应用程序的日期和时间。 |
|deletedDateTime|DateTimeOffset| 删除应用程序的日期和时间。 |
|displayName|String|应用程序的显示名称。 |
|id|String|应用程序的唯一标识符。 继承自 [directoryObject](directoryobject.md)。 键。 不可为 null。 只读。 |
|identifierUris|String 集合| 用于标识应用程序的 URI。 有关详细信息，请参阅[应用程序对象和服务主体对象](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)。 多值属性筛选器表达式需要 *any* 运算符。 不可为 Null。 |
|info|[informationalUrl](informationalurl.md)| 应用程序的基本配置文件信息。 |
|isFallbackPublicClient|Boolean| 将回退应用类型指定为公共客户端，例如在移动设备上运行的已安装应用。 默认值为 *false*，这意味着回退应用类型是诸如 Web 应用之类的机密客户端。 在某些情况下，Azure AD 无法确定客户端应用类型（例如 [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) 流，其中在不指定重定向 URI 的情况下配置客户端应用类型）。 在这些情况下，Azure AD 将基于此属性的值解释应用类型。|
|keyCredentials|[keyCredential](keycredential.md) 集合|与应用程序关联的密钥凭据集合，不可为 Null。 |
|logo|Stream|应用程序的主徽标。 不可为 Null。 |
|optionalClaims|optionalClaims| 保留供以后使用。 |
|orgRestrictions|String 集合| 保留供以后使用。 |
|parentalControlSettings|[parentalControlSettings](parentalcontrolsettings.md) |指定应用程序的家长控制设置。|
|passwordCredentials|[passwordCredential](passwordcredential.md) 集合|与应用程序关联的密码凭据集合。 不可为 Null。|
|publicClient|[publicClient](publicclient.md)| 指定已安装客户端（如台式设备或移动设备）的设置。 |
|publisherDomain| String | 应用程序的已验证发布者域。 只读。|
|requiredResourceAccess|[requiredResourceAccess](requiredresourceaccess.md) 集合|指定此应用程序需要访问的资源以及在每个资源下所需的 OAuth 权限范围和应用程序角色集。 这种预配置的所需资源访问权限可驱动同意体验。 不可为 Null。|
|signInAudience | String | 指定当前应用程序支持的 Microsoft 帐户。 支持的值为：<ul><li>**AzureADMyOrg**：在我的组织的 Azure AD 租户（即单租户）中拥有 Microsoft 工作或学校帐户的用户</li><li>**AzureADMultipleOrgs**：在任意组织的 Azure AD 租户（即多租户）中拥有 Microsoft 工作或学校帐户的用户</li> <li>**AzureADandPersonalMicrosoftAccount**：拥有个人 Microsoft 帐户或任意组织的 Azure AD 租户中的工作或学校帐户的用户</li></ul> | `AzureADandPersonalMicrosoftAccount` |
|tags|String 集合| 可用于分类和标识应用程序的自定义字符串。 |
|web|[web](web.md)| 指定 Web 应用程序的设置。 |

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
|:---------------|:--------|:----------|
|calls           |[call](call.md) 集合                  |只读。可为 Null。|
|connectorGroup|[connectorGroup](connectorgroup.md)| 应用程序与 Azure AD 应用程序代理一起使用的 connectorGroup。 可为 Null。|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| 只读。|
|onlineMeetings  |[onlineMeeting](onlinemeeting.md) 集合|只读。可为 Null。|
|owners|[directoryObject](directoryobject.md) 集合|拥有此应用程序的目录对象。 所有者是一组允许修改此对象的非管理员用户。 需要版本 2013-11-08 或更高版本。 只读。 可为 Null。|
|policy|[policy](policy.md) 集合|已分配至此应用程序的策略。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "createdOnBehalfOf",
    "owners"
  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "api": {"@odata.type": "microsoft.graph.apiApplication"},
  "appId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isFallbackPublicClient": true,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "optionalClaims": [{"@odata.type": "microsoft.graph.optionalClaims"}],
  "orgRestrictions": ["Guid"],
  "parentalControlSettings": [{"@odata.type": "microsoft.graph.parentalControlSettings"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "signInAudience": "String",
  "tags": ["String"],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/application.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
