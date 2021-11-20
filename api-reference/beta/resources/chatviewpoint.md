---
title: chatViewpoint 资源类型
description: 表示聊天的用户特定属性。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d9efb70dec447bf2f3c504a05245f67944783f6
ms.sourcegitcommit: 70b3caded085ba8ef15e389f81fa005506f1e2fb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2021
ms.locfileid: "61131922"
---
# <a name="chatviewpoint-resource-type"></a>chatViewpoint 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示聊天的特定于用户 [的属性](../resources/chat.md)。 这些属性可能会根据 API 调用方的身份而更改。

> **注意：** 目前，仅 ["列表"聊天](../api/chat-list.md) 操作支持 **chatViewpoint**。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|IsHidden|布尔值|指示当前用户是否隐藏聊天。|
|lastMessageReadDateTime|DateTimeOffset|表示直到当前用户已读取特定聊天中的 [chatMessages](../resources/chatmessage.md) 的日期/时间。|

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
  "isHidden": "Boolean",
  "lastMessageReadDateTime": "String (timestamp)"
}
```

