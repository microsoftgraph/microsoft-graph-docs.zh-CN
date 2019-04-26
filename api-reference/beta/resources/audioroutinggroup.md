---
title: audioRoutingGroup 资源类型
description: 音频路由组在多方对话中的参与者之间存储专用音频路由。 源是参与者本身, 而接收器是多方对话中的其他参与者的子集。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c5139b9f1f0c56b93848868c0d76ebf3051a148c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328249"
---
# <a name="audioroutinggroup-resource-type"></a>audioRoutingGroup 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

音频路由组在多方对话中的参与者之间存储专用音频路由。 源是参与者本身, 而接收器是多方对话中的其他参与者的子集。

> **注意:**[ConfigureMixer](../api/participant-configuremixer.md)不涉及任何路由, 而是用于设置源接收器组合的音量级别的整个调用。

## <a name="methods"></a>方法

| 方法                                                  | 返回类型                               | 说明                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [获取 audioRoutingGroup](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | 读取 audioRoutingGroup 对象的属性和关系。|
| [更新](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | 更新接收器列表。                       |
| [删除](../api/audioroutinggroup-delete.md)            | 无                                      | 删除音频路由组。              |

## <a name="properties"></a>属性

| 属性      | 类型              | 说明                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | string            | 只读。 由服务器生成。                                         |
| 接收器     | collection(string) | 接收参与者 id 的列表。                                   |
| routingMode   | string            | 路由组模式。  可取值为：`oneToOne`、`multicast`。   |
| 源       | collection(string) | 源参与者 id 的列表。                                      |

> **注意:** 路由模式确定对源和接收器的限制。 仅支持以下路由组。
> - `oneToOne`-源和接收器每个只有一个参与者。
> - `multicast`-源具有一个参与者, 但有多个接收器。 收件人列表可能会更新。

> **注意:** 如果创建了多个音频路由组 (例如, 每个参与者的 bot), 则仅转发前4个主扬声器的音频。 除了自定义的音频路由组, 如果扬声器在主混音器中的音量不足, 他/她也不会听到此扬声器和机器人的专用音频组, 即使在主混音器中没有太大的声音。

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
  "id": "string (identifier)",
  "receivers": [ "string" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "string" ]
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
  "suppressions": []
}
-->
