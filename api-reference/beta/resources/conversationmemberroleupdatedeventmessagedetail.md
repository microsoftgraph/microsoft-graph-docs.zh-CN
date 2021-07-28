---
title: conversationMemberRoleUpdatedEventMessageDetail 资源类型
description: 表示有关频道或团队中对话成员更新角色的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2ab15ff8f874ffeaa4424f29b8cc452ae128ae2c
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534307"
---
# <a name="conversationmemberroleupdatedeventmessagedetail-resource-type"></a>conversationMemberRoleUpdatedEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关频道或团队中对话成员更新角色的事件消息的详细信息。
更新频道或团队中成员的角色时，将生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|conversationMemberRoles|字符串集合|覆盖成员用户的角色。|
|conversationMemberUser|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|对话成员用户的标识。|
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
- [有关频道或团队中对话成员已更新角色的事件消息的示例响应](/graph/system-messages/#conversation-member-role-updated)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。