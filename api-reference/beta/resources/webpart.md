---
author: rahmit
description: WebPart 资源表示 sitePage 上的 web 部件的类型和呈现信息。
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b69762298f4f165ac18e4e0137dd979bde176652
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973470"
---
# <a name="webpart-resource"></a>webPart 资源

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**WebPart**资源表示[sitePage](sitepage.md)上的 web 部件的类型和呈现信息。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (identifier)",
  "data": {"@odata.type":"microsoft.graph.sitePageData"}
}
```

## <a name="properties"></a>属性

| 属性                | 类型             | 说明
|:------------------------|:-----------------|:----------------------------------
| **类型**                | String           | 指定 Web 部件类型的唯一标识符。 只读。
| **data**                | [sitePageData][] | Web 部件 (的必需属性因 Web 部件而异) 

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>说明

Web 部件可以在 **data**下定义自己的必需属性。

有关页面的详细信息，请参阅 [sitePage](sitepage.md)。
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": []
}
-->


