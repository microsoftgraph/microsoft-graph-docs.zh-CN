---
title: 网站资源类型
description: 代表网站。
localization_priority: Normal
ms.openlocfilehash: b44fcacf77f3b2afb5cdc9dfea2340d0a1fc1cd5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339606"
---
# <a name="website-resource-type"></a>网站资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表网站。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|type|String| 可取值为：`other`、`home`、`work`、`blog`、`profile`。|
|address|string|网站的 URL。|
|displayName|string|网站的显示名称。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
