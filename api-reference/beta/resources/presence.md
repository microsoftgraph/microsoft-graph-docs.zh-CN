---
title: 状态资源类型
description: 包含有关用户状态的信息，包括用户的可用性和用户活动。
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 797ddac8bc582cd5e5d4d51e0e1ad94645c3c1e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521570"
---
# <a name="presence-resource-type"></a>状态资源类型

命名空间： microsoft. graph

包含有关用户状态的信息，包括用户的可用性和用户活动。

> **注意：** 此资源目前仅对 Microsoft 团队用户受支持。

## <a name="methods"></a>方法

| 方法                                                            | 返回类型                                       | 说明                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [获取状态](../api/presence-get.md)     | [状态](../resources/presence.md)     | 获取用户的状态信息。
| [获取多个用户的状态](../api/cloudcommunications-getpresencesbyuserid.md)    |  [状态](../resources/presence.md)集合     |  获取多个用户的状态信息。      |


## <a name="properties"></a>属性

| 关系        | 类型                                                 | 说明                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|id    |  string     |  User 对象 id   |
|availability    |  string 集合   |   用户的基本状态信息。 可能的值`Available`为`AvailableIdle`、 `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb`、、、、 `Offline`、、`PresenceUnknown`  |
|activity    |  string 集合      |    将补充信息提供给用户的可用性。 可能的值`Available`为`Away`、 `BeRightBack``Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `UrgentInterruptionsOnly`、、`InAMeeting`、、、、、、、、、、、。 `Offline` `OffWork``OutOfOffice` `PresenceUnknown``Presenting`       |

>**注意：** 若要了解有关不同状态的详细信息，请参阅[团队中的用户状态](https://docs.microsoft.com/microsoftteams/presence-admins)。 

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
   "activity":"string"
}
```
