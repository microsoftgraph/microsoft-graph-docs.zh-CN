---
title: teamsTab 资源类型
description: 'teamsTab 是固定到团队 () 频道的选项卡。 '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 38351b0bde174b03f0e01392e7c8ec9c4df0db44
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660112"
---
# <a name="teamstab-resource-type"></a>teamsTab 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

teamsTab[是固定](../resources/teamstab.md)到团队 () 频道的[](channel.md)[选项卡](team.md)。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出频道中的选项卡](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | 列出固定到频道的选项卡。|
|[获取频道中的选项卡](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | 获取固定到频道的特定选项卡。|
|[将选项卡添加到频道](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | 将选项卡添加（固定）到频道。|
|[更新频道中的选项卡](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | 更新频道中的选项卡的属性。|
|[从频道中删除选项卡](../api/channel-delete-tabs.md) | 无 | 从频道中删除（取消固定）选项卡。|
|[列出聊天中的选项卡](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | 列出固定到聊天的选项卡。|
|[获取聊天中的选项卡](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | 获取固定到聊天的特定选项卡。|
|[向聊天添加选项卡](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | 将 (固定) 选项卡添加到聊天中。|
|[聊天中的"更新"选项卡](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | 更新聊天中选项卡的属性。|
|[从聊天中删除选项卡](../api/chat-delete-tabs.md) | 无 | 从 (选项卡) 取消固定。|



## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|  id              |   string                  |  唯一标识通道选项卡的特定实例的标识符。只读。     |
|  displayName            |   string                  |  选项卡的名称。     |
|  名称 (已弃)       |   string                  |  选项卡的名称。     |
|  teamsAppId (已弃用) |   string             |  选项卡的应用定义标识符。创建选项卡后无法更改此值。 由于此属性已弃用，我们建议扩展 **teamsApp** 以检索链接到选项卡的应用程序。 |
|  sortOrderIndex  |   string                  |  用于对选项卡进行排序的顺序的索引。     |
|  webUrl          |   string                  |  选项卡实例的深层链接 URL。 只读。     |
|  configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  应用于选项卡的自定义设置的容器。只有在设置此属性后，选项卡才被视为已配置。     |

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | 链接到选项卡的应用程序。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration": "teamsTabConfiguration",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a>另请参阅

[配置内置选项卡类型](/graph/teams-configuring-builtin-tabs)


