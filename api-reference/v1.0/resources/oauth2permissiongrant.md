---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予应用程序的委派权限（OAuth 2.0 作用域），这通常是由用户或管理员的同意过程造成的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: edf4ff7ed44e9b084ca2206b24fed0e18b5c581c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290165"
---
# <a name="oauth2permissiongrant-resource-type"></a>oAuth2PermissionGrant 资源类型

命名空间：microsoft.graph

表示已授予应用程序的服务主体的委派权限。

委派权限授予可因用户同意应用程序的访问 API 的请求而创建，或直接创建。

委派权限有时称为 "OAuth 2.0 作用域" 或 "作用域"。

## <a name="methods"></a>Methods

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
| [列出 oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) 集合 | 检索委派权限授予的列表。 |
| [获取 oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md)  | 阅读单个委派权限授予。|
| [创建 oAuth2PermissionGrant](../api/oauth2permissiongrant-post.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) | 创建委派权限授予。 |
| [更新 oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | 无 | 更新 oAuth2PermissionGrant 对象。 |
| [删除 oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | 无  | 删除委派权限授予。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| id | String | **OAuth2PermissionGrant**的唯一标识符。 只读。|
| clientId | 字符串 | 授权在访问 API 时代表登录用户执行操作的应用程序的客户端[服务主体](serviceprincipal.md)的**id** 。 必填。 支持 `$filter` （ `eq` 仅限）。 |
| consentType | String | 指示是否向客户端应用程序授予了授权以模拟所有用户或仅模拟特定用户。 *AllPrincipals*表示模拟所有用户的授权。 *主体*指示模拟特定用户的授权。 管理员可以授予代表所有用户的同意。 在某些情况下，对于某些委派权限，非管理员用户可能有权代表自己同意代表自己。 必填。 支持 `$filter` （ `eq` 仅限）。 |
| principalId | String | 当**consentType**为*Principal*时，代表其授权客户端访问该资源的[用户](user.md)的**id** 。 如果**consentType**为*AllPrincipals* ，则此值为 null。 当**consentType**为*Principal*时是必需的。 |
| resourceId | String | 向其授予访问权限的资源[服务主体](serviceprincipal.md)的**id** 。 这将标识客户端授权尝试代表已登录用户呼叫的 API。 |
| scope | String | 应包含在资源应用程序（API）的访问令牌中的委派权限的声明值列表（以空格分隔）。 例如，`openid User.Read GroupMember.Read.All`。 每个声明值都应与 API 定义的某个委派权限的**值**字段相匹配，这些权限在资源[服务主体](serviceprincipal.md)的**publishedPermissionScopes**属性中列出。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
