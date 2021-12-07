---
title: membersLeftEventMessageDetail 资源类型
description: 表示有关左侧成员的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7fd75e032e58a2254cc9f9965360c2d3a9327759
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322356"
---
# <a name="memberslefteventmessagedetail-resource-type"></a>membersLeftEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关左侧成员的事件 [消息](../resources/conversationMember.md) 的详细信息。
当成员离开会议 **聊天** 时，将生成 [此消息](../resources/chat.md)。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|members|[teamworkUserIdentity](../resources/teamworkuseridentity.md) 集合|离开 **聊天** 的成员 **列表**。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersLeftEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersLeftEventMessageDetail",
  "members": [
    {
      "@odata.type": "microsoft.graph.teamworkUserIdentity"
    }
  ],
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关左侧成员的事件消息 **的示例** 响应](/graph/system-messages/#members-left)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
