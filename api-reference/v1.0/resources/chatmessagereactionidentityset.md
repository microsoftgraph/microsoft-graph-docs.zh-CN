---
title: chatMessageReactionIdentitySet 资源类型
description: 表示对聊天或频道中的消息做出响应的用户。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 35b97d1b7fe470beced8daca4b92f5e1c167b467
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109393"
---
# <a name="chatmessagereactionidentityset-resource-type"></a>chatMessageReactionIdentitySet 资源类型

命名空间：microsoft.graph

表示 **对** 聊天 [或频道中](../resources/chatmessage.md) 的消息做出响应的用户。 仅 `user` 属性具有值。


继承自 [identitySet](../resources/identityset.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|application|[Identity](../resources/identity.md)|继承自 [identitySet](../resources/identityset.md)。 未设置，因为应用程序无法对消息做出反应。|
|设备|[identity](../resources/identity.md)|继承自 [identitySet](../resources/identityset.md)。 未设置，因为设备无法对消息做出反应。|
|用户|[identity](../resources/identity.md)|继承自 [identitySet](../resources/identityset.md)。 有关对邮件做出响应的用户的详细信息。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageReactionIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageReactionIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

