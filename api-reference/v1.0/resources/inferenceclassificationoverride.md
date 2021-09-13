---
title: inferenceClassificationOverride 资源类型
description: 表示来自特定发件人的传入邮件始终应如何分类的用户的替代。
ms.localizationpriority: medium
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 652e01ea00bbca40f6ec3a7f685e636ef5aa4167
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118598"
---
# <a name="inferenceclassificationoverride-resource-type"></a>inferenceClassificationOverride 资源类型

命名空间：microsoft.graph

表示来自特定发件人的传入邮件始终应如何分类的用户的替代。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[更新](../api/inferenceclassificationoverride-update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |按指定内容更改替代的 **ClassifyAs** 字段。 |
|[删除](../api/inferenceclassificationoverride-delete.md) | 无 |删除由其 ID 指定的替代。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|classifyAs|inferenceClassificationType| 指定来自特定发件人的传入邮件始终应如何分类。 可能的值是 `focused` `other` ：、。|
|id|string| 替代的唯一标识符。只读。|
|senderEmailAddress|[emailAddress](emailaddress.md)|为其创建替代的发件人的电子邮件地址信息。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

