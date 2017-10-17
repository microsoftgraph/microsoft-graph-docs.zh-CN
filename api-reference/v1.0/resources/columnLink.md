---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: ef7fef6fb6ca35f1117433b452de0841691282a0
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="columnlink-resource-type"></a>ColumnLink 资源类型

[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。

[contentType]: contentType.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **columnLink** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| **id**        | string | 列的唯一标识符。
| **name**      | string | 此内容类型中的列的名称。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
