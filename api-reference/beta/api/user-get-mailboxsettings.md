---
title: 获取用户的邮箱设置
description: '获取用户的 mailboxSettings。 这包括自动答复设置（自动通知用户 '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4d4cb61bb69b918fe9706adbbe2c2780df1ddcf3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421118"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="82cbc-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="82cbc-104">Get user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82cbc-105">获取用户的 [mailboxSettings](../resources/mailboxsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="82cbc-105">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="82cbc-106">这包括自动答复的设置 (在收到电子邮件时自动通知人员)、区域设置 (语言和国家/地区)、时区和工作时间。</span><span class="sxs-lookup"><span data-stu-id="82cbc-106">This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), time zone, and working hours.</span></span>

<span data-ttu-id="82cbc-107">可以查看所有邮箱设置或获取特定设置。</span><span class="sxs-lookup"><span data-stu-id="82cbc-107">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="82cbc-108">时区是用户可以为用户邮箱设置的首选设置之一。</span><span class="sxs-lookup"><span data-stu-id="82cbc-108">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="82cbc-109">用户从管理员为用户的邮箱服务器设置的[受支持时区](outlookuser-supportedtimezones.md)中选择该区域。</span><span class="sxs-lookup"><span data-stu-id="82cbc-109">The user chooses it from the [supported time zones](outlookuser-supportedtimezones.md) that an administrator has set up for the user's mailbox server.</span></span> <span data-ttu-id="82cbc-110">管理员在 Windows 时区格式或[Internet 分配的号码颁发机构 (IANA)](https://www.iana.org/time-zones)时区 (也称为 "Olson 时区") 格式中设置时区。</span><span class="sxs-lookup"><span data-stu-id="82cbc-110">The administrator sets up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="82cbc-111">Windows 时区是默认格式。</span><span class="sxs-lookup"><span data-stu-id="82cbc-111">The Windows format is the default.</span></span> 

<span data-ttu-id="82cbc-112">获取用户的首选时区时，时区按创建时的格式返回。</span><span class="sxs-lookup"><span data-stu-id="82cbc-112">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="82cbc-113">若要将时区设置为某种特定格式（Windows 或 IANA），可以先[将相应格式的首选时区更新为邮箱设置](user-update-mailboxsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="82cbc-113">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="82cbc-114">随后便可以获取相应格式的时区。</span><span class="sxs-lookup"><span data-stu-id="82cbc-114">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="82cbc-115">也可以在应用中单独管理格式转换。</span><span class="sxs-lookup"><span data-stu-id="82cbc-115">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="82cbc-116">权限</span><span class="sxs-lookup"><span data-stu-id="82cbc-116">Permissions</span></span>
<span data-ttu-id="82cbc-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82cbc-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82cbc-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="82cbc-119">Permission type</span></span>      | <span data-ttu-id="82cbc-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82cbc-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82cbc-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82cbc-121">Delegated (work or school account)</span></span> | <span data-ttu-id="82cbc-122">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82cbc-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="82cbc-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82cbc-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82cbc-124">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82cbc-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="82cbc-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="82cbc-125">Application</span></span> | <span data-ttu-id="82cbc-126">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82cbc-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="82cbc-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82cbc-127">HTTP request</span></span>
<span data-ttu-id="82cbc-128">若要获取用户的所有邮箱设置, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="82cbc-128">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="82cbc-129">若要获取特定设置-仅限自动答复设置、区域设置、时区或工作时间:</span><span class="sxs-lookup"><span data-stu-id="82cbc-129">To get specific settings - only the automatic replies settings, locale, time zone, or working hours:</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="82cbc-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="82cbc-130">Optional query parameters</span></span>
<span data-ttu-id="82cbc-131">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="82cbc-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="82cbc-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="82cbc-132">Request headers</span></span>
| <span data-ttu-id="82cbc-133">名称</span><span class="sxs-lookup"><span data-stu-id="82cbc-133">Name</span></span>       | <span data-ttu-id="82cbc-134">类型</span><span class="sxs-lookup"><span data-stu-id="82cbc-134">Type</span></span> | <span data-ttu-id="82cbc-135">说明</span><span class="sxs-lookup"><span data-stu-id="82cbc-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="82cbc-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="82cbc-136">Authorization</span></span>  | <span data-ttu-id="82cbc-137">string</span><span class="sxs-lookup"><span data-stu-id="82cbc-137">string</span></span>  | <span data-ttu-id="82cbc-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82cbc-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82cbc-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="82cbc-140">Request body</span></span>
<span data-ttu-id="82cbc-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82cbc-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82cbc-142">响应</span><span class="sxs-lookup"><span data-stu-id="82cbc-142">Response</span></span>

<span data-ttu-id="82cbc-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和以下请求对象之一：</span><span class="sxs-lookup"><span data-stu-id="82cbc-143">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="82cbc-144">[mailboxSettings](../resources/mailboxsettings.md) 对象</span><span class="sxs-lookup"><span data-stu-id="82cbc-144">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="82cbc-145">[automaticRepliesSetting](../resources/automaticrepliessetting.md) 对象</span><span class="sxs-lookup"><span data-stu-id="82cbc-145">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="82cbc-146">[localeInfo](../resources/localeinfo.md) 对象</span><span class="sxs-lookup"><span data-stu-id="82cbc-146">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="82cbc-147">字符串（适用于 **timeZone**）</span><span class="sxs-lookup"><span data-stu-id="82cbc-147">string (for **timeZone**)</span></span>
- [<span data-ttu-id="82cbc-148">workingHours</span><span class="sxs-lookup"><span data-stu-id="82cbc-148">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="82cbc-149">示例</span><span class="sxs-lookup"><span data-stu-id="82cbc-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="82cbc-150">请求 1</span><span class="sxs-lookup"><span data-stu-id="82cbc-150">Request 1</span></span>
<span data-ttu-id="82cbc-151">第一个示例获取已登录用户邮箱的所有邮箱设置，其中包括时区、自动答复、区域设置（语言和国家/地区）和工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="82cbc-151">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="82cbc-152">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="82cbc-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82cbc-153">C#</span><span class="sxs-lookup"><span data-stu-id="82cbc-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82cbc-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82cbc-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82cbc-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="82cbc-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="82cbc-156">响应 1</span><span class="sxs-lookup"><span data-stu-id="82cbc-156">Response 1</span></span>
<span data-ttu-id="82cbc-157">响应包括已登录用户的所有邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="82cbc-157">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="82cbc-158">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="82cbc-158">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="82cbc-159">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82cbc-159">All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="82cbc-160">请求 2</span><span class="sxs-lookup"><span data-stu-id="82cbc-160">Request 2</span></span>
<span data-ttu-id="82cbc-161">第二个示例专门获取已登录用户邮箱的自动答复设置。</span><span class="sxs-lookup"><span data-stu-id="82cbc-161">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="82cbc-162">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="82cbc-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82cbc-163">C#</span><span class="sxs-lookup"><span data-stu-id="82cbc-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82cbc-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82cbc-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82cbc-165">目标-C</span><span class="sxs-lookup"><span data-stu-id="82cbc-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="82cbc-166">响应 2</span><span class="sxs-lookup"><span data-stu-id="82cbc-166">Response 2</span></span>
<span data-ttu-id="82cbc-p108">该响应仅包括自动答复设置。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82cbc-p108">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-3"></a><span data-ttu-id="82cbc-170">请求 3</span><span class="sxs-lookup"><span data-stu-id="82cbc-170">Request 3</span></span>
<span data-ttu-id="82cbc-171">第三个示例专门获取已登录用户邮箱的工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="82cbc-171">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="82cbc-172">响应 3</span><span class="sxs-lookup"><span data-stu-id="82cbc-172">Response 3</span></span>
<span data-ttu-id="82cbc-173">该响应仅包括工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="82cbc-173">The response includes only the working hours settings.</span></span> <span data-ttu-id="82cbc-174">请注意，用户的工作时间在[自定义时区](../resources/customtimezone.md)内。</span><span class="sxs-lookup"><span data-stu-id="82cbc-174">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="82cbc-175">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="82cbc-175">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="82cbc-176">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82cbc-176">All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
