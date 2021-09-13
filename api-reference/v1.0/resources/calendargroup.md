---
title: calendarGroup 资源类型
description: 一组用户日历。
author: harini84
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ca67a29dd6c48119442423570a08b66dd5a83f9b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129962"
---
# <a name="calendargroup-resource-type"></a>calendarGroup 资源类型

命名空间：microsoft.graph

一组用户日历。

## <a name="methods"></a>方法

| 方法                                                      | 返回类型                        | 说明                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [列出日历组](../api/user-list-calendargroups.md)  | [日历](calendar.md) 集合 | 获取用户的日历组。                               |
| [创建日历组](../api/user-post-calendargroups.md) | [日历](calendar.md)            | 创建新的日历组。                                  |
| [创建日历组](../api/calendargroup-get.md)           | [calendarGroup](calendargroup.md)  | 读取 calendar 对象的属性和关系。 |
| [更新](../api/calendargroup-update.md)                    | [calendarGroup](calendargroup.md)  | 更新 calendarGroup 对象。                                  |
| [删除](../api/calendargroup-delete.md)                    | 无                               | 删除 calendarGroup 对象。                                  |
| [List calendars](../api/calendargroup-list-calendars.md)    | [Calendar](calendar.md) collection | 列出日历组中的日历。                           |
| [创建日历](../api/calendargroup-post-calendars.md)   | [日历](calendar.md)            | 在日历组中创建新日历。                    |

## <a name="properties"></a>属性

| 属性  | 类型   | 说明                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| name      | String | 组名称。                                                                                                                                                                                           |
| changeKey | String | 标识日历组的版本。每次日历组更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。 |
| classId   | Guid   | 类标识符。只读。                                                                                                                                                                          |
| id        | String | 组的唯一标识符。只读。                                                                                                                                                                 |

## <a name="relationships"></a>关系

| 关系 | 类型                               | 说明                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| calendars    | [Calendar](calendar.md) collection | 日历组中的日历。导航属性。只读。可为 Null。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendarGroup",
  "@odata.annotations": [
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

