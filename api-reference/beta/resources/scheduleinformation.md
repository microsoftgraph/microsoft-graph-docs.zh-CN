---
title: scheduleInformation 资源类型
description: '表示用户、通讯组列表或资源在指定时间段内的可用性。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: 3d6ede4e1085a8be3f78b714f690b79b836abbcb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965304"
---
# <a name="scheduleinformation-resource-type"></a>scheduleInformation 资源类型

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示用户、通讯组列表或资源 (会议室或设备) 在指定时间段的可用性。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|availabilityView |String |表示中`scheduleItems`所有项的可用性的合并视图。 视图由时间段组成。 在每个时间段内的可用性表示`0`为: = `1`free、= `2`暂定、= `3`忙碌、= 外出, `4`= 在其他地方工作。|
|error |[freeBusyError](freebusyerror.md) |有关尝试获取用户、通讯组列表或资源的可用性的错误信息。 |
|scheduleId |String |标识**scheduleInformation**实例的用户、通讯组列表或资源的 SMTP 地址。 |
|scheduleItems |[scheduleItem](scheduleitem.md)集合 |包含描述用户或资源可用性的项。 |
|workingHours |[workingHours](workinghours.md) |特定时区用户一周的工作天数和小时数。 这些设置为用户的[mailboxSettings](mailboxsettings.md)的一部分。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
