---
title: chatMessageIdentitySet 资源类型
description: 表示聊天@mentioned频道中的消息中的资源资源。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: bf19b34143935f66ab835cd12a47881bc0b1b1b2aa1f960d1d35f4be3d2ed41a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238151"
---
# <a name="chatmessagementionedidentityset-resource-type"></a>chatMessageIdentitySet 资源类型

命名空间：microsoft.graph

表示用户 (、应用程序或对话) @mentioned聊天或频道中的消息中的资源资源。 [](../resources/chatmessage.md)


继承自 [identitySet](../resources/identityset.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|application|[Identity](../resources/identity.md)|继承自 [identitySet](../resources/identityset.md)。 如果存在，表示应用程序 (例如，自动程序) @mentioned消息 [中的自动程序](../resources/chatmessage.md)。|
|conversation|[teamworkConversationIdentity](../resources/teamworkconversationidentity.md)|如果存在，表示对话 (例如，团队或频道) @mentioned消息 [中](../resources/chatmessage.md)。|
|设备|[identity](../resources/identity.md)|继承自 [identitySet](../resources/identityset.md)。 由于不支持在设备上使用@mention使用。|
|用户|[identity](../resources/identity.md)|继承自 [identitySet](../resources/identityset.md)。 如果存在，表示用户@mentioned消息[中显示。](../resources/chatmessage.md)|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMentionedIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageMentionedIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  },
  "conversation": {
    "@odata.type": "microsoft.graph.teamworkConversationIdentity"
  }
}
```