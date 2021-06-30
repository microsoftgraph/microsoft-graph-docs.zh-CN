---
title: teamworkConversationIdentity 资源类型
description: 表示对话中的Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 84e936368b7cc4589b7611b15cf310f92b055e2a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211219"
---
# <a name="teamworkconversationidentity-resource-type"></a>teamworkConversationIdentity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 **用户 (** 聊天、团队或频道) 对话Microsoft Teams。

继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|conversationIdentityType|teamworkConversationIdentityType|对话类型。 可能的值是 `team` ：、 `channel` 和 `chat` 。|
|displayName|String|继承自 [标识](../resources/identity.md)。 对话的显示名称。 可选。|
|id|String|继承自 [标识](../resources/identity.md)。 对话的 ID。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConversationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConversationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "conversationIdentityType": "String"
}
```

