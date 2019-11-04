---
title: resourceAccess 资源类型
description: 指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: d0d04ba99c0132a0f305bb0fdcaa5e32071d7554
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939262"
---
# <a name="resourceaccess-resource-type"></a>resourceAccess 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。 [RequiredResourceAccess](requiredresourceaccess.md)类型的**ResourceAccess**属性是**resourceAccess**的集合。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|Guid|资源应用程序公开的[oauth2PermissionScopes](permissionscope.md)或[appRole](approle.md)实例之一的唯一标识符。|
|type|字符串|指定**id**属性引用的是[oauth2PermissionScopes](permissionscope.md)还是[appRole](approle.md)。 可能的值为 "scope" 或 "role"。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
