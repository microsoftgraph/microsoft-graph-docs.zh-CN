---
title: pinnedChatMessageInfo 资源类型
description: 表示聊天实体中的单个固定消息。
author: sumanac
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d9ee744cfe71a2c9a8c05b0a8ed86c046827428d
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653603"
---
# <a name="pinnedchatmessageinfo-resource-type"></a>pinnedChatMessageInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [聊天](chat.md)中的单个固定消息。


继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出聊天中固定的消息](../api/chat-list-pinnedmessages.md)|[pinnedChatMessageInfo](../resources/pinnedchatmessageinfo.md) 集合|获取聊天中固定消息的列表。|
|[在聊天中固定消息](../api/chat-post-pinnedmessages.md)|[pinnedChatMessageInfo](../resources/pinnedchatmessageinfo.md)|在聊天中固定聊天消息。|
|[取消固定聊天中的消息](../api/chat-delete-pinnedmessages.md)|None|取消固定聊天中的消息。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| id| String| [chatMessage 的](../resources/chatmessage.md) ID。 只读。 |

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
| message | [chatMessage](../resources/chatmessage.md) | 表示有关固定的聊天消息的详细信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.pinnedChatMessageInfo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pinnedChatMessageInfo",
  "id": "String (identifier)"
}
```

