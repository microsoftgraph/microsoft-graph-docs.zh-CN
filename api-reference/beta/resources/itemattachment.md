---
title: itemAttachment 资源类型
description: 附加到其他事件的联系人、事件或邮件，
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: db57bbad71349af6b40b16c88941444d6bac200e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133782"
---
# <a name="itemattachment-resource-type"></a>itemAttachment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

附加到用户事件、邮件[、Outlook](../resources/outlooktask.md)任务或帖子的联系人、[](../resources/event.md)事件或[](../resources/message.md)[邮件](../resources/post.md)。  

派生自 [附件](attachment.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [itemAttachment](itemattachment.md) |读取 itemAttachment 对象的属性、关系或原始内容。|
|[删除](../api/attachment-delete.md) | 无 |删除 itemAttachment 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contentType|String|附件的内容类型。|
|id|String| 附件 ID。|
|isInline|Boolean|如果附件是内联的（例如嵌入到项目正文中的图像），请设置为 true。|
|lastModifiedDateTime|DateTimeOffset|上次修改附件的时间和日期。|
|name|String|附件的显示名称。|
|大小|Int32|附件大小，以字节为单位。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|项|[OutlookItem](outlookitem.md)|附加的联系人、邮件或事件。导航属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "optionalProperties": [
    "item"
  ],
  "@odata.type": "microsoft.graph.itemAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


