---
title: appRoleAssignment 资源类型
description: 用于记录何时将用户、组或服务主体分配给应用程序的服务主体上的应用角色。可以创建、读取和删除应用角色分配。
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 67e3684b9b0668ae7adce632dd754eb813bf1162
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333195"
---
# <a name="approleassignment-resource-type"></a>appRoleAssignment 资源类型

命名空间：microsoft.graph

用于记录何时将用户、组或服务主体分配给应用的应用角色。

应用角色分配是分配的主体（用户、组或服务主体）、资源应用程序（应用的服务主体）与在资源应用程序上定义的应用角色之间的关系。

如果已分配给主体的 [应用角色](approle.md) 的 **值** 属性不为空，则将其包含在主题为已分配主体的令牌（例如 SAML 响应、ID 令牌、标识已登录用户的访问令牌或者标识服务主体的访问令牌）**角色** 声明中。应用程序和 API 将这些声明用作授权逻辑的一部分。

可直接向用户分配应用角色。 如果将某应用角色分配给组，则该组的直接成员也将被视为已分配了该应用角色。 向用户分配应用程序的应用角色后，该应用程序的磁贴将显示在用户的 [MyApps 门户](/azure/active-directory/user-help/my-apps-portal-end-user-access)和 [Microsoft 365 应用启动器](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a)中。

分配的主体为服务主体的应用角色分配是 [仅限应用权限](/azure/active-directory/develop/v2-permissions-and-consent#permission-types) 授予。当用户或管理员同意仅限应用的权限时，将创建应用角色分配，其中分配的主体是客户端应用程序的服务主体，资源是目标 API 的服务主体。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| appRoleId | Guid | 分配给主体的 [应用角色](approle.md)的标识符 (**id**)。 必须在资源应用程序的服务主体 (**resourceId**) 上的 **appRoles** 属性中公开此应用角色。 如果资源应用程序尚未声明任何应用角色，则可以指定默认应用角色 ID `00000000-0000-0000-0000-000000000000`，以表示将主体分配给资源应用，但没有任何特定应用角色。 创建时为必需项。  |
| createdDateTime | DateTimeOffset | 创建应用角色分配的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 表示为：`2014-01-01T00:00:00Z`。只读。  |
| id | String | **appRoleAssignment** 键的唯一标识符。不可为 null。只读。 |
| principalDisplayName | String |已被授予应用角色分配的用户、组或服务主体的显示名称。支持 `$filter`（`eq` 和 `startswith`）。 |
| principalId | Guid | 被授予应用角色的 [用户](user.md)、[组](group.md) 或 [服务主体](serviceprincipal.md) 的唯一标识符（**id**）。创建时需要。  |
| principalType | 字符串 | 已分配的主体的类型。 这可以是 `User`、`Group` 或 `ServicePrincipal`。 只读。  |
| resourceDisplayName | 字符串 | 已为其分配的资源应用的服务主体的显示名称。  |
| resourceId | Guid |已为其进行分配的资源 [服务主体](serviceprincipal.md) 的唯一标识符（**id**）。创建时需要。支持`$filter`（仅限 `eq`）。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "appRoleId": "Guid",
  "createdDateTime": "String (timestamp)",
  "id": "String",
  "principalDisplayName": "String",
  "principalId": "Guid",
  "principalType": "String",
  "resourceDisplayName": "String",
  "resourceId": "Guid"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
