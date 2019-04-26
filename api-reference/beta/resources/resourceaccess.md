---
title: resourceAccess 资源类型
description: 指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。 requiredResourceAccess 类型的**resourceAccess**属性是**resourceAccess**的集合。
localization_priority: Normal
ms.openlocfilehash: bb77a12a207e274b27263029d96f4ef260cfe5cb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343631"
---
# <a name="resourceaccess-resource-type"></a>resourceAccess 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。 [requiredResourceAccess](requiredresourceaccess.md)类型的**resourceAccess**属性是**resourceAccess**的集合。


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
|id|Guid|资源应用程序公开的[oAuth2Permission](oauth2permission.md)或[appRole](approle.md)实例之一的唯一标识符。|
|type|String|指定**id**属性引用的是[oAuth2Permission](oauth2permission.md)还是[appRole](approle.md)。 可能的值为 "scope" 或 "role"。|

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
