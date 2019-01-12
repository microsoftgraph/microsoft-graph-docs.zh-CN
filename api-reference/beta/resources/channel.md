---
title: 通道资源类型
description: '频道是 chatMessages 团队中的集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6529c555e418589cb757a1bc52bda520bd792745
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952326"
---
# <a name="channel-resource-type"></a>通道资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

频道是[chatMessages](chatmessage.md) [团队](../resources/team.md)中的集合。 通道表示一个主题，因此讨论，团队中的逻辑隔离。 示例可以是"星期五团队可边午餐"通道和"体系结构讨论"通道。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列表通道](../api/channel-list.md) | [通道](channel.md)集合 | 此团队中获取通道的列表。|
|[创建通道](../api/channel-post.md) | [通道](channel.md) | 创建新的通道通过包括的显示名称和说明。|
|[获取通道](../api/channel-get.md) | [通道](channel.md) | 读取属性和该频道的关系。|
|[更新通道](../api/channel-patch.md) | [通道](channel.md) | 更新该频道的属性。|
|[删除通道](../api/channel-delete.md) | 无 | 删除通道。|
|[列表通道消息](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | 在通道中收到消息 |
|[创建聊天线程](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md)集合| 创建在指定的频道的聊天线程。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|字符串|通道的可选文字说明。|
|displayName|字符串|通道名称将显示于 Microsoft 团队中的用户。|
|id|字符串|通道的唯一标识符。 只读。|
|isFavoriteByDefault|布尔|是否通道应自动标记喜欢为团队的所有成员。 默认值： `false`。|
|email|布尔| 向通道发送邮件的电子邮件地址。 只读。|
|WebUrl|String|将导航至 Microsoft 团队中的通道超链接。 这是您获取右键单击 Microsoft 团队中的通道，然后选择 Get 链接到通道时的 URL。 此 URL 应是视为不透明 blob，并且未分列。 只读。|


## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md)集合|在进入频道的所有邮件的集合。 导航属性。 可为 Null。 目前此 API 仅支持读取，但将最终太支持写入消息。|
|chatThreads|[chatThread](chatthread.md)集合|（这被淘汰以消息属性应用） chatThreads 支持创建新邮件，但未阅读邮件。 ChatThreads 是导航属性，并且是可以为 Null。|
|选项卡|[teamsTab](../resources/teamstab.md)集合|在进入频道的所有选项卡的集合。 导航属性。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
