---
title: itemAttachment 资源类型
description: 附加到另一个事件的联系人、事件或邮件,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: b4220a1428edab2eeab89cabe53efc91bea76a8b
ms.sourcegitcommit: 496269b62d42cb7a96752a77b0f2e0cb16918f0b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2019
ms.locfileid: "36484378"
---
# <a name="itemattachment-resource-type"></a>itemAttachment 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

附加到另一个[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[公告](../resources/post.md)的联系人、事件或邮件。  

派生自 [附件](attachment.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [itemAttachment](itemattachment.md) |读取 itemAttachment 对象的属性和关系。|
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
|项|[OutlookItem](outlookitem.md)|附加的联系人、消息或事件。 导航属性。|

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
