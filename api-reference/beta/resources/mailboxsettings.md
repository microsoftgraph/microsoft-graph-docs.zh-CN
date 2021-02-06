---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5da5e2294845fdf0aba2029acd410a59a7c0806c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135217"
---
# <a name="mailboxsettings-resource-type"></a>mailboxSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户的主邮箱 [的设置](user.md)。

可以通过 [查询](../api/user-get-mailboxsettings.md)[用户的](../api/user-update-mailboxsettings.md) **mailboxSettings** 属性获取或更新用户的邮箱设置。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|archiveFolder|string|用户存档文件夹的文件夹 ID。 只读。|
|automaticRepliesSetting|[automaticRepliesSetting](automaticrepliessetting.md)|自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。|
|dateFormat|string|用户邮箱的日期格式。|
|delegateMeetingMessageDeliveryOptions|delegateMeetingMessageDeliveryOptions| 如果用户具有日历代理，则指定代理、邮箱所有者还是同时接收会议邮件和会议响应。 可取值为：`sendToDelegateAndInformationToPrincipal`、`sendToDelegateAndPrincipal`、`sendToDelegateOnly`。 默认值为 `sendToDelegateOnly` 。|
|语言|[localeInfo](localeinfo.md)|用户的区域设置信息，包括首选语言和国家/地区。|
|timeFormat|string|用户邮箱的时间格式。|
|timeZone|string|用户邮箱的默认时区。|
|workingHours|[workingHours](workinghours.md)|特定时区用户一周的工作天数和小时数。|
|userPurpose|[userPurpose](userpurpose.md)|邮箱的用途。 用于区分单个用户的邮箱与 Exchange Online 中的共享邮箱和设备邮箱。 只读。|

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
  "delegateMeetingMessageDeliveryOptions": "String",
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeFormat": "string",
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"},
  "userPurpose": {"@odata.type": "microsoft.graph.userPurpose"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


