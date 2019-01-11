---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
ms.openlocfilehash: d4df71930a26c711c59f164aca5090bda809b503
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826997"
---
# <a name="mailboxsettings-resource-type"></a>mailboxSettings 资源类型

已登录用户的主邮箱的设置。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|archiveFolder|string|用户存档文件夹的文件夹 ID。|
|automaticRepliesSetting|[automaticRepliesSetting](automaticrepliessetting.md)|自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。|
|语言|[localeInfo](localeinfo.md)|用户的区域设置信息，包括首选语言和国家/地区。|
|timeZone|string|用户邮箱的默认时区。|
|workingHours|[workingHours](workinghours.md)|特定时区用户一周的工作天数和小时数。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
