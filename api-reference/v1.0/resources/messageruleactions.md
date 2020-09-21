---
title: messageRuleActions 资源类型
description: 表示适用于规则的一组操作。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ed2486994a9ccb496dc92e241506baa867ebeb1f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965384"
---
# <a name="messageruleactions-resource-type"></a>messageRuleActions 资源类型

命名空间：microsoft.graph


表示适用于规则的一组操作。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| assignCategories | String 集合 | 分配给邮件的类别列表。 |
| copyToFolder | String | 将邮件复制到其中的文件夹的 ID。 |
| delete | Boolean | 指示邮件是否应移动到“已删除项目”文件夹。 |
| forwardAsAttachmentTo | [recipient](recipient.md) 集合 | 应以附件形式接收转发邮件的收件人的电子邮件地址。 |
| forwardTo | [recipient](recipient.md) 集合 | 应接收转发邮件的收件人的电子邮件地址。 |
| markAsRead | Boolean | 指示是否应将邮件标记为已读。 |
| markImportance | importance | 设置邮件重要性，可以是：`low`、`normal`、`high`。 |
| moveToFolder |  String| 邮件将移至其中的文件夹的 ID。 |
| permanentDelete | Boolean | 指示邮件是否应永久删除且不保存到“已删除项目”文件夹。 |
| redirectTo | [recipient](recipient.md) collection | 应将邮件重定向到的电子邮件地址。 |
| stopProcessingRules | Boolean | 指示是否应对后续规则进行评估。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

