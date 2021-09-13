---
title: teamworkConversationIdentity 资源类型
description: 表示对话中的Microsoft Teams。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a463f37152b6d2108ac6ca04d9971cb908d6ba4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59055827"
---
# <a name="teamworkconversationidentity-resource-type"></a>teamworkConversationIdentity 资源类型

命名空间：microsoft.graph

代表 **用户 (** 聊天、团队或频道) 对话Microsoft Teams。

继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|conversationIdentityType|teamworkConversationIdentityType|对话类型。 可能的值为： `team`、 `channel`、 `chat`和 `unknownFutureValue`。|
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

