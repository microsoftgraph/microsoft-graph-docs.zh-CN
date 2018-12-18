---
title: audioRoutingGroup 资源类型
description: 音频路由组存储在进行多方对话中的参与者之间的专用音频路由。 源是参与者本身而接收器是进行多方对话中的其他参与者的子集。
author: VinodRavichandran
ms.openlocfilehash: 0e1db47963576e728a07a6b99ecff09a0f4640d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344469"
---
# <a name="audioroutinggroup-resource-type"></a>audioRoutingGroup 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

音频路由组存储在进行多方对话中的参与者之间的专用音频路由。 源是参与者本身而接收器是进行多方对话中的其他参与者的子集。

> **注意：**[ConfigureMixer](../api/participant-configuremixer.md)不涉及任何路由，用于整个呼叫设置源接收器组合的音量级别。

## <a name="methods"></a>方法

| 方法                                                  | 返回类型                               | 说明                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [获取 audioRoutingGroup](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | 读取属性和 audioRoutingGroup 对象的关系。|
| [Update](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | 更新接收器列表。                       |
| [删除](../api/audioroutinggroup-delete.md)            | 无                                      | 音频路由组中删除。              |

## <a name="properties"></a>属性

| 属性      | 类型              | 说明                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | String            | 只读。 生成的服务器。                                         |
| 接收器     | 字符串集合 | 接收参与者 id 的列表。                                   |
| routingMode   | 字符串            | 路由组模式。  可取值为：`oneToOne`、`multicast`。   |
| sources       | 字符串集合 | 源参与者 id 的列表。                                      |

> **注意：** 路由模式确定源和接收器的限制。 支持以下路由组。
> - `oneToOne`-源和接收器具有只有一个参与者。
> - `multicast`-源有一个参与者，但有多个接收器。 接收器列表可能会更新。

> **注意：** 如果创建许多音频路由组 （例如每个参与者自动程序），则将被转接仅顶部 4 基准扬声器的音频。 它与自定义音频路由组，即使意味着，如果扬声器不调节主混音器中，即使仅为此扬声器和自动程序的专用音频组他/她不能通过 bot 听到。

## <a name="relationships"></a>Relationships
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
<!-- {
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
