---
title: scheduleInformation 资源类型
description: '表示用户、通讯组列表或资源在指定时间段内的可用性。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: harini84
ms.openlocfilehash: 6a7122ac4842ce4d2809837498874c7aabd9d942
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811376"
---
# <a name="scheduleinformation-resource-type"></a>scheduleInformation 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在指定时间段内，用户、通讯组列表或资源 (会议室或设备) 的可用性。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|availabilityView |String |表示中所有项的可用性的合并视图 `scheduleItems` 。 视图由时间段组成。 在每个时间段内的可用性表示为： `0` = free、 `1` = 暂定、 `2` = 忙碌、 `3` = 外出， `4` = 在其他地方工作。|
|error |[freeBusyError](freebusyerror.md) |有关尝试获取用户、通讯组列表或资源的可用性的错误信息。 |
|scheduleId |String |标识 **scheduleInformation**实例的用户、通讯组列表或资源的 SMTP 地址。 |
|scheduleItems |[scheduleItem](scheduleitem.md) 集合 |包含描述用户或资源可用性的项。 |
|workingHours |[workingHours](workinghours.md) |特定时区用户一周的工作天数和小时数。 这些设置为用户的 [mailboxSettings](mailboxsettings.md)的一部分。|


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
