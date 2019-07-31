---
title: preAuthorizedApplication 资源类型
description: 表示应用程序和请求的隐式同意权限。 要求管理员向应用程序提供许可。 preAuthorizedApplications 不要求用户同意请求的权限。 PreAuthorizedApplications 中列出的权限不需要用户同意。 但是, preAuthorizedApplications 中未列出的任何其他请求的权限都需要用户同意。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7adaf4fe960b762b12f6b2cc8607e64c9813712e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965813"
---
# <a name="preauthorizedapplication-resource-type"></a>preAuthorizedApplication 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示应用程序和请求的隐式同意权限。 要求管理员向应用程序提供许可。 preAuthorizedApplications 不要求用户同意请求的权限。 PreAuthorizedApplications 中列出的权限不需要用户同意。 但是, preAuthorizedApplications 中未列出的任何其他请求的权限都需要用户同意。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|appId|String| 应用程序的唯一标识符。 |
|permissionIds|String collection| 应用程序所需的[publishedPermissionScope](permissionscope.md)或[appRole](approle.md)的唯一标识符。 |

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
  "suppressions": []
}
-->
