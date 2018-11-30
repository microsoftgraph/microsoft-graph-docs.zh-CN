---
title: locationConstraintItem 资源类型
description: 客户端声明的会议地点条件。
ms.openlocfilehash: f29ff1283d876e726e27473485a183956137f981
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041786"
---
# <a name="locationconstraintitem-resource-type"></a>locationConstraintItem 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

客户端声明的会议地点条件。

由 [location](location.md) 派生。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  
  ],
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| address | [physicalAddress](physicaladdress.md) |位置的街道地址。 |
| coordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | 地理坐标和位置的海拔高度。 |
| displayName  | String | 与地点相关联的名称。                       |
| locationEmailAddress | String | （可选）与位置相关联的电子邮件地址。 |
| locationUri | String | （可选）表示位置的 URI。 |
| resolveAvailability | Boolean | 如果设为 true，且指定的资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 会查找另一空闲资源。如果设为 false，且指定的资源处于忙碌状态，**findMeetingTimes** 会返回用户缓存中排名最靠前的资源，而不会检查其是否空闲。默认值为 true。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->