---
title: channelModerationSettings 资源类型
description: 用于控制谁可以启动新帖子和回复频道中的帖子。
author: anandjo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 31538f7b5db717977490fa0b6e37749ef2787edd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337045"
---
# <a name="channelmoderationsettings-resource-type"></a>channelModerationSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Microsoft Teams 中，团队所有者可以打开频道的审核，以控制谁可以启动新帖子并回复该频道中的帖子。 例如，所有者可能需要执行以下操作：

- 仅对通知使用通道。
- 使用课堂团队中讨论频道，只有教师才能开始新讨论。
- 使用连接器可以启动新帖子的针对生活网站问题的通道。

默认情况下，审核为 `OFF`，这意味着常规频道设置适用于团队所有者和团队成员，具有其他控制，只允许团队成员或包括来宾在内的每个人启动新频道帖子。 将频道审阅设置为 `ON` 仅允许审阅人启动新帖子，并额外控制团队成员。

若要通过 Microsoft Graph API 支持频道审核设置，

- 团队成员应能够查询频道审核设置。
- 团队所有者应能够设置频道审核设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowNewMessageFromBots|Boolean|指示是否允许机器人发布消息。|
|allowNewMessageFromConnectors|Boolean|指示是否允许连接器发布邮件。|
|replyRestriction|replyRestriction|指示允许谁回复团队频道。 可取值为：`everyone`、`authorAndModerators`、`unknownFutureValue`。|
|userNewMessageRestriction|userNewMessageRestriction|指示允许谁向团队频道发布消息。 可能的值是：`everyone`、`everyoneExceptGuests`、`moderators`、`unknownFutureValue`。|

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

## <a name="see-also"></a>另请参阅

- 若要修改频道的审核设置，请参阅更新频道中 [的示例](../api/channel-patch.md) 2。
