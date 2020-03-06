---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: siteCollection 资源提供有关网站集的详细信息。
doc_type: resourcePageType
ms.openlocfilehash: 2e34b4fdb63a825e87cea8eda6117232ee1da93d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533688"
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
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a>属性

| 属性名称        | 类型     | 说明
|:---------------------|:---------|:---------------------------------------------------
| **主机名称**         | string   | 网站集的主机名称。只读。
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
