---
title: teamsAppUpgradedEventMessageDetail 资源类型
description: 表示有关 teamsApp 升级的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4bca8bbb7c218333d72cb290e508b352fd977f2d
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535705"
---
# <a name="teamsappupgradedeventmessagedetail-resource-type"></a>teamsAppUpgradedEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关 teamsApp 升级的事件消息的详细信息。
当 teamsApp 在频道、聊天或团队中升级时，将生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|teamsAppDisplayName|String|teamsApp 的显示名称。|
|teamsAppId|String|teamsApp 的唯一标识符。|

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
- [有关 teamsApp 已升级的事件消息的示例响应](/graph/system-messages/#teams-app-upgraded)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。