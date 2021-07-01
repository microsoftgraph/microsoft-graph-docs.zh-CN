---
title: chatMessageFromIdentitySet 资源类型
description: 表示聊天或频道中消息的发送方。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 30b8c8add62c94ff16fe5e560a78ec5c9c95627d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211075"
---
# <a name="chatmessagefromidentityset-resource-type"></a>chatMessageFromIdentitySet 资源类型

命名空间：microsoft.graph

表示聊天 [或](../resources/chatmessage.md) 频道中消息的发送方。 此对象可能适用于内部系统已删除或发送Microsoft Teams的邮件;例如，用于添加 `null` 成员的事件消息。


继承自 [identitySet](../resources/identityset.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|application|[Identity](../resources/identity.md)|继承自 [identitySet](../resources/identityset.md)。 如果存在，表示应用程序 (例如，自动程序) 发送消息。|
|设备|[identity](../resources/identity.md)|继承自 [identitySet](../resources/identityset.md)。 未使用。|
|user|[identity](../resources/identity.md)|继承自 [identitySet](../resources/identityset.md)。 如果存在，表示发送消息的用户。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageFromIdentitySet",
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

