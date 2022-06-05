---
title: locationConstraint 资源类型
description: 客户端声明的会议地点条件。
ms.localizationpriority: medium
author: harini84
ms.prod: calendar
doc_type: resourcePageType
ms.openlocfilehash: 5381c688f007a6c9d30deccf384ae70a98492c43
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898488"
---
# <a name="locationconstraint-resource-type"></a>locationConstraint 资源类型

命名空间：microsoft.graph

客户端声明的会议地点条件。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|isRequired|Boolean|客户端请求服务在响应中添加会议地点。若为 true，且所有资源处于忙碌状态，[findMeetingTimes](../api/user-findmeetingtimes.md) 将不会返回任何会议时间建议。若为 false，且所有资源处于忙碌状态，**findMeetingTimes** 仍会在没有会议地点的情况下查找会议时间。 |
|locations|[locationConstraintItem](locationconstraintitem.md) 集合|客户端请求的一个或多个会议地点的约束信息。|
|suggestLocation|Boolean|客户端请求服务返回一个或多个会议地点建议。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

