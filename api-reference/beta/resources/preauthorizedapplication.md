---
title: preAuthorizedApplication 资源类型
description: 表示应用程序和隐式同意请求的权限。 需要管理员可以提供了到应用程序的许可。 preAuthorizedApplications 不需要用户同意所请求的权限。 PreAuthorizedApplications 中列出的权限不需要用户同意。 但是，preAuthorizedApplications 中未列出任何其他请求的权限要求用户同意。
localization_priority: Normal
ms.openlocfilehash: 22945589341066f4609d47773cb04426774648fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524546"
---
# <a name="preauthorizedapplication-resource-type"></a>preAuthorizedApplication 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示应用程序和隐式同意请求的权限。 需要管理员可以提供了到应用程序的许可。 preAuthorizedApplications 不需要用户同意所请求的权限。 PreAuthorizedApplications 中列出的权限不需要用户同意。 但是，preAuthorizedApplications 中未列出任何其他请求的权限要求用户同意。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|appId|String| 应用程序的唯一标识符。 |
|permissionIds|String 集合| 需要[publishedPermissionScope](permissionscope.md)或[appRole](approle.md)应用程序的唯一标识符。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/preauthorizedapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
