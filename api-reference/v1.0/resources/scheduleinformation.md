---
title: scheduleInformation 资源类型
description: 表示用户、通讯组列表或资源在指定时间段的可用性。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 67b7396cfebc19baa3771c2ec8d153950928288506cfc699851b891e15409a0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231479"
---
# <a name="scheduleinformation-resource-type"></a>scheduleInformation 资源类型

命名空间：microsoft.graph

表示用户、通讯组列表或资源在 (或设备) 的可用性。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|availabilityView |String |表示 中所有项目的可用性的合并视图 `scheduleItems` 。 视图由时间段组成。 每个时间段的可用性指示为 `0` ：= 空闲 `1` 、= 暂定 `2` 、= 忙碌、= 外出 `3` `4` 、= 在其他地方工作。|
|error |[freeBusyError](freebusyerror.md) |尝试获取用户、通讯组列表或资源的可用性的错误信息。 |
|scheduleId |String |标识 **scheduleInformation** 实例的用户、通讯组列表或资源的 SMTP 地址。 |
|scheduleItems |[scheduleItem](scheduleitem.md) 集合 |包含描述用户或资源可用性的项目。 |
|workingHours |[workingHours](workinghours.md) |特定时区用户一周的工作天数和小时数。 这些设置为用户的 [mailboxSettings 的一部分](mailboxsettings.md)。|


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
  "tocPath": ""
}
-->

