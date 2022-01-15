---
title: skypeForBusinessUserConversationMember 资源类型
description: 表示Skype for Business聊天中的用户
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3badca1cb93a2e001e31bb9280a1a213f5be7805
ms.sourcegitcommit: 096bad7aaaa5d9b5ce698a524cb21f4070c7b4d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2022
ms.locfileid: "62056354"
---
# <a name="skypeforbusinessuserconversationmember-resource-type"></a>skypeForBusinessUserConversationMember 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Skype for Business用户。 

有关实现Teams和Skype for Business的信息，请参阅了解Microsoft Teams[和Skype for Business共存和互操作性](/microsoftteams/teams-and-skypeforbusiness-coexistence-and-interoperability)。

继承自 [conversationMember](../resources/conversationmember.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|用户的显示名称。 继承自 [conversationMember](../resources/conversationmember.md)。|
|id|字符串|表示此资源的成员身份 ID。 继承自 [实体](../resources/entity.md)。|
|角色|String 集合|此用户的特殊角色。 继承自 [conversationMember](../resources/conversationmember.md)。|
|tenantId|字符串|用户所属的租户的 ID。|
|userId|String|用户的 ID。|
|visibleHistoryStartDateTime|DateTimeOffset|表示对话历史久远程度的时间戳与对话成员共享。 继承自 [conversationMember](../resources/conversationmember.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeForBusinessUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "userId": "String",
  "tenantId": "String"
}
```

