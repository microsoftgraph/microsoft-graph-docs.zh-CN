---
title: 获取用户的邮箱设置
description: '获取用户的 mailboxSettings。 这包括自动答复设置（自动通知用户 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2989be09e15ecc7ab6a0bf976ac9c6069b55023e
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402492"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="22cc6-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="22cc6-104">Get user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22cc6-105">获取用户的 [mailboxSettings](../resources/mailboxsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="22cc6-105">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="22cc6-106">您可以查看所有邮箱设置或获取特定设置。</span><span class="sxs-lookup"><span data-stu-id="22cc6-106">You can view all mailbox settings, or get specific settings.</span></span>

<span data-ttu-id="22cc6-107">用户可以通过 Outlook 客户端为其邮箱设置以下设置：</span><span class="sxs-lookup"><span data-stu-id="22cc6-107">Users can set the following settings for their mailboxes through an Outlook client:</span></span>

- <span data-ttu-id="22cc6-108">[自动答复](../resources/automaticrepliessetting.md)（收到电子邮件后自动通知人员）</span><span class="sxs-lookup"><span data-stu-id="22cc6-108">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="22cc6-109">日期格式</span><span class="sxs-lookup"><span data-stu-id="22cc6-109">date format</span></span>
- <span data-ttu-id="22cc6-110">[区域设置](../resources/localeinfo.md)（语言和国家/地区）</span><span class="sxs-lookup"><span data-stu-id="22cc6-110">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="22cc6-111">时间格式</span><span class="sxs-lookup"><span data-stu-id="22cc6-111">time format</span></span>
- <span data-ttu-id="22cc6-112">时区</span><span class="sxs-lookup"><span data-stu-id="22cc6-112">time zone</span></span>
- [<span data-ttu-id="22cc6-113">working hours － 工作时间</span><span class="sxs-lookup"><span data-stu-id="22cc6-113">working hours</span></span>](../resources/workinghours.md)

<span data-ttu-id="22cc6-114">用户可以使用 Outlook 网页设置其首选的日期和时间格式。</span><span class="sxs-lookup"><span data-stu-id="22cc6-114">Users can set their preferred date and time formats using Outlook on the web.</span></span> <span data-ttu-id="22cc6-115">用户可以选择一种受支持的[短日期](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate)或[短时间](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime)格式。</span><span class="sxs-lookup"><span data-stu-id="22cc6-115">Users can choose one of the supported [short date](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) formats.</span></span> <span data-ttu-id="22cc6-116">此`GET`操作将返回用户选择的格式。</span><span class="sxs-lookup"><span data-stu-id="22cc6-116">This `GET` operation returns the format the user has chosen.</span></span>

<span data-ttu-id="22cc6-117">用户可以在任何 Outlook 客户端上设置喜欢的时区，方法是从其管理员为其邮箱服务器设置的[受支持时区](outlookuser-supportedtimezones.md)中进行选择。</span><span class="sxs-lookup"><span data-stu-id="22cc6-117">Users can set the time zone they prefer on any Outlook client, by choosing from the [supported time zones](outlookuser-supportedtimezones.md) that their administrator has set up for their mailbox server.</span></span> <span data-ttu-id="22cc6-118">管理员可以在 Windows 时区格式或[Internet 分配的号码颁发机构（IANA）](https://www.iana.org/time-zones)时区（也称为 "Olson 时区"）格式中设置时区。</span><span class="sxs-lookup"><span data-stu-id="22cc6-118">The administrator can set up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="22cc6-119">Windows 时区是默认格式。</span><span class="sxs-lookup"><span data-stu-id="22cc6-119">The Windows format is the default.</span></span> 

<span data-ttu-id="22cc6-120">此`GET`操作将以管理员设置的格式返回用户的首选时区。</span><span class="sxs-lookup"><span data-stu-id="22cc6-120">This `GET` operation returns the user's preferred time zone in the format that the administrator has set up.</span></span> <span data-ttu-id="22cc6-121">若要将时区设置为某种特定格式（Windows 或 IANA），可以先[将相应格式的首选时区更新为邮箱设置](user-update-mailboxsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="22cc6-121">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="22cc6-122">随后便可以获取相应格式的时区。</span><span class="sxs-lookup"><span data-stu-id="22cc6-122">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="22cc6-123">也可以在应用中单独管理格式转换。</span><span class="sxs-lookup"><span data-stu-id="22cc6-123">Alternatively, you can manage the format conversion separately in your app.</span></span> 

## <a name="permissions"></a><span data-ttu-id="22cc6-124">权限</span><span class="sxs-lookup"><span data-stu-id="22cc6-124">Permissions</span></span>
<span data-ttu-id="22cc6-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22cc6-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22cc6-127">权限类型</span><span class="sxs-lookup"><span data-stu-id="22cc6-127">Permission type</span></span>      | <span data-ttu-id="22cc6-128">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22cc6-128">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22cc6-129">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22cc6-129">Delegated (work or school account)</span></span> | <span data-ttu-id="22cc6-130">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22cc6-130">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="22cc6-131">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22cc6-131">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22cc6-132">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22cc6-132">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="22cc6-133">应用程序</span><span class="sxs-lookup"><span data-stu-id="22cc6-133">Application</span></span> | <span data-ttu-id="22cc6-134">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22cc6-134">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="22cc6-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22cc6-135">HTTP request</span></span>
<span data-ttu-id="22cc6-136">若要获取用户的所有邮箱设置，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="22cc6-136">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="22cc6-137">若要获取特定设置-仅限自动答复设置、日期格式、区域设置、时间格式、时区或工作时间：</span><span class="sxs-lookup"><span data-stu-id="22cc6-137">To get specific settings - only the automatic replies settings, date format, locale, time format, time zone, or working hours:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/dateFormat
GET /users/{id|userPrincipalName}/mailboxSettings/dateFormat

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeFormat
GET /users/{id|userPrincipalName}/mailboxSettings/timeFormat

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="22cc6-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="22cc6-138">Optional query parameters</span></span>
<span data-ttu-id="22cc6-139">此方法支持一些[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="22cc6-139">This method supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="22cc6-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="22cc6-140">Request headers</span></span>
| <span data-ttu-id="22cc6-141">名称</span><span class="sxs-lookup"><span data-stu-id="22cc6-141">Name</span></span>       | <span data-ttu-id="22cc6-142">类型</span><span class="sxs-lookup"><span data-stu-id="22cc6-142">Type</span></span> | <span data-ttu-id="22cc6-143">说明</span><span class="sxs-lookup"><span data-stu-id="22cc6-143">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="22cc6-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="22cc6-144">Authorization</span></span>  | <span data-ttu-id="22cc6-145">string</span><span class="sxs-lookup"><span data-stu-id="22cc6-145">string</span></span>  | <span data-ttu-id="22cc6-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22cc6-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22cc6-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="22cc6-148">Request body</span></span>
<span data-ttu-id="22cc6-149">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22cc6-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22cc6-150">响应</span><span class="sxs-lookup"><span data-stu-id="22cc6-150">Response</span></span>

<span data-ttu-id="22cc6-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和以下请求对象之一：</span><span class="sxs-lookup"><span data-stu-id="22cc6-151">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="22cc6-152">[mailboxSettings](../resources/mailboxsettings.md) 对象</span><span class="sxs-lookup"><span data-stu-id="22cc6-152">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="22cc6-153">[automaticRepliesSetting](../resources/automaticrepliessetting.md) 对象</span><span class="sxs-lookup"><span data-stu-id="22cc6-153">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="22cc6-154">string （用于**dateFormat**）</span><span class="sxs-lookup"><span data-stu-id="22cc6-154">string (for **dateFormat**)</span></span>
- <span data-ttu-id="22cc6-155">[localeInfo](../resources/localeinfo.md) 对象</span><span class="sxs-lookup"><span data-stu-id="22cc6-155">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="22cc6-156">string （用于**timeFormat**）</span><span class="sxs-lookup"><span data-stu-id="22cc6-156">string (for **timeFormat**)</span></span>
- <span data-ttu-id="22cc6-157">字符串（适用于 **timeZone**）</span><span class="sxs-lookup"><span data-stu-id="22cc6-157">string (for **timeZone**)</span></span>
- [<span data-ttu-id="22cc6-158">workingHours</span><span class="sxs-lookup"><span data-stu-id="22cc6-158">workingHours</span></span>](../resources/workinghours.md)

## <a name="examples"></a><span data-ttu-id="22cc6-159">示例</span><span class="sxs-lookup"><span data-stu-id="22cc6-159">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="22cc6-160">示例 1</span><span class="sxs-lookup"><span data-stu-id="22cc6-160">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="22cc6-161">请求</span><span class="sxs-lookup"><span data-stu-id="22cc6-161">Request</span></span> 
<span data-ttu-id="22cc6-162">第一个示例获取已登录用户邮箱的所有邮箱设置，其中包括自动答复的设置、日期格式、区域设置（语言和国家/地区）、时间格式、时区和工作时间。</span><span class="sxs-lookup"><span data-stu-id="22cc6-162">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for automatic replies, date format, locale (language and country/region), time format, time zone, and working hours.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="22cc6-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="22cc6-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22cc6-164">C#</span><span class="sxs-lookup"><span data-stu-id="22cc6-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22cc6-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22cc6-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22cc6-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22cc6-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="22cc6-167">响应</span><span class="sxs-lookup"><span data-stu-id="22cc6-167">Response</span></span>
<span data-ttu-id="22cc6-168">响应包括已登录用户的所有邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="22cc6-168">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="22cc6-169">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="22cc6-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="22cc6-170">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22cc6-170">All of the properties will be returned from an actual call.</span></span>
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
    },
    "dateFormat": "MM/dd/yyyy",
    "timeFormat": "hh:mm tt"
}
```

### <a name="example-2"></a><span data-ttu-id="22cc6-171">示例 2</span><span class="sxs-lookup"><span data-stu-id="22cc6-171">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="22cc6-172">请求</span><span class="sxs-lookup"><span data-stu-id="22cc6-172">Request</span></span>
<span data-ttu-id="22cc6-173">第二个示例专门获取已登录用户邮箱的自动答复设置。</span><span class="sxs-lookup"><span data-stu-id="22cc6-173">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="22cc6-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="22cc6-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22cc6-175">C#</span><span class="sxs-lookup"><span data-stu-id="22cc6-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22cc6-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22cc6-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22cc6-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22cc6-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="22cc6-178">响应</span><span class="sxs-lookup"><span data-stu-id="22cc6-178">Response</span></span>
<span data-ttu-id="22cc6-p109">该响应仅包括自动答复设置。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22cc6-p109">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="22cc6-182">示例 3</span><span class="sxs-lookup"><span data-stu-id="22cc6-182">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="22cc6-183">请求</span><span class="sxs-lookup"><span data-stu-id="22cc6-183">Request</span></span>
<span data-ttu-id="22cc6-184">第三个示例专门获取已登录用户邮箱的工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="22cc6-184">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
#### <a name="response"></a><span data-ttu-id="22cc6-185">响应</span><span class="sxs-lookup"><span data-stu-id="22cc6-185">Response</span></span>
<span data-ttu-id="22cc6-186">该响应仅包括工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="22cc6-186">The response includes only the working hours settings.</span></span> <span data-ttu-id="22cc6-187">请注意，用户的工作时间在[自定义时区](../resources/customtimezone.md)内。</span><span class="sxs-lookup"><span data-stu-id="22cc6-187">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="22cc6-188">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="22cc6-188">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="22cc6-189">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22cc6-189">All of the properties will be returned from an actual call.</span></span>
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
