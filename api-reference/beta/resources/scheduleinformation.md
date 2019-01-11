---
title: scheduleInformation 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: e535f5c2b47e810fc767cb29d0b24f28ed3c7bf0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828705"
---
# <a name="scheduleinformation-resource-type"></a>scheduleInformation 资源类型

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。
 
在指定的时间段代表用户、 通讯组列表或资源的可用性。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|availabilityView |字符串 |表示的合并的视图中的所有项目的可用性的`scheduleItems`。 视图包含的时间段。 指示期间每个时间段的可用性：`0`免费 = `1`= 暂定、 `2`= 忙`3`= 外出、 `4`= 其他地方工作。|
|error |[freeBusyError](freebusyerror.md) |从尝试获取用户、 通讯组列表或资源的可用性信息的错误。 |
|scheduleId |字符串 |用户、 通讯组列表或资源，标识实例**scheduleInformation**SMTP 地址。 |
|scheduleItems |[scheduleItem](scheduleitem.md)集合 |包含描述的用户或资源的可用性的项。 |
|workingHours |[workingHours](workinghours.md) |特定时区用户一周的工作天数和小时数。 这些设置用户的[mailboxSettings](mailboxsettings.md)的一部分。|


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
<!-- {
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
