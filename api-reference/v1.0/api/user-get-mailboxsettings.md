---
title: 获取用户的邮箱设置
description: '获取用户的 mailboxSettings。 这包括自动答复设置（自动通知用户 '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 687b25294d257beb8ae25bd94bd0ffd9c3a6ca70
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886243"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="22598-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="22598-104">Get user mailbox settings</span></span>

<span data-ttu-id="22598-p102">获取用户的 [mailboxSettings](../resources/mailboxsettings.md)。这包括自动答复（收到发件人的电子邮件时自动通知发件人）、区域设置（语言和国家/地区）、时区和工作时间的设置。</span><span class="sxs-lookup"><span data-stu-id="22598-p102">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone, and working hours.</span></span>

<span data-ttu-id="22598-107">可以查看所有邮箱设置或获取特定设置。</span><span class="sxs-lookup"><span data-stu-id="22598-107">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="22598-108">时区是用户可以为用户邮箱设置的首选设置之一。</span><span class="sxs-lookup"><span data-stu-id="22598-108">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="22598-109">有效的时区格式包括 Windows 时区格式和 [Internet 号码分配局 (IANA) 时区](https://www.iana.org/time-zones)（亦称为“Olson 时区”）格式。</span><span class="sxs-lookup"><span data-stu-id="22598-109">Valid time zone formats include the Windows time zone format and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="22598-110">Windows 时区是默认格式。</span><span class="sxs-lookup"><span data-stu-id="22598-110">The Windows format is the default.</span></span> 

<span data-ttu-id="22598-111">获取用户的首选时区时，时区按创建时的格式返回。</span><span class="sxs-lookup"><span data-stu-id="22598-111">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="22598-112">若要将时区设置为某种特定格式（Windows 或 IANA），可以先[将相应格式的首选时区更新为邮箱设置](user-update-mailboxsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="22598-112">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="22598-113">随后便可以获取相应格式的时区。</span><span class="sxs-lookup"><span data-stu-id="22598-113">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="22598-114">也可以在应用中单独管理格式转换。</span><span class="sxs-lookup"><span data-stu-id="22598-114">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="22598-115">权限</span><span class="sxs-lookup"><span data-stu-id="22598-115">Permissions</span></span>
<span data-ttu-id="22598-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22598-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22598-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="22598-118">Permission type</span></span>      | <span data-ttu-id="22598-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22598-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22598-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22598-120">Delegated (work or school account)</span></span> | <span data-ttu-id="22598-121">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22598-121">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="22598-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22598-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22598-123">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22598-123">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="22598-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="22598-124">Application</span></span> | <span data-ttu-id="22598-125">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22598-125">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="22598-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22598-126">HTTP request</span></span>
<span data-ttu-id="22598-127">获取用户的所有邮箱设置：</span><span class="sxs-lookup"><span data-stu-id="22598-127">To get all mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="22598-128">获取特定设置，例如，仅获取自动答复设置、区域设置、时区或工作时间设置：</span><span class="sxs-lookup"><span data-stu-id="22598-128">To get specific settings - for example, only the automatic replies settings, locale, time zone, or working hours:</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="22598-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="22598-129">Optional query parameters</span></span>
<span data-ttu-id="22598-130">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="22598-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="22598-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="22598-131">Request headers</span></span>
| <span data-ttu-id="22598-132">名称</span><span class="sxs-lookup"><span data-stu-id="22598-132">Name</span></span>       | <span data-ttu-id="22598-133">类型</span><span class="sxs-lookup"><span data-stu-id="22598-133">Type</span></span> | <span data-ttu-id="22598-134">说明</span><span class="sxs-lookup"><span data-stu-id="22598-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="22598-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="22598-135">Authorization</span></span>  | <span data-ttu-id="22598-136">string</span><span class="sxs-lookup"><span data-stu-id="22598-136">string</span></span>  | <span data-ttu-id="22598-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22598-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22598-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="22598-139">Request body</span></span>
<span data-ttu-id="22598-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22598-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22598-141">响应</span><span class="sxs-lookup"><span data-stu-id="22598-141">Response</span></span>

<span data-ttu-id="22598-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和以下请求对象之一：</span><span class="sxs-lookup"><span data-stu-id="22598-142">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="22598-143">[mailboxSettings](../resources/mailboxsettings.md) 对象</span><span class="sxs-lookup"><span data-stu-id="22598-143">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="22598-144">[automaticRepliesSetting](../resources/automaticrepliessetting.md) 对象</span><span class="sxs-lookup"><span data-stu-id="22598-144">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="22598-145">[localeInfo](../resources/localeinfo.md) 对象</span><span class="sxs-lookup"><span data-stu-id="22598-145">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="22598-146">字符串（适用于 **timeZone**）</span><span class="sxs-lookup"><span data-stu-id="22598-146">string (for **timeZone**)</span></span>
- [<span data-ttu-id="22598-147">workingHours</span><span class="sxs-lookup"><span data-stu-id="22598-147">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="22598-148">示例</span><span class="sxs-lookup"><span data-stu-id="22598-148">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="22598-149">请求 1</span><span class="sxs-lookup"><span data-stu-id="22598-149">Request 1</span></span>
<span data-ttu-id="22598-150">第一个示例获取已登录用户邮箱的所有邮箱设置，其中包括时区、自动答复、区域设置（语言和国家/地区）和工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="22598-150">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="22598-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="22598-151">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22598-152">C#</span><span class="sxs-lookup"><span data-stu-id="22598-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22598-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="22598-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22598-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22598-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="22598-155">Java</span><span class="sxs-lookup"><span data-stu-id="22598-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="22598-156">响应 1</span><span class="sxs-lookup"><span data-stu-id="22598-156">Response 1</span></span>
<span data-ttu-id="22598-p107">该响应包括所有的邮箱设置。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22598-p107">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="22598-160">请求 2</span><span class="sxs-lookup"><span data-stu-id="22598-160">Request 2</span></span>
<span data-ttu-id="22598-161">第二个示例专门获取已登录用户邮箱的自动答复设置。</span><span class="sxs-lookup"><span data-stu-id="22598-161">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="22598-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="22598-162">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22598-163">C#</span><span class="sxs-lookup"><span data-stu-id="22598-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22598-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="22598-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22598-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22598-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="22598-166">Java</span><span class="sxs-lookup"><span data-stu-id="22598-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="22598-167">响应 2</span><span class="sxs-lookup"><span data-stu-id="22598-167">Response 2</span></span>
<span data-ttu-id="22598-p108">该响应仅包括自动答复设置。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22598-p108">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-3"></a><span data-ttu-id="22598-171">请求 3</span><span class="sxs-lookup"><span data-stu-id="22598-171">Request 3</span></span>
<span data-ttu-id="22598-172">第三个示例专门获取已登录用户邮箱的工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="22598-172">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="22598-173">响应 3</span><span class="sxs-lookup"><span data-stu-id="22598-173">Response 3</span></span>
<span data-ttu-id="22598-174">该响应仅包括工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="22598-174">The response includes only the working hours settings.</span></span> <span data-ttu-id="22598-175">请注意，用户的工作时间在[自定义时区](../resources/customtimezone.md)内。</span><span class="sxs-lookup"><span data-stu-id="22598-175">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="22598-176">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="22598-176">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="22598-177">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22598-177">All of the properties will be returned from an actual call.</span></span>
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
