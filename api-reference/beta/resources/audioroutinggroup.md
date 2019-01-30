---
title: audioRoutingGroup 资源类型
description: 音频路由组存储在进行多方对话中的参与者之间的专用音频路由。 源是参与者本身而接收器是进行多方对话中的其他参与者的子集。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e7fc7de5b5caaa2f4079c453f9cd855a42577cb8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643169"
---
# <a name="audioroutinggroup-resource-type"></a>audioRoutingGroup 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

音频路由组存储在进行多方对话中的参与者之间的专用音频路由。 源是参与者本身而接收器是进行多方对话中的其他参与者的子集。

> **注意：**[ConfigureMixer](../api/participant-configuremixer.md)不涉及任何路由，用于整个呼叫设置源接收器组合的音量级别。

## <a name="methods"></a>方法

| 方法                                                  | 返回类型                               | 说明                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [获取 audioRoutingGroup](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | 读取属性和 audioRoutingGroup 对象的关系。|
| [更新](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | 更新接收器列表。                       |
| [删除](../api/audioroutinggroup-delete.md)            | 无                                      | 音频路由组中删除。              |

## <a name="properties"></a>属性

| 属性      | 类型              | 说明                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | String            | 只读。 由服务器生成。                                         |
| 接收器     | String 集合 | 接收参与者 id 的列表。                                   |
| routingMode   | String            | 路由组模式。  可取值为：`oneToOne`、`multicast`。   |
| sources       | String 集合 | 源参与者 id 的列表。                                      |

> **注意：** 路由模式确定源和接收器的限制。 支持以下路由组。
> - `oneToOne`-源和接收器具有只有一个参与者。
> - `multicast`-源有一个参与者，但有多个接收器。 接收器列表可能会更新。

> **注意：** 如果创建许多音频路由组 （例如每个参与者自动程序），则将被转接仅顶部 4 基准扬声器的音频。 它与自定义音频路由组，即使意味着，如果扬声器不调节主混音器中，即使仅为此扬声器和自动程序的专用音频组他/她不能通过 bot 听到。

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "String" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "String" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioroutinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
