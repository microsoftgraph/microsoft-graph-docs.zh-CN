---
title: conversationMemberRoleUpdatedEventMessageDetail 资源类型
description: 表示有关频道或团队中对话成员更新角色的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2c91e2a476b048c6d451c31c96ac95a3756bbbe4
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322396"
---
# <a name="conversationmemberroleupdatedeventmessagedetail-resource-type"></a>conversationMemberRoleUpdatedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关频道或团队中对话成员已更新[角色的事件](../resources/channel.md)消息[](../resources/conversationMember.md)[的详细信息](../resources/team.md)。
更新频道或团队 **中成员的角色****时，** 将生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|conversationMemberRoles|字符串集合|覆盖成员 **用户** 的角色。|
|conversationMemberUser|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|对话成员 **用户的** 标识。|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conversationMemberRoleUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversationMemberRoleUpdatedEventMessageDetail",
  "conversationMemberRoles": [
    "String"
  ],
  "converstaionMemberUser": {
    "@odata.type": "microsoft.graph.teamworkUserIdentity"
  },
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关频道或团队中对话 **成员更新角色** 的事件 **消息的响应****示例**](/graph/system-messages/#conversation-member-role-updated)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
