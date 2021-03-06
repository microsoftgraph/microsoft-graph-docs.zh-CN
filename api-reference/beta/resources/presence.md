---
title: 状态资源类型
description: 包含有关用户状态的信息，包括其可用性和用户活动。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: d6f88f23a6c08d5aa757163d4956c104a603e87b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515623"
---
# <a name="presence-resource-type"></a>状态资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关用户状态的信息，包括其可用性和用户活动。

> **注意：** 此资源当前仅受 Microsoft Teams 用户支持。

此资源支持订阅 [更改通知](/graph/webhooks)。

## <a name="methods"></a>方法

| 方法                                                            | 返回类型                                       | 说明                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [获取状态](../api/presence-get.md)     | [状态](../resources/presence.md)     | 获取用户状态信息。
| [获取多个用户状态](../api/cloudcommunications-getpresencesbyuserid.md)    |  [presence](../resources/presence.md) 集合     |  获取多个用户状态信息。      |


## <a name="properties"></a>属性

| 关系        | 类型                                                 | 说明                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|id    |  string     |  用户对象 ID   |
|availability    |  字符串集合   |   用户的基本状态信息。 可能的值是 `Available` ， ， ， ， ， ， `AvailableIdle` `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` ， `Offline``PresenceUnknown`  |
|活动    |  字符串集合      |    用户可用性的补充信息。 可能的值是 `Available` ， ， ， ， ， ， ， `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` 。       |
|outOfOfficeSettings | [outOfOfficeSettings](outOfOfficeSettings.md) | 用户的外出设置。 |

>**注意：** 若要详细了解不同的状态，请参阅 [Teams 中的用户状态](/microsoftteams/presence-admins)。 

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.presence"
}-->
```json
{
   "id":"string",
   "availability":"string",
   "activity":"string",
   "outOfOfficeSettings":{"@odata.type": "#microsoft.graph.outOfOfficeSettings"}
}
```
