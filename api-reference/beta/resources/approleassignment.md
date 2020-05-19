---
title: appRoleAssignment 资源类型
description: 用于在将用户、组或服务主体分配给应用程序的服务主体上的应用程序角色时进行记录。 您可以创建、读取和删除应用程序角色分配。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 38f8cca5740da2cbd9807cd2411065a6bebda49c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291004"
---
# <a name="approleassignment-resource-type"></a>appRoleAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于记录何时向用户、组或服务主体分配应用程序的应用程序角色。

应用程序角色分配是分配的主体（用户、组或服务主体）、资源应用程序（应用程序的服务主体）和在资源应用程序上定义的应用程序角色之间的关系。

如果已分配给主体的[应用程序角色](approle.md)具有非空**值**属性，则会将其包含在使用者是分配主体的标记的**角色**声明中（例如，SAML 响应、ID 令牌、标识登录用户的访问令牌或标识服务主体的访问令牌）。 应用程序和 Api 将这些声明用作其授权逻辑的一部分。

可以直接向用户分配应用角色。 如果将某个应用程序角色分配给某个组，则会将该组的直接成员视为已分配应用程序角色。 为用户分配应用程序的应用程序角色时，将在用户的[MyApps 门户](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)和[Office 365 应用启动器](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a)中显示该应用程序的图块。

分配的主体是服务主体的应用程序角色分配是[仅限应用的权限](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types)授予。 当用户或管理员同意到仅应用程序的权限时，将创建一个应用程序角色分配，其中分配的主体是客户端应用程序的服务主体，而资源是目标 API 的服务主体。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| id | 字符串 | **AppRoleAssignment**项的唯一标识符。 不可为 null。 只读。 |
| creationTimestamp | DateTimeOffset | 应用程序角色分配的创建时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。 不支持 `$filter` 。 |
| principalId | Guid | 为其授予应用程序角色的[用户](user.md)、[组](group.md)或[服务主体](serviceprincipal.md)的唯一标识符（**id**）。 创建时为必需项。 不支持 `$filter` 。 |
| principalType | String | 分配的主体的类型。 它可以是“User”、“Group”或“ServicePrincipal”。 只读。 不支持 `$filter` 。 |
| principalDisplayName | String |向其授予应用程序角色分配的用户、组或服务主体的显示名称。 只读。 支持 `$filter` （ `eq` 和 `startswith` ）。 |
| resourceId | Guid |为其进行分配的资源[服务主体](serviceprincipal.md)的唯一标识符（**id**）。 创建时为必需项。 支持 `$filter` （ `eq` 仅限）。 |
| resourceDisplayName | String | 为其创建工作分配的资源应用程序的服务主体的显示名称。 不支持 `$filter` 。 |
| appRoleId | Guid | 分配给主体的[应用程序角色](approle.md)的标识符（**id**）。 此应用程序角色必须在资源应用程序的服务主体（**resourceId**）的**appRoles**属性中公开。 如果资源应用程序尚未声明任何应用角色，则可以指定一个默认的应用程序角色 ID，以指示将 `00000000-0000-0000-0000-000000000000` 主体分配给没有任何特定应用程序角色的资源应用程序。 创建时为必需项。 不支持 `$filter` 。 |

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
  "id": "string",
  "creationTimestamp": "String (timestamp)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid",
  "appRoleId": "guid"
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
