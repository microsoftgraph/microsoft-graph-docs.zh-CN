---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 03b5f1007d8dbe6587da736cdf0ac0fdc1ed8a55
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345784"
---
# <a name="webpart-resource"></a>webPart 资源

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**webPart**资源表示[sitePage](sitepage.md)上的 web 部件的类型和呈现信息。

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
| **类型**                | String           | 指定 web 部件类型的唯一标识符。 只读。
| **data**                | [sitePageData][] | web 部件的必需属性 (因 web 部件而异)

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>注解

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
