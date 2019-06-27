---
title: 获取用户的邮箱设置
description: '获取用户的 mailboxSettings。 这包括自动答复设置（自动通知用户 '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7643c40daa2a53b4c22ff2f17c7b8026dc93f365
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270341"
---
# <a name="get-user-mailbox-settings"></a>获取用户的邮箱设置

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取用户的 [mailboxSettings](../resources/mailboxsettings.md)。 这包括自动答复的设置 (在收到电子邮件时自动通知人员)、区域设置 (语言和国家/地区)、时区和工作时间。

可以查看所有邮箱设置或获取特定设置。

时区是用户可以为用户邮箱设置的首选设置之一。 用户从管理员为用户的邮箱服务器设置的[受支持时区](outlookuser-supportedtimezones.md)中选择该区域。 管理员在 Windows 时区格式或[Internet 分配的号码颁发机构 (IANA)](https://www.iana.org/time-zones)时区 (也称为 "Olson 时区") 格式中设置时区。 Windows 时区是默认格式。 

获取用户的首选时区时，时区按创建时的格式返回。 若要将时区设置为某种特定格式（Windows 或 IANA），可以先[将相应格式的首选时区更新为邮箱设置](user-update-mailboxsettings.md)。 随后便可以获取相应格式的时区。 也可以在应用中单独管理格式转换。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | MailboxSettings.Read、MailboxSettings.ReadWrite    |
|委派（个人 Microsoft 帐户） | MailboxSettings.Read、MailboxSettings.ReadWrite    |
|应用程序 | MailboxSettings.Read、MailboxSettings.ReadWrite |

## <a name="http-request"></a>HTTP 请求
若要获取用户的所有邮箱设置, 请执行以下操作:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

若要获取特定设置-仅限自动答复设置、区域设置、时区或工作时间:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和以下请求对象之一：

- [mailboxSettings](../resources/mailboxsettings.md) 对象
- [automaticRepliesSetting](../resources/automaticrepliessetting.md) 对象
- [localeInfo](../resources/localeinfo.md) 对象
- 字符串（适用于 **timeZone**）
- [workingHours](../resources/workinghours.md)

## <a name="example"></a>示例
##### <a name="request-1"></a>请求 1
第一个示例获取已登录用户邮箱的所有邮箱设置，其中包括时区、自动答复、区域设置（语言和国家/地区）和工作时间设置。
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
##### <a name="response-1"></a>响应 1
响应包括已登录用户的所有邮箱设置。 注意：为简洁起见，可能会截断此处显示的响应对象。 将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "externalAudience": "All",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-14T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
        "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime":"08:00:00.0000000",
        "endTime":"17:00:00.0000000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    }
}
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailboxsettings_1-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailboxsettings_1-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_mailboxsettings_1-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a>请求 2
第二个示例专门获取已登录用户邮箱的自动答复设置。
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a>响应 2
该响应仅包括自动答复设置。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings/automaticRepliesSetting",
    "status": "alwaysEnabled",
    "externalAudience": "None",
    "scheduledStartDateTime": {
        "dateTime": "2016-03-19T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "scheduledEndDateTime": {
        "dateTime": "2016-03-20T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
}
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailboxsettings_2-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailboxsettings_2-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_mailboxsettings_2-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-3"></a>请求 3
第三个示例专门获取已登录用户邮箱的工作时间设置。
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a>响应 3
该响应仅包括工作时间设置。 请注意，用户的工作时间在[自定义时区](../resources/customtimezone.md)内。 注意：为简洁起见，可能会截断此处显示的响应对象。 将从实际调用中返回所有属性。
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3",
  "truncated": true,
  "@odata.type": "microsoft.graph.workingHours"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
    "daysOfWeek":[
        "monday",
        "tuesday",
        "wednesday",
        "thursday",
        "friday",
        "saturday"
    ],
    "startTime":"09:00:00.0000000",
    "endTime":"18:30:00.0000000",
    "timeZone":{
        "@odata.type":"#microsoft.graph.customTimeZone",
        "bias":-200,
        "name":"Customized Time Zone",
        "standardOffset":{
            "time":"02:00:00.0000000",
            "dayOccurrence":4,
            "dayOfWeek":"sunday",
            "month":5,
            "year":0
        },
        "daylightOffset":{
            "daylightBias":-100,
            "time":"02:00:00.0000000",
            "dayOccurrence":2,
            "dayOfWeek":"sunday",
            "month":10,
            "year":0
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-get-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-get-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-get-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-get-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-get-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
