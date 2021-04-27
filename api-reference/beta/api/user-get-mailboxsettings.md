---
title: 获取用户的邮箱设置
description: '获取用户的 mailboxSettings。 这包括自动答复设置（自动通知用户 '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fe6e476eb8fdb29fd2817a94f6f7935c86c7006a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051737"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="1aba3-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="1aba3-104">Get user mailbox settings</span></span>

<span data-ttu-id="1aba3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1aba3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1aba3-106">获取用户的 [mailboxSettings](../resources/mailboxsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="1aba3-106">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="1aba3-107">可以查看所有邮箱设置或获取特定设置。</span><span class="sxs-lookup"><span data-stu-id="1aba3-107">You can view all mailbox settings, or get specific settings.</span></span>

<span data-ttu-id="1aba3-108">用户可通过 Outlook 客户端为其邮箱设置以下设置：</span><span class="sxs-lookup"><span data-stu-id="1aba3-108">Users can set the following settings for their mailboxes through an Outlook client:</span></span>

- <span data-ttu-id="1aba3-109">[自动答复](../resources/automaticrepliessetting.md)（收到发件人的电子邮件时自动通知发件人）</span><span class="sxs-lookup"><span data-stu-id="1aba3-109">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="1aba3-110">日期格式</span><span class="sxs-lookup"><span data-stu-id="1aba3-110">date format</span></span>
- <span data-ttu-id="1aba3-111">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="1aba3-111">delegateMeetingMessageDeliveryOptions</span></span>
- <span data-ttu-id="1aba3-112">[区域设置](../resources/localeinfo.md)（语言和国家/地区）</span><span class="sxs-lookup"><span data-stu-id="1aba3-112">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="1aba3-113">时间格式</span><span class="sxs-lookup"><span data-stu-id="1aba3-113">time format</span></span>
- <span data-ttu-id="1aba3-114">时区</span><span class="sxs-lookup"><span data-stu-id="1aba3-114">time zone</span></span>
- [<span data-ttu-id="1aba3-115">工作时间</span><span class="sxs-lookup"><span data-stu-id="1aba3-115">working hours</span></span>](../resources/workinghours.md)
- [<span data-ttu-id="1aba3-116">用户用途</span><span class="sxs-lookup"><span data-stu-id="1aba3-116">user purpose</span></span>](../resources/userpurpose.md)

<span data-ttu-id="1aba3-117">用户可以使用 Outlook 网页版设置首选的日期和时间格式。</span><span class="sxs-lookup"><span data-stu-id="1aba3-117">Users can set their preferred date and time formats using Outlook on the web.</span></span> <span data-ttu-id="1aba3-118">用户可以选择支持的[短日期](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate)或[短时间](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime)格式之一。</span><span class="sxs-lookup"><span data-stu-id="1aba3-118">Users can choose one of the supported [short date](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) formats.</span></span> <span data-ttu-id="1aba3-119">此 `GET` 操作将返回用户选择的格式。</span><span class="sxs-lookup"><span data-stu-id="1aba3-119">This `GET` operation returns the format the user has chosen.</span></span>

<span data-ttu-id="1aba3-120">通过从管理员为其邮箱服务器设置的[支持时区](outlookuser-supportedtimezones.md)中进行选择，用户可以在任何 Outlook 客户端上设置自己喜欢的时区。</span><span class="sxs-lookup"><span data-stu-id="1aba3-120">Users can set the time zone they prefer on any Outlook client, by choosing from the [supported time zones](outlookuser-supportedtimezones.md) that their administrator has set up for their mailbox server.</span></span> <span data-ttu-id="1aba3-121">管理员能够以 Windows 时区格式或者以 [Internet 号码分配局 (IANA) 时区](https://www.iana.org/time-zones)（也称为“Olson 时区”）格式设置时区。</span><span class="sxs-lookup"><span data-stu-id="1aba3-121">The administrator can set up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="1aba3-122">Windows 时区是默认格式。</span><span class="sxs-lookup"><span data-stu-id="1aba3-122">The Windows format is the default.</span></span> 

<span data-ttu-id="1aba3-123">此 `GET` 操作以管理员设置的格式返回用户的首选时区。</span><span class="sxs-lookup"><span data-stu-id="1aba3-123">This `GET` operation returns the user's preferred time zone in the format that the administrator has set up.</span></span> <span data-ttu-id="1aba3-124">若要将时区设置为某种特定格式（Windows 或 IANA），可以先[将相应格式的首选时区更新为邮箱设置](user-update-mailboxsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="1aba3-124">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="1aba3-125">随后便可以获取相应格式的时区。</span><span class="sxs-lookup"><span data-stu-id="1aba3-125">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="1aba3-126">也可以在应用中单独管理格式转换。</span><span class="sxs-lookup"><span data-stu-id="1aba3-126">Alternatively, you can manage the format conversion separately in your app.</span></span> 

## <a name="permissions"></a><span data-ttu-id="1aba3-127">权限</span><span class="sxs-lookup"><span data-stu-id="1aba3-127">Permissions</span></span>
<span data-ttu-id="1aba3-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1aba3-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1aba3-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="1aba3-130">Permission type</span></span>      | <span data-ttu-id="1aba3-131">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1aba3-131">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1aba3-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1aba3-132">Delegated (work or school account)</span></span> | <span data-ttu-id="1aba3-133">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1aba3-133">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1aba3-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1aba3-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aba3-135">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1aba3-135">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1aba3-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="1aba3-136">Application</span></span> | <span data-ttu-id="1aba3-137">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1aba3-137">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1aba3-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1aba3-138">HTTP request</span></span>
<span data-ttu-id="1aba3-139">若要获取用户的所有邮箱设置：</span><span class="sxs-lookup"><span data-stu-id="1aba3-139">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="1aba3-140">若要获取特定设置 - 仅自动答复设置、日期格式、区域设置、时间格式、时区、工作时间或用户用途：</span><span class="sxs-lookup"><span data-stu-id="1aba3-140">To get specific settings - only the automatic replies settings, date format, locale, time format, time zone, working hours, or user purpose:</span></span>
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

GET /me/mailboxSettings/userPurpose
GET /users/{id|userPrincipalName}/mailboxSettings/userPurpose
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1aba3-141">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1aba3-141">Optional query parameters</span></span>
<span data-ttu-id="1aba3-142">此方法支持一些 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1aba3-142">This method supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1aba3-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="1aba3-143">Request headers</span></span>
| <span data-ttu-id="1aba3-144">名称</span><span class="sxs-lookup"><span data-stu-id="1aba3-144">Name</span></span>       | <span data-ttu-id="1aba3-145">类型</span><span class="sxs-lookup"><span data-stu-id="1aba3-145">Type</span></span> | <span data-ttu-id="1aba3-146">说明</span><span class="sxs-lookup"><span data-stu-id="1aba3-146">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1aba3-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="1aba3-147">Authorization</span></span>  | <span data-ttu-id="1aba3-148">string</span><span class="sxs-lookup"><span data-stu-id="1aba3-148">string</span></span>  | <span data-ttu-id="1aba3-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1aba3-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1aba3-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="1aba3-151">Request body</span></span>
<span data-ttu-id="1aba3-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1aba3-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1aba3-153">响应</span><span class="sxs-lookup"><span data-stu-id="1aba3-153">Response</span></span>

<span data-ttu-id="1aba3-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和以下请求对象之一：</span><span class="sxs-lookup"><span data-stu-id="1aba3-154">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="1aba3-155">[mailboxSettings](../resources/mailboxsettings.md) 对象</span><span class="sxs-lookup"><span data-stu-id="1aba3-155">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="1aba3-156">[automaticRepliesSetting](../resources/automaticrepliessetting.md) 对象</span><span class="sxs-lookup"><span data-stu-id="1aba3-156">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="1aba3-157">字符串（适用于 **dateFormat**）</span><span class="sxs-lookup"><span data-stu-id="1aba3-157">string (for **dateFormat**)</span></span>
- <span data-ttu-id="1aba3-158">**delegateMeetingMessageDeliveryOptions** (的字符串) </span><span class="sxs-lookup"><span data-stu-id="1aba3-158">string (for **delegateMeetingMessageDeliveryOptions**)</span></span>
- <span data-ttu-id="1aba3-159">[localeInfo](../resources/localeinfo.md) 对象</span><span class="sxs-lookup"><span data-stu-id="1aba3-159">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="1aba3-160">字符串（适用于 **timeFormat**）</span><span class="sxs-lookup"><span data-stu-id="1aba3-160">string (for **timeFormat**)</span></span>
- <span data-ttu-id="1aba3-161">字符串（适用于 **timeZone**）</span><span class="sxs-lookup"><span data-stu-id="1aba3-161">string (for **timeZone**)</span></span>
- [<span data-ttu-id="1aba3-162">workingHours</span><span class="sxs-lookup"><span data-stu-id="1aba3-162">workingHours</span></span>](../resources/workinghours.md)
- [<span data-ttu-id="1aba3-163">userPurpose</span><span class="sxs-lookup"><span data-stu-id="1aba3-163">userPurpose</span></span>](../resources/userpurpose.md)

## <a name="examples"></a><span data-ttu-id="1aba3-164">示例</span><span class="sxs-lookup"><span data-stu-id="1aba3-164">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="1aba3-165">示例 1</span><span class="sxs-lookup"><span data-stu-id="1aba3-165">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="1aba3-166">请求</span><span class="sxs-lookup"><span data-stu-id="1aba3-166">Request</span></span> 
<span data-ttu-id="1aba3-167">第一个示例获取已登录用户邮箱的所有邮箱设置，其中包括自动答复、日期格式、区域设置 (语言以及国家/地区) 、时间格式、时区、工作时间和用户用途的设置。</span><span class="sxs-lookup"><span data-stu-id="1aba3-167">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for automatic replies, date format, locale (language and country/region), time format, time zone, working hours, and user purpose.</span></span>

# <a name="http"></a>[<span data-ttu-id="1aba3-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="1aba3-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
# <a name="c"></a>[<span data-ttu-id="1aba3-169">C#</span><span class="sxs-lookup"><span data-stu-id="1aba3-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1aba3-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1aba3-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1aba3-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1aba3-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1aba3-172">Java</span><span class="sxs-lookup"><span data-stu-id="1aba3-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1aba3-173">响应</span><span class="sxs-lookup"><span data-stu-id="1aba3-173">Response</span></span>
<span data-ttu-id="1aba3-174">该响应包括已登录用户的所有邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="1aba3-174">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="1aba3-175">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1aba3-175">Note: The response object shown here might be shortened for readability.</span></span>
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
    "userPurpose": {
        "value": "user"
    },
    "dateFormat": "MM/dd/yyyy",
    "timeFormat": "hh:mm tt",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateOnly"
}
```

### <a name="example-2"></a><span data-ttu-id="1aba3-176">示例 2</span><span class="sxs-lookup"><span data-stu-id="1aba3-176">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="1aba3-177">请求</span><span class="sxs-lookup"><span data-stu-id="1aba3-177">Request</span></span>
<span data-ttu-id="1aba3-178">第二个示例专门获取已登录用户邮箱的自动答复设置。</span><span class="sxs-lookup"><span data-stu-id="1aba3-178">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="1aba3-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="1aba3-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
# <a name="c"></a>[<span data-ttu-id="1aba3-180">C#</span><span class="sxs-lookup"><span data-stu-id="1aba3-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1aba3-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1aba3-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1aba3-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1aba3-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1aba3-183">Java</span><span class="sxs-lookup"><span data-stu-id="1aba3-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1aba3-184">响应</span><span class="sxs-lookup"><span data-stu-id="1aba3-184">Response</span></span>
<span data-ttu-id="1aba3-185">该响应仅包括自动答复设置。</span><span class="sxs-lookup"><span data-stu-id="1aba3-185">The response includes only the automatic replies settings.</span></span> <span data-ttu-id="1aba3-186">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1aba3-186">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="1aba3-187">示例 3</span><span class="sxs-lookup"><span data-stu-id="1aba3-187">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="1aba3-188">请求</span><span class="sxs-lookup"><span data-stu-id="1aba3-188">Request</span></span>
<span data-ttu-id="1aba3-189">第三个示例专门获取已登录用户邮箱的工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="1aba3-189">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
#### <a name="response"></a><span data-ttu-id="1aba3-190">响应</span><span class="sxs-lookup"><span data-stu-id="1aba3-190">Response</span></span>
<span data-ttu-id="1aba3-191">该响应仅包括工作时间设置。</span><span class="sxs-lookup"><span data-stu-id="1aba3-191">The response includes only the working hours settings.</span></span> <span data-ttu-id="1aba3-192">请注意，用户的工作时间在[自定义时区](../resources/customtimezone.md)内。</span><span class="sxs-lookup"><span data-stu-id="1aba3-192">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="1aba3-193">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1aba3-193">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-4"></a><span data-ttu-id="1aba3-194">示例 4</span><span class="sxs-lookup"><span data-stu-id="1aba3-194">Example 4</span></span>
#### <a name="request"></a><span data-ttu-id="1aba3-195">请求</span><span class="sxs-lookup"><span data-stu-id="1aba3-195">Request</span></span>
<span data-ttu-id="1aba3-196">第四个示例专门获取已 [登录](../resources/userpurpose.md) 用户邮箱的用户用途设置。</span><span class="sxs-lookup"><span data-stu-id="1aba3-196">The fourth example gets specifically the [user purpose](../resources/userpurpose.md) settings of the signed-in user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="1aba3-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="1aba3-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings/userPurpose
```
# <a name="c"></a>[<span data-ttu-id="1aba3-198">C#</span><span class="sxs-lookup"><span data-stu-id="1aba3-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1aba3-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1aba3-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1aba3-200">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1aba3-200">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1aba3-201">Java</span><span class="sxs-lookup"><span data-stu-id="1aba3-201">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1aba3-202">响应</span><span class="sxs-lookup"><span data-stu-id="1aba3-202">Response</span></span>
<span data-ttu-id="1aba3-203">该响应仅包括 [用户目的](../resources/userpurpose.md) 设置。</span><span class="sxs-lookup"><span data-stu-id="1aba3-203">The response includes only the [user purpose](../resources/userpurpose.md) settings.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_mailboxsettings_4",
  "truncated": true,
  "@odata.type": "microsoft.graph.userPurpose"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('622eaaff-0683-4862-9de4-f2ec83c2bd98')/mailboxSettings/userPurpose",
    "value": "user"
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
