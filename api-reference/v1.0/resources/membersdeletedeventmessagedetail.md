---
title: membersDeletedEventMessageDetail 资源类型
description: 表示有关已删除成员的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0f33dfa80fc27f7eb48e00dbaa6c427f7bb30a45
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322395"
---
# <a name="membersdeletedeventmessagedetail-resource-type"></a>membersDeletedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关已删除成员的事件 [消息](../resources/conversationMember.md) 的详细信息。
当从聊天、频道或团队中删除成员时[](../resources/chat.md)，将生成[](../resources/channel.md)[此消息](../resources/team.md)。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|members|[teamworkUserIdentity](../resources/teamworkuseridentity.md) 集合|已删除 **的成员** 列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersDeletedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersDeletedEventMessageDetail",
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
- [有关已删除成员的事件 **消息的响应** 示例](/graph/system-messages/#members-deleted)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
