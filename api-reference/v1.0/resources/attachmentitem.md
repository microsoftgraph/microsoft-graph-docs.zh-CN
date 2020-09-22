---
title: attachmentItem 资源类型
description: 表示要附加的项的属性。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2027654cbbeab483a965cdbce8d743092ec9f379
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003274"
---
# <a name="attachmentitem-resource-type"></a>attachmentItem 资源类型

命名空间：microsoft.graph

表示要附加的项的属性。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|attachmentType|String| 附件的类型。 可取值为：`file`、`item`、`reference`。 此为必需属性。|
|contentType|String|附件中的数据的性质。 可选。|
|isInline|Boolean|如果附件是内嵌附件，则为 `true`；否则为 `false`。 可选。|
|name|String|附件的显示名称。 它可以是描述性字符串，不必是实际的文件名。 必需。|
|size|Int64|附件大小，以字节为单位。 此为必需属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentType",
    "isInline"
  ],
  "@odata.type": "microsoft.graph.attachmentItem",
  "baseType": null
}-->

```json
{
  "attachmentType": "String",
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
