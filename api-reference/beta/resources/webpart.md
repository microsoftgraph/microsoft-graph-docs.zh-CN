---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453607"
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
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a>属性

| 属性                | 类型             | 描述
|:------------------------|:-----------------|:----------------------------------
| **类型**                | 字符串           | 指定 web 部件类型的唯一标识符。 只读。
| **data**                | [sitePageData][] | web 部件的必需属性 (因 web 部件而异)

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>备注

Web 部件可以在**data**下定义自己的必需属性。

有关页面的详细信息, 请参阅[sitePage](sitepage.md)。
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": [
    "Error: /api-reference/beta/resources/webpart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
