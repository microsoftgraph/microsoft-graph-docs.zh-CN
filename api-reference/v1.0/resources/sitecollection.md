---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 84de2a8aa6796051b3b11ebec0d0f8f5934ea1fc
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "19069341"
---
# <a name="sitecollection-resource"></a>SiteCollection 资源

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
| **主机名称**         | 字符串   | 网站集的主机名称。只读。
| **root**             | [root][] | 如果存在此参数，指示这是 SharePoint 中的根网站集。 只读。

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
