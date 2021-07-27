---
title: teamsAppRemovedEventMessageDetail 资源类型
description: 表示有关已删除 teamsApp 的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 24d080e77d679e0e12970be2b78ea3af7b4d6668
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535706"
---
# <a name="teamsappremovedeventmessagedetail-resource-type"></a>teamsAppRemovedEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已删除 teamsApp 的事件消息的详细信息。
当从频道、聊天或团队中删除 teamsApp 时，将生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|teamsAppDisplayName|String|teamApp 的显示名称。|
|teamsAppId|String|teamsApp 的唯一标识符。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppRemovedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppRemovedEventMessageDetail",
  "teamsAppId": "String",
  "teamsAppDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关 teamsApp 已删除的事件消息的示例响应](/graph/system-messages/#teams-app-removed)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。