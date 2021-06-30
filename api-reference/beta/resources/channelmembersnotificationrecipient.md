---
title: channelMembersNotificationRecipient 资源类型
description: 表示在活动源中发送的通知Microsoft Teams收件人。 收件人由频道成员组成。
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 821d4f2ee41c15cb93cd3d53b9af9cf1e63db97b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211286"
---
# <a name="channelmembersnotificationrecipient-resource-type"></a>channelMembersNotificationRecipient 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在活动源中发送的通知Microsoft Teams收件人。 收件人由频道成员组成。

继承自 [teamworkNotificationRecipient](teamworknotificationrecipient.md)。

## <a name="properties"></a>属性
| 属性  | 类型   | 说明                                            |
| :-------- | :----- | :----------------------------------------------------- |
| teamId    | String | 频道所在的团队的标识符。 |
| channelId | String | 频道的标识符。                              |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.channelMembersNotificationRecipient",
  "teamId": "String",
  "channelId": "String"
}
```
