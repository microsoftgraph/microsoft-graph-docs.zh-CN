---
title: 获取用户的邮箱设置
description: '获取用户的 mailboxSettings。 这包括自动答复设置（自动通知用户 '
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 42a19bc64e8be7d5e12d3d49b1342a696a1d47cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069602"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="90324-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="90324-104">Get user mailbox settings</span></span>

<span data-ttu-id="90324-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90324-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90324-106">获取用户的 [mailboxSettings](../resources/mailboxsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="90324-106">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="90324-107">可以查看所有邮箱设置或获取特定设置。</span><span class="sxs-lookup"><span data-stu-id="90324-107">You can view all mailbox settings, or get specific settings.</span></span>

<span data-ttu-id="90324-108">用户可通过 Outlook 客户端为其邮箱设置以下设置：</span><span class="sxs-lookup"><span data-stu-id="90324-108">Users can set the following settings for their mailboxes through an Outlook client:</span></span>

- <span data-ttu-id="90324-109">[自动答复](../resources/automaticrepliessetting.md)（收到发件人的电子邮件时自动通知发件人）</span><span class="sxs-lookup"><span data-stu-id="90324-109">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="90324-110">日期格式</span><span class="sxs-lookup"><span data-stu-id="90324-110">date format</span></span>
- <span data-ttu-id="90324-111">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="90324-111">delegateMeetingMessageDeliveryOptions</span></span>
- <span data-ttu-id="90324-112">[区域设置](../resources/localeinfo.md)（语言和国家/地区）</span><span class="sxs-lookup"><span data-stu-id="90324-112">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="90324-113">时间格式</span><span class="sxs-lookup"><span data-stu-id="90324-113">time format</span></span>
- <span data-ttu-id="90324-114">时区</span><span class="sxs-lookup"><span data-stu-id="90324-114">time zone</span></span>
- [<span data-ttu-id="90324-115">工作时间</span><span class="sxs-lookup"><span data-stu-id="90324-115">working hours</span></span>](../resources/workinghours.md)

<span data-ttu-id="90324-116">用户可以使用 Outlook 网页版设置首选的日期和时间格式。</span><span class="sxs-lookup"><span data-stu-id="90324-116">Users can set their preferred date and time formats using Outlook on the web.</span></span> <span data-ttu-id="90324-117">用户可以选择支持的[短日期](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate)或[短时间](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime)格式之一。</span><span class="sxs-lookup"><span data-stu-id="90324-117">Users can choose one of the supported [short date](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) formats.</span></span> <span data-ttu-id="90324-118">此 `GET` 操作将返回用户选择的格式。</span><span class="sxs-lookup"><span data-stu-id="90324-118">This `GET` operation returns the format the user has chosen.</span></span>

<span data-ttu-id="90324-119">通过从管理员为其邮箱服务器设置的[支持时区](outlookuser-supportedtimezones.md)中进行选择，用户可以在任何 Outlook 客户端上设置自己喜欢的时区。</span><span class="sxs-lookup"><span data-stu-id="90324-119">Users can set the time zone they prefer on any Outlook client, by choosing from the [supported time zones](outlookuser-supportedtimezones.md) that their administrator has set up for their mailbox server.</span></span> <span data-ttu-id="90324-120">管理员能够以 Windows 时区格式或者以 [Internet 号码分配局 (IANA) 时区](https://www.iana.org/time-zones)（也称为“Olson 时区”）格式设置时区。</span><span class="sxs-lookup"><span data-stu-id="90324-120">The administrator can set up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="90324-121">Windows 时区是默认格式。</span><span class="sxs-lookup"><span data-stu-id="90324-121">The Windows format is the default.</span></span>

<span data-ttu-id="90324-122">此 `GET` 操作以管理员设置的格式返回用户的首选时区。</span><span class="sxs-lookup"><span data-stu-id="90324-122">This `GET` operation returns the user's preferred time zone in the format that the administrator has set up.</span></span> <span data-ttu-id="90324-123">若要将时区设置为某种特定格式（Windows 或 IANA），可以先[将相应格式的首选时区更新为邮箱设置](user-update-mailboxsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="90324-123">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="90324-124">随后便可以获取相应格式的时区。</span><span class="sxs-lookup"><span data-stu-id="90324-124">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="90324-125">也可以在应用中单独管理格式转换。</span><span class="sxs-lookup"><span data-stu-id="90324-125">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="90324-126">权限</span><span class="sxs-lookup"><span data-stu-id="90324-126">Permissions</span></span>
<span data-ttu-id="90324-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90324-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90324-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="90324-129">Permission type</span></span>      | <span data-ttu-id="90324-130">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90324-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90324-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90324-131">Delegated (work or school account)</span></span> | <span data-ttu-id="90324-132">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90324-132">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="90324-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90324-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90324-134">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90324-134">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="90324-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="90324-135">Application</span></span> | <span data-ttu-id="90324-136">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90324-136">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="90324-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90324-137">HTTP request</span></span>
<span data-ttu-id="90324-138">若要获取用户的所有邮箱设置：</span><span class="sxs-lookup"><span data-stu-id="90324-138">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="90324-139">若要获取特定设置 - 仅限自动答复设置、日期格式、区域设置、时间格式、时区或工作时间：</span><span class="sxs-lookup"><span data-stu-id="90324-139">To get specific settings - only the automatic replies settings, date format, locale, time format, time zone, or working hours:</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="90324-140">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="90324-140">Optional query parameters</span></span>
<span data-ttu-id="90324-141">此方法支持一些 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="90324-141">This method supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="90324-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="90324-142">Request headers</span></span>
| <span data-ttu-id="90324-143">名称</span><span class="sxs-lookup"><span data-stu-id="90324-143">Name</span></span>       | <span data-ttu-id="90324-144">类型</span><span class="sxs-lookup"><span data-stu-id="90324-144">Type</span></span> | <span data-ttu-id="90324-145">说明</span><span class="sxs-lookup"><span data-stu-id="90324-145">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="90324-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="90324-146">Authorization</span></span>  | <span data-ttu-id="90324-147">string</span><span class="sxs-lookup"><span data-stu-id="90324-147">string</span></span>  | <span data-ttu-id="90324-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90324-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90324-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="90324-150">Request body</span></span>
<span data-ttu-id="90324-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90324-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90324-152">响应</span><span class="sxs-lookup"><span data-stu-id="90324-152">Response</span></span>

<span data-ttu-id="90324-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和以下请求对象之一：</span><span class="sxs-lookup"><span data-stu-id="90324-153">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="90324-154">[mailboxSettings](../resources/mailboxsettings.md) 对象</span><span class="sxs-lookup"><span data-stu-id="90324-154">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="90324-155">[automaticRepliesSetting](../resources/automaticrepliessetting.md) 对象</span><span class="sxs-lookup"><span data-stu-id="90324-155">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="90324-156">字符串（适用于 **dateFormat**）</span><span class="sxs-lookup"><span data-stu-id="90324-156">string (for **dateFormat**)</span></span>
- <span data-ttu-id="90324-157">**delegateMeetingMessageDeliveryOptions**的字符串 () </span><span class="sxs-lookup"><span data-stu-id="90324-157">string (for **delegateMeetingMessageDeliveryOptions**)</span></span>
- <span data-ttu-id="90324-158">[localeInfo](../resources/localeinfo.md) 对象</span><span class="sxs-lookup"><span data-stu-id="90324-158">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="90324-159">字符串（适用于 **timeFormat**）</span><span class="sxs-lookup"><span data-stu-id="90324-159">string (for **timeFormat**)</span></span>
- <span data-ttu-id="90324-160">字符串（适用于 **timeZone**）</span><span class="sxs-lookup"><span data-stu-id="90324-160">string (for **timeZone**)</span></span>
- [<span data-ttu-id="90324-161">workingHours</span><span class="sxs-lookup"><span data-stu-id="90324-161">workingHours</span></span>](../resources/workinghours.md)

## <a name="examples"></a><span data-ttu-id="90324-162">示例</span><span class="sxs-lookup"><span data-stu-id="90324-162">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="90324-163">示例 1</span><span class="sxs-lookup"><span data-stu-id="90324-163">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="90324-164">请求</span><span class="sxs-lookup"><span data-stu-id="90324-164">Request</span></span>
<span data-ttu-id="90324-165">第一个示例获取已登录用户邮箱的所有邮箱设置，其中包括自动答复、日期格式、区域设置（语言和国家/地区）、时间格式、时区和工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="90324-165">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for automatic replies, date format, locale (language and country/region), time format, time zone, and working hours.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```

#### <a name="response"></a><span data-ttu-id="90324-166">响应</span><span class="sxs-lookup"><span data-stu-id="90324-166">Response</span></span>
<span data-ttu-id="90324-167">该响应包括已登录用户的所有邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="90324-167">The response includes all the mailbox settings of the signed-in user.</span></span>
<span data-ttu-id="90324-168">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="90324-168">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="90324-169">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90324-169">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2"></a><span data-ttu-id="90324-170">示例 2</span><span class="sxs-lookup"><span data-stu-id="90324-170">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="90324-171">请求</span><span class="sxs-lookup"><span data-stu-id="90324-171">Request</span></span>
<span data-ttu-id="90324-172">第二个示例专门获取已登录用户邮箱的自动答复设置。</span><span class="sxs-lookup"><span data-stu-id="90324-172">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="90324-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="90324-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
# <a name="c"></a>[<span data-ttu-id="90324-174">C#</span><span class="sxs-lookup"><span data-stu-id="90324-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90324-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90324-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90324-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90324-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90324-177">Java</span><span class="sxs-lookup"><span data-stu-id="90324-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="90324-178">响应</span><span class="sxs-lookup"><span data-stu-id="90324-178">Response</span></span>
<span data-ttu-id="90324-p109">该响应仅包括自动答复设置。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90324-p109">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="90324-182">示例 3</span><span class="sxs-lookup"><span data-stu-id="90324-182">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="90324-183">请求</span><span class="sxs-lookup"><span data-stu-id="90324-183">Request</span></span>
<span data-ttu-id="90324-184">第三个示例专门获取已登录用户邮箱的工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="90324-184">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/workingHours
```
#### <a name="response"></a><span data-ttu-id="90324-185">响应</span><span class="sxs-lookup"><span data-stu-id="90324-185">Response</span></span>
<span data-ttu-id="90324-186">该响应仅包括工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="90324-186">The response includes only the working hours settings.</span></span> <span data-ttu-id="90324-187">请注意，用户的工作时间在[自定义时区](../resources/customtimezone.md)内。</span><span class="sxs-lookup"><span data-stu-id="90324-187">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span>
<span data-ttu-id="90324-188">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="90324-188">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="90324-189">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90324-189">All of the properties will be returned from an actual call.</span></span>
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

