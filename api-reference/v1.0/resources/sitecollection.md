---
author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
ms.localizationpriority: medium
ms.prod: sharepoint
description: siteCollection 资源提供有关网站集的详细信息。
doc_type: resourcePageType
ms.openlocfilehash: 8260970575a225b5a7fea415c783293a917e0b72
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123039"
---
# <a name="sitecollection-resource"></a>SiteCollection 资源

命名空间：microsoft.graph

**siteCollection** 资源提供有关网站集的详细信息。

如果 [**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。

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
| **dataLocationCode** | string   | 此网站集所在的地理区域代码。 只读。
| **根**             | [根][] | 如果存在，则指示这是网站集中的根SharePoint。 只读。

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/SiteCollection"
}-->

