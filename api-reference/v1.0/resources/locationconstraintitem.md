---
title: locationConstraintItem 资源类型
description: locationConstraintItem - 客户端为会议位置声明的条件。
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: fb5828e603c9a5dc2ef0f66d6d00b8c5fe7741ed
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900343"
---
# <a name="locationconstraintitem-resource-type"></a>locationConstraintItem 资源类型

命名空间：microsoft.graph

客户端声明的会议地点条件。

由 [location](location.md) 派生。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.location",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| address | [physicalAddress](physicaladdress.md) |位置的街道地址。 |
| displayName  | String | 与地点相关联的名称。                       |
| locationEmailAddress | String | （可选）与地点相关联的电子邮件地址。 |
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

