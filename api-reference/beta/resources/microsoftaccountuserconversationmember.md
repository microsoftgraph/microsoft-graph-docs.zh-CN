---
title: microsoftAccountUserConversationMember 资源类型
description: 表示聊天中的个人 Microsoft 帐户用户。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6d68d9bf9aa32bbb0965f5a892cd923627266c8e
ms.sourcegitcommit: 096bad7aaaa5d9b5ce698a524cb21f4070c7b4d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2022
ms.locfileid: "62056375"
---
# <a name="microsoftaccountuserconversationmember-resource-type"></a>microsoftAccountUserConversationMember 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示聊天中的个人 Microsoft 帐户用户。


继承自 [conversationMember](../resources/conversationmember.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|用户的显示名称。 继承自 [conversationMember](../resources/conversationmember.md)。|
|id|String|表示此资源的成员身份 ID。 继承自 [实体](../resources/entity.md)。|
|角色|String 集合|此用户的特殊角色。 继承自 [conversationMember](../resources/conversationmember.md)。|
|userId|String|用户的 ID。|
|visibleHistoryStartDateTime|DateTimeOffset|表示对话历史久远程度的时间戳与对话成员共享。 继承自 [conversationMember](../resources/conversationmember.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAccountUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAccountUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "userId": "String"
}
```

