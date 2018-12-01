---
title: preAuthorizedApplication 资源类型
description: 表示应用程序和隐式同意请求的权限。 需要管理员可以提供了到应用程序的许可。 preAuthorizedApplications 不需要用户同意所请求的权限。 PreAuthorizedApplications 中列出的权限不需要用户同意。 但是，preAuthorizedApplications 中未列出任何其他请求的权限要求用户同意。
ms.openlocfilehash: d299aefcac541407e0e42d0b0933e903afa3e84d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049092"
---
# <a name="preauthorizedapplication-resource-type"></a>preAuthorizedApplication 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
<!-- {
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->