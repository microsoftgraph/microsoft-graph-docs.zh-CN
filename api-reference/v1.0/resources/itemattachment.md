---
title: itemAttachment 资源类型
description: '附加到另一事件、邮件或帖子的联系人、事件或邮件。  '
localization_priority: Priority
ms.prod: outlook
author: abheek-das
doc_type: resourcePageType
ms.openlocfilehash: 07bf925b83be912f0ed50fb072fb2deadc59e0e18729c13ea76acd975a9193ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192220"
---
# <a name="itemattachment-resource-type"></a>itemAttachment 资源类型

命名空间：microsoft.graph

附加到用户[事件](../resources/event.md)、[邮件](../resources/message.md)或[帖子](../resources/post.md)的联系人、事件或邮件。  

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
|项|[OutlookItem](outlookitem.md)|附加的消息或事件。导航属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

