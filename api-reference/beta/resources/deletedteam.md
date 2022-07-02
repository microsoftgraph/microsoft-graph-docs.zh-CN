---
title: deletedTeam 资源类型
description: 表示 Microsoft Teams 中的已删除团队。
author: agnesliu
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: de027a7e224db03f72fe424c1a4e08f5d238bea7
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66578118"
---
# <a name="deletedteam-resource-type"></a>deletedTeam 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft Teams 中的已删除 [团队](../resources/team.md)。

每个已删除团队都与 [Microsoft 365 组](../resources/group.md) 关联。 有关使用组和团队内部成员的详细信息，请参阅 [使用 Microsoft Graph API 处理 Microsoft Teams](teams-api-overview.md)。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[getAllMessages](../api/deletedteam-getallmessages.md)|[chatMessage](../resources/chatmessage.md) 集合|检索 [已删除团队](../resources/deletedteam.md) 中跨所有 [频道](../resources/channel.md) 的全部 [消息](../resources/chatmessage.md)。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|已删除团队的 ID。 继承自 [entity](../resources/entity.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|channels|[channel](../resources/channel.md) 集合|这些频道是与此已删除的团队共享的，或是在此已删除团队中创建的。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deletedTeam",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
    "@odata.type": "#microsoft.graph.deletedTeam",
    "id": "String (identifier)"
}
```

