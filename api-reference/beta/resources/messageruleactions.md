---
title: messageRuleActions 资源类型
description: 表示适用于规则的一组操作。
ms.openlocfilehash: fbd189d8a43dc47e139f69cd345b4c14744d94f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042271"
---
# <a name="messageruleactions-resource-type"></a>messageRuleActions 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
| markImportance | String | 设置邮件重要性，可以是：`low`、`normal`、`high`。 |
| moveToFolder |  String| 邮件将移至其中的文件夹的 ID。 |
| permanentDelete | Boolean | 指示邮件是否应永久删除且不保存到“已删除项目”文件夹。 |
| redirectTo | [recipient](recipient.md) | 邮件应重定向到的电子邮件地址。 |
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
  "redirectTo": {"@odata.type": "microsoft.graph.recipient"},
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