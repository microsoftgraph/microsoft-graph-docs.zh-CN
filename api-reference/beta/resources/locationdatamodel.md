---
title: locationDataModel 资源类型
description: 表示事件的 locationDataModel 信息。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2b1fd0c25cdd41e6a8d9c87f8a1c0c80d70b78e5
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057343"
---
# <a name="locationdatamodel-resource-type"></a>locationDataModel 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示会议的位置信息。


## <a name="properties"></a>属性
| 属性  | 类型   | 说明                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| address | [省略](postaladdress.md) |位置的街道地址。 |
| coordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | 地理坐标和位置的海拔高度。 |
| displayName  | 字符串 | 与地点相关联的名称。                       |
| locationEmailAddress | String | （可选）与位置相关联的电子邮件地址。 |
| locationUri | String | （可选）表示位置的 URI。 |


## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationDataModel"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationdatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
