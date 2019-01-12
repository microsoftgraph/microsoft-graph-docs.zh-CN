---
title: 应用程序资源类型
description: '代表应用程序。 必须在目录中注册 outsources Azure Active Directory (Azure AD) 身份验证的任何应用程序。 应用程序注册涉及告诉 Azure AD 关于您的应用程序，包括其具有位于何处，身份验证，以确定您的应用程序和更多的 URI 后发送答复的 URL 的 URL。 有关详细信息，请参阅基础知识的注册 Azure AD 中的应用程序。 继承自 directoryObject。 '
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9fb5722640149471f6728ec6ab893cf388fa9b6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946677"
---
# <a name="application-resource-type"></a>应用程序资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表应用程序。 必须在目录中注册 outsources Azure Active Directory (Azure AD) 身份验证的任何应用程序。 应用程序注册涉及告诉 Azure AD 关于您的应用程序，包括其具有位于何处，身份验证，以确定您的应用程序和更多的 URI 后发送答复的 URL 的 URL。 有关详细信息，请参阅[基础知识的注册 Azure AD 中的应用程序](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad)。 继承自 [directoryObject](directoryobject.md)。 

> **注意：** 当前正在开发对应用程序资源类型的更改。 有关详细信息，请参阅[使用 Microsoft Graph 的已知问题](/graph/known-issues#application-and-serviceprincipal-api-changes)。

该资源支持：

- 通过提供 [delta](../api/application-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[获取应用程序](../api/application-get.md) | application |读取属性和 application 对象的关系。|
|[创建应用程序](../api/application-post-applications.md) | application | 创建 (register) 的新应用程序。|
|[应用程序列表](../api/application-list.md) | application | 检索组织中的应用程序的列表。 |
|[更新应用程序](../api/application-update.md) | application |更新应用程序对象。 |
|[删除应用程序](../api/application-delete.md) | 无 |删除应用程序对象。 |
|[列表分配策略](../api/policy-list-assigned.md)| [策略](policy.md)集合| 获取所有策略分配给此对象。|
|[创建所有者](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| 通过发布到所有者集合中创建一个新的所有者。|
|[列出所有者](../api/application-list-owners.md) |[directoryObject](directoryobject.md) 集合| 获取一个所有者对象集合。|
|[delta](../api/application-delta.md)|应用程序集合| 获取应用程序的增量更改。 |
|[创建呼叫](../api/application-post-calls.md)|[呼叫](call.md)|通过发布到呼叫集合中创建新的呼叫。|
|[创建联机会议](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|通过发布到 onlineMeetings 集合中创建新的联机会议。|

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:---------------|:--------|:----------|
|api|[api](api.md)| 指定 API 应用程序的设置。 |
|appId| String | Azure AD 由分配给应用程序的应用程序的唯一标识符。 不可为 null。 只读。 |
|appRoles|[appRole](approle.md)集合|声明应用程序可能的应用程序角色的集合。 这些角色可以分配给用户、 组或服务主体。 不可为 null。|
|createdDateTime|DateTimeOffset| 日期和时间注册应用程序。 |
|deletedDateTime|DateTimeOffset| 日期和时间的应用程序已删除。 |
|displayName|字符串|应用程序的显示名称。 |
|id|字符串|应用程序的唯一标识符。 继承自 [directoryObject](directoryobject.md)。 键。 不可为 null。 只读。 |
|identifierUris|String 集合| 标识应用程序的 Uri。 有关详细信息，请参阅[应用程序对象和服务主体对象](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)。 *Any*运算符，则需要为多值属性的筛选器表达式。 不可为 null。 |
|信息|[informationalUrl](informationalurl.md)| 应用程序的基本配置文件信息。 |
|isFallbackPublicClient|布尔| 指定该回退应用程序类型为公共客户端，如已安装应用程序在移动设备上运行。 默认值为*false*这意味着该回退应用程序类型是机密的客户端，例如 web 应用程序。 有特定情况下，Azure AD 无法确定客户端应用程序类型 （例如配置时未指定重定向 URI 位置的[ROPC](https://tools.ietf.org/html/rfc6749#section-4.3)流）。 在这些情况下 Azure AD 将解释基于此属性的值的应用程序类型。|
|keyCredentials|[keyCredential](keycredential.md)集合|不应用程序关联的关键凭据集合可以为 null。 |
|logo|Stream|主应用程序徽标。 不可为 null。 |
|optionalClaims|optionalClaims| 保留以备今后使用。 |
|orgRestrictions|String 集合| 保留以备今后使用。 |
|parentalControlSettings|[parentalControlSettings](parentalcontrolsettings.md) |指定应用程序的家长的控制设置。|
|passwordCredentials|[passwordCredential](passwordcredential.md)集合|应用程序关联的密码凭据的集合。 不可为 null。|
|publicClient|[publicClient](publicclient.md)| 指定安装客户端，如桌面或移动设备的设置。 |
|publisherDomain| 字符串 | 应用程序验证的发行者域。 此为只读属性。|
|requiredResourceAccess|[requiredResourceAccess](requiredresourceaccess.md)集合|指定此应用程序需要访问和一组的 OAuth 权限范围和应用程序角色它需要在每个这些资源的资源。 此预配置完所需的资源访问驱动器的同意体验。 不可为 null。|
|signInAudience | 字符串 | 指定当前应用程序支持哪些 Microsoft 帐户。 支持的值包括：<ul><li>**AzureADMyOrg**： 与 Microsoft 的用户工作或学校我的组织 Azure AD 租户 （即单租户） 中的帐户</li><li>**AzureADMultipleOrgs**： 与 Microsoft 的用户工作或学校任何组织的 Azure AD 租户 （即多租户） 中的帐户</li> <li>**AzureADandPersonalMicrosoftAccount**： 用户个人 Microsoft 帐户或任何组织的 Azure AD 租户中的工作或学校帐户</li></ul> | `AzureADandPersonalMicrosoftAccount` |
|标记前添加的标记|String 集合| 用于分类和确定应用程序的自定义字符串。 |
|web|[web](web.md)| 指定 web 应用程序的设置。 |

## <a name="relationships"></a>Relationships

| 关系 | 类型 | Description |
|:---------------|:--------|:----------|
|呼叫           |[呼叫](call.md)集合                  |只读。可为 NULL。|
|connectorGroup|[connectorGroup](connectorgroup.md)| ConnectorGroup 应用程序使用与 Azure AD 应用程序代理。 可为 Null。|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| 此为只读属性。|
|onlineMeetings  |[onlineMeeting](onlinemeeting.md)集合|只读。可为 NULL。|
|owners|[directoryObject](directoryobject.md) 集合|目录对象的所有者的应用程序。 所有者是一组的非管理员用户有权修改此对象。 需要版本 2013年-11-08 或更高版本。 只读。 可为 Null。|
|策略|[策略](policy.md)集合|分配给此应用程序的策略。|

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
<!-- {
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
