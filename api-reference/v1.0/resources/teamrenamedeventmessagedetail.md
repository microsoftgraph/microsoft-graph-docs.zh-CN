---
title: teamRenamedEventMessageDetail 资源类型
description: 表示有关重命名团队的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c1569be468116d539d0144519d0225975abf004b
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322359"
---
# <a name="teamrenamedeventmessagedetail-resource-type"></a>teamRenamedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关重命名的团队的事件消息 [的详细信息](../resources/team.md)。
更新团队名称 **时，将** 生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|teamDisplayName|String|更新的团队 **名称**。|
|teamId|String|团队的唯一 **标识符**。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamRenamedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamRenamedEventMessageDetail",
  "teamId": "String",
  "teamDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关重命名团队的事件消息的响应 **示例**](/graph/system-messages/#team-renamed)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
