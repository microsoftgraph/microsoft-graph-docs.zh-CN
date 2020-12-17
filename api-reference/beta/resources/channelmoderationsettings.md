---
title: channelModerationSettings 资源类型
description: 用于控制谁可以启动新帖子和回复频道中的帖子。
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2de1c16ed998a0b793d14c6a4d791613e0bef62
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706243"
---
# <a name="channelmoderationsettings-resource-type"></a>channelModerationSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Microsoft Teams 中，团队所有者可以启用频道审核，以控制谁可以启动新帖子并回复该频道中的帖子。 例如，所有者可能希望执行以下操作：

- 仅对通知使用频道。
- 使用频道在课堂团队中讨论，只有教师才能开始新的讨论。
- 使用一个通道解决可通过连接器启动新帖子的现场问题。

默认情况下，审核是，这意味着常规频道设置适用于团队所有者和团队成员，具有其他控制，以仅允许团队成员或包括来宾在内的每个人启动新 `OFF` 频道帖子。 将频道审阅设置为仅允许审阅人启动新帖子，对团队成员 `ON` 具有其他控制。

若要通过 Microsoft Graph API 支持频道审核设置，

- 团队成员应能够查询频道审核设置。
- 团队所有者应能够设置频道审核设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowNewMessageFromBots|布尔|指示是否允许机器人发布消息。|
|allowNewMessageFromConnectors|布尔|指示是否允许连接器发布邮件。|
|replyRestriction|replyRestriction|指示允许谁回复团队频道。 可取值为：`everyone`、`authorAndModerators`、`unknownFutureValue`。|
|userNewMessageRestriction|userNewMessageRestriction|指示允许谁向团队频道发布消息。 可取值为：`everyone`、`everyoneExceptGuests`、`moderators`、`unknownFutureValue`。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelModerationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelModerationSettings",
  "userNewMessageRestriction": "String",
  "replyRestriction": "String",
  "allowNewMessageFromBots": "Boolean",
  "allowNewMessageFromConnectors": "Boolean"
}
```
