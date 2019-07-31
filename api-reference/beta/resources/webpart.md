---
author: rahmit
description: WebPart 资源表示 sitePage 上的 web 部件的类型和呈现信息。
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71626440abe9eb63af3419b3e65c4351ae442dea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007352"
---
# <a name="webpart-resource"></a>webPart 资源

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
| **data**                | [sitePageData][] | Web 部件的必需属性 (因 Web 部件而异)

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>说明

Web 部件可以在**data**下定义自己的必需属性。

有关页面的详细信息, 请参阅[sitePage](sitepage.md)。
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
