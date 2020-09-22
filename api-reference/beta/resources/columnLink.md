---
author: daspek
description: contentType 上的 columnLink 将网站 columnDefinition 附加到该内容类型。
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f60392954cb1a214327edd4ffcc65449c6d976f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034061"
---
# <a name="columnlink-resource-type"></a>ColumnLink 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。

[contentType]: contenttype.md

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": []
}
-->


