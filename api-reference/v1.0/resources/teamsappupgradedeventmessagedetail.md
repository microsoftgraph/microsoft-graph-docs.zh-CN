---
title: teamsAppUpgradedEventMessageDetail 资源类型
description: 表示有关 teamsApp 升级的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 119b32650be32612e90134ff87e593e7132b9741
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322363"
---
# <a name="teamsappupgradedeventmessagedetail-resource-type"></a>teamsAppUpgradedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关 [teamsApp](../resources/teamsApp.md) 升级的事件消息的详细信息。
当 **teamsApp** 在频道、聊天或团队中 [](../resources/channel.md)升级 [时，将](../resources/chat.md)生成 [此消息](../resources/team.md)。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|teamsAppDisplayName|String|teamsApp 的 **显示名称**。|
|teamsAppId|String|teamsApp 的唯一 **标识符**。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppUpgradedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppUpgradedEventMessageDetail",
  "teamsAppId": "String",
  "teamsAppDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关 teamsApp 已升级的事件 **消息的示例** 响应](/graph/system-messages/#teams-app-upgraded)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
