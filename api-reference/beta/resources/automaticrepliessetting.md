---
title: automaticRepliesSetting 资源类型
description: '配置设置以自动通知中的邮件传入电子邮件的发件人 '
localization_priority: Normal
ms.openlocfilehash: 6755fda99f7a6186316b6198bfa975d73e14b09b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576771"
---
# <a name="automaticrepliessetting-resource-type"></a>automaticRepliesSetting 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。例如，通知已登录用户无法回复电子邮件的自动答复。 


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|externalAudience|externalAudienceScope| 一组的访问群体已登录的用户组织的外部用户将收到**ExternalReplyMessage**，如果**状态**为`AlwaysEnabled`或`Scheduled`。 可能的值为： `none`， `contactsOnly`， `all`。|
|externalReplyMessage|string|如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示发送给指定外部受众的自动答复。|
|internalReplyMessage|string|如果 **Status** 为 `AlwaysEnabled` 或 `Scheduled`，则表示发送给已登录用户组织内部受众的自动答复。 |
|scheduledEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为结束。 |
|scheduledStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为开始。|
|status|automaticRepliesStatus|配置自动答复状态。 可能的值为： `disabled`， `alwaysEnabled`， `scheduled`。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/automaticrepliessetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
