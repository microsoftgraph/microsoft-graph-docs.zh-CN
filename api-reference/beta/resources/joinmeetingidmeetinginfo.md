---
title: joinMeetingIdMeetingInfo 资源类型
description: 包含允许使用 joinMeetingId 和密码加入现有会议的信息。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a35dff2db37686bae85a52d47a4b1f1aa3a10ff0
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645615"
---
# <a name="joinmeetingidmeetinginfo-resource-type"></a>joinMeetingIdMeetingInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含的信息允许使用 **joinMeetingId** 和 **密码** (加入现有会议（如果需要）) 。 可以从 [Get onlineMeeting](../api/onlinemeeting-get.md) API 检索这些属性。

继承自 [meetingInfo](../resources/meetinginfo.md)。

## <a name="properties"></a>属性

| 属性                | 类型    | 说明                                                   |
| :---------------------- | :------ | :------------------------------------------------------------ |
| joinMeetingId           | String  | 用于加入会议的 ID。                              |
| 密码                | String  | 用于加入会议的密码。 可选。              |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.joinMeetingIdMeetingInfo"
}-->
```json
{
    "joinMeetingId": "String",
    "passcode": "String"
}
```
