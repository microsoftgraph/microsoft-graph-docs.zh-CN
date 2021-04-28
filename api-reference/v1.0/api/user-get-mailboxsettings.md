---
title: 获取用户的邮箱设置
description: '获取用户的 mailboxSettings。 这包括自动答复设置（自动通知用户 '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e2f697a332eb4912f0f4f442f57ccf79b86d03ca
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054306"
---
# <a name="get-user-mailbox-settings"></a>获取用户的邮箱设置

命名空间：microsoft.graph

获取用户的 [mailboxSettings](../resources/mailboxsettings.md)。 可以查看所有邮箱设置或获取特定设置。

用户可通过 Outlook 客户端为其邮箱设置以下设置：

- [自动答复](../resources/automaticrepliessetting.md)（收到发件人的电子邮件时自动通知发件人）
- 日期格式
- delegateMeetingMessageDeliveryOptions
- [区域设置](../resources/localeinfo.md)（语言和国家/地区）
- 时间格式
- 时区
- [工作时间](../resources/workinghours.md)

用户可以使用 Outlook 网页版设置首选的日期和时间格式。 用户可以选择支持的[短日期](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate)或[短时间](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime)格式之一。 此 `GET` 操作将返回用户选择的格式。

通过从管理员为其邮箱服务器设置的[支持时区](outlookuser-supportedtimezones.md)中进行选择，用户可以在任何 Outlook 客户端上设置自己喜欢的时区。 管理员能够以 Windows 时区格式或者以 [Internet 号码分配局 (IANA) 时区](https://www.iana.org/time-zones)（也称为“Olson 时区”）格式设置时区。 Windows 时区是默认格式。

此 `GET` 操作以管理员设置的格式返回用户的首选时区。 若要将时区设置为某种特定格式（Windows 或 IANA），可以先[将相应格式的首选时区更新为邮箱设置](user-update-mailboxsettings.md)。 随后便可以获取相应格式的时区。 也可以在应用中单独管理格式转换。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | MailboxSettings.Read、MailboxSettings.ReadWrite    |
|委派（个人 Microsoft 帐户） | MailboxSettings.Read、MailboxSettings.ReadWrite    |
|应用程序 | MailboxSettings.Read、MailboxSettings.ReadWrite |

## <a name="http-request"></a>HTTP 请求
若要获取用户的所有邮箱设置：
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

若要获取特定设置 - 仅限自动答复设置、日期格式、区域设置、时间格式、时区或工作时间：
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/dateFormat
GET /users/{id|userPrincipalName}/mailboxSettings/dateFormat

GET /me/mailboxSettings/delegateMeetingMessageDeliveryOptions
GET /users/{id|userPrincipalName}/mailboxSettings/delegateMeetingMessageDeliveryOptions

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeFormat
GET /users/{id|userPrincipalName}/mailboxSettings/timeFormat

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。
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
- 字符串（适用于 **dateFormat**）
- **delegateMeetingMessageDeliveryOptions** (的字符串) 
- [localeInfo](../resources/localeinfo.md) 对象
- 字符串（适用于 **timeFormat**）
- 字符串（适用于 **timeZone**）
- [workingHours](../resources/workinghours.md)

## <a name="examples"></a>示例

### <a name="example-1"></a>示例 1
#### <a name="request"></a>请求
第一个示例获取已登录用户邮箱的所有邮箱设置，其中包括自动答复、日期格式、区域设置（语言和国家/地区）、时间格式、时区和工作时间设置。

<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```

#### <a name="response"></a>响应
该响应包括已登录用户的所有邮箱设置。
注意：为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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
        "startTime": "08:00:00.0000000",
        "endTime": "17:00:00.0000000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    },
    "dateFormat": "MM/dd/yyyy",
    "timeFormat": "hh:mm tt",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateOnly"
}
```

### <a name="example-2"></a>示例 2
#### <a name="request"></a>请求
第二个示例专门获取已登录用户邮箱的自动答复设置。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
该响应仅包括自动答复设置。
注意：为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
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

### <a name="example-3"></a>示例 3
#### <a name="request"></a>请求
第三个示例专门获取已登录用户邮箱的工作时间设置。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/workingHours
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
该响应仅包括工作时间设置。 请注意，用户的工作时间在[自定义时区](../resources/customtimezone.md)内。
注意：为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "name": "get_mailboxsettings_3",
  "truncated": true,
  "@odata.type": "microsoft.graph.workingHours"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
