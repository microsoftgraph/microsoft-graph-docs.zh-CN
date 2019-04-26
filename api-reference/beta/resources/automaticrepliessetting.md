---
title: automaticRepliesSetting 资源类型
description: '配置设置, 以自动将传入电子邮件的发件人通知发件人的邮件 '
localization_priority: Normal
ms.openlocfilehash: 6d7be13a47359e74b4d7a1dc44a4cca38924396e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328217"
---
# <a name="automaticrepliessetting-resource-type"></a>automaticRepliesSetting 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。例如，通知已登录用户无法回复电子邮件的自动答复。 


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|externalAudience|String| 如果 **Status** 是 **** 或 `AlwaysEnabled`，则表示将接收 `Scheduled` 的已登录用户组织外部的受众组。可能的值是：`none`、`contactsOnly`、`all`。|
|externalReplyMessage|string|如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示发送给指定外部受众的自动答复。|
|internalReplyMessage|string|如果 **Status** 为 `AlwaysEnabled` 或 `Scheduled`，则表示发送给已登录用户组织内部受众的自动答复。 |
|scheduledEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为结束。 |
|scheduledStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为开始。|
|status|String|自动答复的配置状态。可能的值是：`disabled`、`alwaysEnabled`、`scheduled`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
