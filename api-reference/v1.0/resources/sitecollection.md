---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: siteCollection 资源提供有关网站集的详细信息。
doc_type: resourcePageType
ms.openlocfilehash: f4444d4dcc78ee3a0cfe6e74d7fcb6616d9084e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036959"
---
# <a name="sitecollection-resource"></a>SiteCollection 资源

命名空间：microsoft.graph

**siteCollection** 资源提供有关网站集的详细信息。

如果[**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a>属性

| 属性名称        | 类型     | 说明
|:---------------------|:---------|:---------------------------------------------------
| **主机名称**         | string   | 网站集的主机名称。只读。
| **dataLocationCode** | 字符串   | 此网站集所在位置的地理区域代码。 只读。
| **根**             | [根][] | 如果存在，则表示这是 SharePoint 中的根网站集。 只读。

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->

