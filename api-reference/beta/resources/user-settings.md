---
title: 设置资源类型
description: '当前用户设置。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5812141d21a32b8ab1835a75c05cbd57ea25a3a4
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571812"
---
# <a name="settings-resource-type"></a>设置资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

当前用户设置。 若要了解如何获取或更新用户设置，请参阅[获取设置](../api/user-get-settings.md)并[更新设置](../api/user-update-settings.md)。

该资源支持：

- 检查用户和用户的组织是否为内容发现参与。
- 如果禁用或启用特定用户的内容发现。 这还将禁用 Office 深入中的文档。

## <a name="methods"></a>方法
| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取用户设置](../api/user-get-settings.md) |[settings](../resources/user-settings.md)| 获取用户和组织设置。 |
|[更新用户设置](../api/user-update-settings.md) |[settings](../resources/user-settings.md)| 更新用户的当前设置。 |

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|布尔值|设置为 true，代理访问权限的用户时禁用[趋势](insights-trending.md)API。 当设置为在用户的 Office 深入为 true，则文档将被禁用。 当设置为 true，Office 365，例如在建议的网站中 SharePoint 主页中显示的内容的相关性和受影响的 OneDrive for Business 中的发现视图。 用户可以控制在[Office 深入](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)此设置。 |
|contributionToContentDiscoveryAsOrganizationDisabled|布尔值|反映[组织级别设置](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)控制对[趋势](insights-trending.md)API 的代理访问。 当设置为 true，组织不具有对 Office 深入的访问。 为整个组织受影响的 Office 365，例如在建议的网站中 SharePoint 主页和 OneDrive for Business 中的发现视图中显示的内容相关性。 此设置是只读的并且只能通过[SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)中的管理员来更改。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.userSettings"
}-->
```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/user-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
