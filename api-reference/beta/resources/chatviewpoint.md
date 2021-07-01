---
title: chatViewpoint 资源类型
description: 表示聊天的用户特定属性。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca6a542903aae7b203c6183a25dd99889b97f275
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236295"
---
# <a name="chatviewpoint-resource-type"></a>chatViewpoint 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示聊天的特定于用户 [的属性](../resources/chat.md)。 这些属性可能会根据 API 调用方的身份而更改。

> **注意：** 目前，仅 [列表聊天](../api/chat-list.md) 操作支持 **chatViewpoint**。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastMessageReadDateTime|DateTimeOffset|表示直到呼叫用户已读取特定聊天中的 [chatMessages](../resources/chatmessage.md) 的日期/时间。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatViewpoint",
  "lastMessageReadDateTime": "String (timestamp)"
}
```

