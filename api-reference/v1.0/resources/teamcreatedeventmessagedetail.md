---
title: teamCreatedEventMessageDetail 资源类型
description: 表示有关已创建团队的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c60ceda4f89832671700ed929bc80b5cb0078edf
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322367"
---
# <a name="teamcreatedeventmessagedetail-resource-type"></a>teamCreatedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关已创建团队的事件消息 [的详细信息](../resources/team.md)。
创建团队时将 **生成** 此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|teamDescription|String|团队 **的说明**。|
|teamDisplayName|String|团队的显示 **名称**。|
|teamId|String|团队的唯一 **标识符**。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamCreatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamCreatedEventMessageDetail",
  "teamId": "String",
  "teamDisplayName": "String",
  "teamDescription": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关已创建团队的事件消息的示例 **响应**](/graph/system-messages/#team-created)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
