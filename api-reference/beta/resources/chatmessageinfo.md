---
title: chatMessageInfo 资源类型
description: 表示 chatMessage 资源的预览。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dc03ee6743aa8115f5a231b3766cc2d6c3d5537b
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236292"
---
# <a name="chatmessageinfo-resource-type"></a>chatMessageInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [chatMessage 资源的](../resources/chatmessage.md) 预览。 此对象只能作为聊天列表的一 [部分获取](../resources/chat.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|body|[itemBody](../resources/itembody.md)|[chatMessage 的正文](../resources/chatmessage.md)。 即使对象不返回@mentions和附件，这仍将包含@mentions标记。|
|createdDateTime|DateTimeOffset|表示创建邮件的时间的日期时间对象。|
|起始数量|[chatMessageFromIdentitySet](../resources/chatmessagefromidentityset.md)|有关邮件发件人的信息。|
|id|String|[chatMessage](../resources/chatmessage.md)的 ID。|
|isDeleted|布尔值|如果设置为 `true` ，则原始邮件已删除。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageInfo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageInfo",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "from": {
    "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
  },
  "createdDateTime": "String (timestamp)",
  "isDeleted": "Boolean"
}
```

## <a name="see-also"></a>另请参阅

- [聊天](../resources/chat.md)
- [chatMessage](../resources/chatmessage.md)

