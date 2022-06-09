---
title: automaticRepliesSetting 资源类型
description: '用于自动通知发件人传入电子邮件的配置设置，其中包含来自 '
ms.localizationpriority: medium
author: abheek-das
ms.prod: mail
doc_type: resourcePageType
ms.openlocfilehash: 6579843c9ecb5cea7db7350c89a72256dd935ede
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971153"
---
# <a name="automaticrepliessetting-resource-type"></a>automaticRepliesSetting 资源类型

命名空间：microsoft.graph

自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。例如，通知已登录用户无法回复电子邮件的自动答复。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|externalAudience|externalAudienceScope| 如果 **Status** 是  或 `AlwaysEnabled`，则表示将接收 `Scheduled` 的已登录用户组织外部的受众组。 可能的值包括 `none`、`contactsOnly`、`all`。|
|externalReplyMessage|string|如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示发送给指定外部受众的自动答复。|
|internalReplyMessage|string|如果 **Status** 为 `AlwaysEnabled` 或 `Scheduled`，则表示发送给已登录用户组织内部受众的自动答复。 |
|scheduledEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为结束。 |
|scheduledStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为开始。|
|status|automaticRepliesStatus|自动答复的配置状态。 可能的值包括 `disabled`、`alwaysEnabled`、`scheduled`。|

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
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

