---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 99097c026ef219e82a34a6c7b043cf70d36c965d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447505"
---
# <a name="mailboxsettings-resource-type"></a>mailboxSettings 资源类型

命名空间： microsoft. graph

[用户](user.md)的主邮箱的设置。

您可以通过查询用户的**mailboxSettings**属性来[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)用户的邮箱设置。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|archiveFolder|string|用户存档文件夹的文件夹 ID。|
|automaticRepliesSetting|[automaticRepliesSetting](automaticrepliessetting.md)|自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。|
|dateFormat|string|用户邮箱的日期格式。|
|语言|[localeInfo](localeinfo.md)|用户的区域设置信息，包括首选语言和国家/地区。|
|timeFormat|string|用户邮箱的时间格式。|
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
  "dateFormat": "string",
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeFormat": "string",
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
