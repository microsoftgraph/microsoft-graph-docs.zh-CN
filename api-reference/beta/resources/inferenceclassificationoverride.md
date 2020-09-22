---
title: inferenceClassificationOverride 资源类型
description: 表示来自特定发件人的传入邮件应始终按如下方式分类的用户替代
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: b289d369c151e2f735fb992c5bd9a3347da67d17
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016533"
---
# <a name="inferenceclassificationoverride-resource-type"></a>inferenceClassificationOverride 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关特定发件人的传入邮件应始终按 [重点收件箱](manage-focused-inbox.md)的方式进行分类的用户替代。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[更新](../api/inferenceclassificationoverride-update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |按指定内容更改替代的 **ClassifyAs** 字段。 |
|[删除](../api/inferenceclassificationoverride-delete.md) | 无 |删除由其 ID 指定的替代。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|classifyAs|string| 指定来自特定发件人的传入邮件始终应如何分类。可能的值是：`focused`、`other`。|
|id|string| 替代的唯一标识符。只读。|
|senderEmailAddress|[emailAddress](emailaddress.md)|为其创建替代的发件人的电子邮件地址信息。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


