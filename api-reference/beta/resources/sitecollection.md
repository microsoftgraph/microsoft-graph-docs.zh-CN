---
author: JeremyKelley
description: siteCollection 资源提供有关网站集的详细信息。
ms.date: 09/10/2017
title: SiteCollection
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1a2d685382eb96d332408a0f03131b5ab0cd6d02
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720824"
---
# <a name="sitecollection-resource"></a>SiteCollection 资源

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**siteCollection** 资源提供有关网站集的详细信息。

如果 [**网站**](site.md)资源具有非 NULL **siteCollection** 属性，则此网站为网站集的根网站。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
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

| 属性             | 类型     | 说明                                                                         |
| :------------------- | :------- | :---------------------------------------------------------------------------------- |
| **主机名称**         | string   | 网站集的主机名称。只读。                                    |
| **dataLocationCode** | string   | 此网站集所在的地理区域代码。 只读。       |
| **根**             | [根][] | 如果存在，则指示这是网站集中的根SharePoint。 只读。 |

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
