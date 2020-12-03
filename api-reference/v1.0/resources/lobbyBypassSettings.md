---
title: lobbyBypassSettings 资源类型
description: 指定哪些参与者可以绕过会议厅。
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 761a45ce5c4e29d06287edb18aa8d79256c08923
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523159"
---
# <a name="lobbybypasssettings-resource-type"></a>lobbyBypassSettings 资源类型

命名空间：microsoft.graph

指定哪些参与者可以绕过会议厅。

## <a name="properties"></a>属性

| 属性              | 类型             | 说明                                                                                                                                                          |
| --------------------- | ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| scope                 | lobbyBypassScope | 指定自动获准加入会议的参与者的类型（绕会议厅）。 下表中列出了可能的值。 可选。 |
| isDialInBypassEnabled | 布尔值          | 指定是否始终让拨入呼叫者绕过会议厅。 可选。                                                                                   |

### <a name="lobbybypassscope-values"></a>lobbyBypassScope 值

| 值                    | 说明                                                                                                                                                                     |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 组织者                | 绕过会议厅，仅允许组织者进入会议。 所有其他参与者都将放入会议厅中。                                                   |
| 组织             | 只有来自同一公司的参与者才会绕过大厅获准参加会议。 所有其他参与者都将放入会议厅中。                         |
| organizationAndFederated | 只有来自同一家公司或受信任组织的参与者才会被允许加入会议，从而绕过会议厅。 所有其他参与者都将放入会议厅中。 |
| 成员                 | 允许所有人参加会议。 不会在会议厅中放置任何参与者。                                                                                         |
| 向 unknownfuturevalue       | Unknow 未来值。                                                                                                                                                            |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "String",
  "isDialInBypassEnabled": "Boolean",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "lobbyBypassSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
