---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9147d434a94380c4d178efdf80ccba90734bf96f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939040"
---
# <a name="webpart-resource"></a>web 部件资源

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**Web 部件**资源表示类型和呈现[sitePage](sitepage.md)web 部件的信息。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a>属性

| 属性                | 类型             | 说明
|:------------------------|:-----------------|:----------------------------------
| **类型**                | 字符串           | 指定 web 部件类型的唯一标识符。 只读。
| **data**                | [sitePageData][] | 所需的 web 部件 （随 web 部件） 属性

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>备注

Web 部件可以定义在**数据**下自己所需的属性。

有关页面的详细信息，请参阅[sitePage](sitepage.md)。
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
