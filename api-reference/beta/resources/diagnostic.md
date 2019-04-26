---
title: 诊断资源类型
description: 有关 OneNote 操作的错误或警告的信息。
localization_priority: Normal
ms.openlocfilehash: 63e146cd44e3e2866d9d632fb78cbc222443c9d8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340866"
---
# <a name="diagnostic-resource-type"></a>诊断资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

有关 OneNote 操作的错误或警告的信息。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |描述|
|:---------------|:--------|:----------|
|message|字符串|描述触发错误或警告的条件的消息。|
|url|String|有关此问题的文档的链接。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
