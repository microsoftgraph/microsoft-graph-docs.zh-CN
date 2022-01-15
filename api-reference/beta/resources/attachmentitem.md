---
title: attachmentItem 资源类型
description: 表示要附加的项目的属性。
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 236e2ed7cb26f0c8c5cd3e4ed086ab58f77087d6
ms.sourcegitcommit: 94741ff7f61f20a39dacfa6ce451a77ca02dd68a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2022
ms.locfileid: "62047232"
---
# <a name="attachmentitem-resource-type"></a>attachmentItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要附加的项目的属性。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|attachmentType|字符串| 附件的类型。 可取值为：`file`、`item`、`reference`。 此为必需属性。|
|contentId|String| 在 HTML 邮件中使用 标记的内联附件的情况下引用的附件的 CID 或 `<img src="cid:contentId">` Content-Id。 可选。|
|contentType|String|附件中数据的性质。 可选。|
|isInline|Boolean|如果附件是内嵌附件，则为 `true`；否则为 `false`。 可选。|
|name|String|附件的显示名称。 这可以是描述性字符串，不需要是实际的文件名。 必需。|
|size|Int64|附件大小，以字节为单位。 此为必需属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentId",
    "contentType",
    "isInline"
  ],
  "@odata.type": "microsoft.graph.attachmentItem",
  "baseType": null
}-->

```json
{
  "attachmentType": "String",
  "contentId": "String",
  "contentType": "String",
  "isInline": true,
  "name": "String",
  "size": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachmentItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

