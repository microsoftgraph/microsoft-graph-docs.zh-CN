---
title: anonymousGuestConversationMember 资源类型
description: 表示聊天中的匿名来宾。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f439daa2e5146b37b94862e2dce87a2efb603f02
ms.sourcegitcommit: 096bad7aaaa5d9b5ce698a524cb21f4070c7b4d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2022
ms.locfileid: "62056356"
---
# <a name="anonymousguestconversationmember-resource-type"></a>anonymousGuestConversationMember 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示聊天中的匿名来宾。 

匿名用户没有标识Microsoft Teams，并且可以使用会议加入链接加入会议。 有关详细信息，请参阅匿名 [用户](/microsoftteams/non-standard-users#anonymous-users)。


继承自 [conversationMember](../resources/conversationmember.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|anonymousGuestId|String|表示用户的唯一 ID。 **注意：** 如果用户离开和重新加入会议，或者从其他设备加入会议，此 ID 可能会更改。|
|displayName|String|用户在加入会议时提供的名称。 继承自 [conversationMember](../resources/conversationmember.md)。|
|id|String|表示此资源的成员身份 ID。 继承自 [实体](../resources/entity.md)。|
|角色|String 集合|此用户的特殊角色。 继承自 [conversationMember](../resources/conversationmember.md)。|
|visibleHistoryStartDateTime|DateTimeOffset|表示对话历史久远程度的时间戳与对话成员共享。 继承自 [conversationMember](../resources/conversationmember.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.anonymousGuestConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.anonymousGuestConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "anonymousGuestId": "String"
}
```

