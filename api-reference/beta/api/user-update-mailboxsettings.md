---
title: 获取用户的邮箱设置
description: 更新用户邮箱的一个或多个设置。 这包括自动答复的设置（在收到电子邮件时自动通知人员）、区域设置（语言和国家/地区）、时区和工作时间。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 667770b069e1a190cebf3bb48133dae92e291da0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938153"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="70302-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="70302-104">Update user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70302-105">启用、配置或禁用以下一个或多个设置作为用户的[mailboxSettings](../resources/mailboxsettings.md)的一部分：</span><span class="sxs-lookup"><span data-stu-id="70302-105">Enable, configure, or disable one or more of the following settings as part of a user's [mailboxSettings](../resources/mailboxsettings.md):</span></span>

- <span data-ttu-id="70302-106">[自动答复](../resources/automaticrepliessetting.md)（收到发件人的电子邮件时自动通知发件人）</span><span class="sxs-lookup"><span data-stu-id="70302-106">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="70302-107">dateFormat</span><span class="sxs-lookup"><span data-stu-id="70302-107">dateFormat</span></span>
- <span data-ttu-id="70302-108">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="70302-108">delegateMeetingMessageDeliveryOptions</span></span>
- <span data-ttu-id="70302-109">[区域设置](../resources/localeinfo.md)（语言和国家/地区）</span><span class="sxs-lookup"><span data-stu-id="70302-109">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="70302-110">timeFormat</span><span class="sxs-lookup"><span data-stu-id="70302-110">timeFormat</span></span>
- <span data-ttu-id="70302-111">时区</span><span class="sxs-lookup"><span data-stu-id="70302-111">time zone</span></span>
- [<span data-ttu-id="70302-112">工作时间</span><span class="sxs-lookup"><span data-stu-id="70302-112">working hours</span></span>](../resources/workinghours.md)

<span data-ttu-id="70302-113">更新用户的首选日期或时间格式时，请分别指定[短日期](https://docs.microsoft.com/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate)或[短时间](https://docs.microsoft.com/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime)格式。</span><span class="sxs-lookup"><span data-stu-id="70302-113">When updating the preferred date or time format for a user, specify it in respectively, the [short date](https://docs.microsoft.com/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](https://docs.microsoft.com/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) format.</span></span> 

<span data-ttu-id="70302-114">更新用户的首选时区时，在 Windows 或[Internet 分配的号码颁发机构（IANA）](https://www.iana.org/time-zones)的时区（也称为 "Olson 时区"）格式中指定它。</span><span class="sxs-lookup"><span data-stu-id="70302-114">When updating the preferred time zone for a user, specify it in the Windows or [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="70302-115">您还可以进一步自定义时区，如下面的[示例 2](#example-2)所示。</span><span class="sxs-lookup"><span data-stu-id="70302-115">You can also further customize the time zone as shown in [example 2](#example-2) below.</span></span>

> [!TIP] 
> <span data-ttu-id="70302-116">您不能创建或删除任何邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="70302-116">You cannot create or delete any mailbox settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="70302-117">权限</span><span class="sxs-lookup"><span data-stu-id="70302-117">Permissions</span></span>
<span data-ttu-id="70302-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70302-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70302-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="70302-120">Permission type</span></span>      | <span data-ttu-id="70302-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70302-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70302-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70302-122">Delegated (work or school account)</span></span> | <span data-ttu-id="70302-123">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70302-123">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="70302-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70302-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70302-125">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70302-125">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="70302-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="70302-126">Application</span></span> | <span data-ttu-id="70302-127">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70302-127">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="70302-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70302-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="70302-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="70302-129">Optional query parameters</span></span>
<span data-ttu-id="70302-130">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="70302-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="70302-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="70302-131">Request headers</span></span>
| <span data-ttu-id="70302-132">名称</span><span class="sxs-lookup"><span data-stu-id="70302-132">Name</span></span>       | <span data-ttu-id="70302-133">类型</span><span class="sxs-lookup"><span data-stu-id="70302-133">Type</span></span> | <span data-ttu-id="70302-134">说明</span><span class="sxs-lookup"><span data-stu-id="70302-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="70302-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="70302-135">Authorization</span></span>  | <span data-ttu-id="70302-136">string</span><span class="sxs-lookup"><span data-stu-id="70302-136">string</span></span>  | <span data-ttu-id="70302-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70302-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70302-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="70302-139">Request body</span></span>
<span data-ttu-id="70302-p105">在请求正文中，提供应更新的相关属性的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。以下是可写/可更新的属性：</span><span class="sxs-lookup"><span data-stu-id="70302-p105">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="70302-144">属性</span><span class="sxs-lookup"><span data-stu-id="70302-144">Property</span></span>     | <span data-ttu-id="70302-145">类型</span><span class="sxs-lookup"><span data-stu-id="70302-145">Type</span></span>   |<span data-ttu-id="70302-146">描述</span><span class="sxs-lookup"><span data-stu-id="70302-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70302-147">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="70302-147">automaticRepliesSetting</span></span>|[<span data-ttu-id="70302-148">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="70302-148">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="70302-149">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="70302-149">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="70302-150">只能将此类通知设置为将来日期范围。</span><span class="sxs-lookup"><span data-stu-id="70302-150">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="70302-151">dateFormat</span><span class="sxs-lookup"><span data-stu-id="70302-151">dateFormat</span></span>|<span data-ttu-id="70302-152">string</span><span class="sxs-lookup"><span data-stu-id="70302-152">string</span></span>|<span data-ttu-id="70302-153">用户邮箱的日期格式。</span><span class="sxs-lookup"><span data-stu-id="70302-153">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="70302-154">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="70302-154">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="70302-155">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="70302-155">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="70302-156">如果用户具有日历代理，则指定代理、邮箱所有者，还是同时接收会议邮件和会议响应。</span><span class="sxs-lookup"><span data-stu-id="70302-156">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="70302-157">可取值为：`sendToDelegateAndInformationToPrincipal`、`sendToDelegateAndPrincipal`、`sendToDelegateOnly`。</span><span class="sxs-lookup"><span data-stu-id="70302-157">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="70302-158">语言</span><span class="sxs-lookup"><span data-stu-id="70302-158">language</span></span>|[<span data-ttu-id="70302-159">localeInfo</span><span class="sxs-lookup"><span data-stu-id="70302-159">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="70302-160">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="70302-160">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="70302-161">timeFormat</span><span class="sxs-lookup"><span data-stu-id="70302-161">timeFormat</span></span>|<span data-ttu-id="70302-162">string</span><span class="sxs-lookup"><span data-stu-id="70302-162">string</span></span>|<span data-ttu-id="70302-163">用户邮箱的时间格式。</span><span class="sxs-lookup"><span data-stu-id="70302-163">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="70302-164">timeZone</span><span class="sxs-lookup"><span data-stu-id="70302-164">timeZone</span></span>|<span data-ttu-id="70302-165">string</span><span class="sxs-lookup"><span data-stu-id="70302-165">string</span></span>|<span data-ttu-id="70302-166">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="70302-166">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="70302-167">workingHours</span><span class="sxs-lookup"><span data-stu-id="70302-167">workingHours</span></span>|[<span data-ttu-id="70302-168">workingHours</span><span class="sxs-lookup"><span data-stu-id="70302-168">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="70302-169">用户工作的小时数、一周的天数和时区。</span><span class="sxs-lookup"><span data-stu-id="70302-169">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="70302-170">响应</span><span class="sxs-lookup"><span data-stu-id="70302-170">Response</span></span>

<span data-ttu-id="70302-171">如果成功，此方法在响应`200 OK`正文中返回响应代码和[mailboxSettings](../resources/mailboxsettings.md)对象的更新的属性。</span><span class="sxs-lookup"><span data-stu-id="70302-171">If successful, this method returns a `200 OK` response code and the updated properties of a [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="70302-172">错误</span><span class="sxs-lookup"><span data-stu-id="70302-172">Errors</span></span>

<span data-ttu-id="70302-173">将工作时间设置为不适当的值可能会返回以下错误。</span><span class="sxs-lookup"><span data-stu-id="70302-173">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="70302-174">应用场景</span><span class="sxs-lookup"><span data-stu-id="70302-174">Scenario</span></span>   | <span data-ttu-id="70302-175">HTTP 状态代码</span><span class="sxs-lookup"><span data-stu-id="70302-175">HTTP status code</span></span> | <span data-ttu-id="70302-176">错误代码</span><span class="sxs-lookup"><span data-stu-id="70302-176">Error code</span></span> | <span data-ttu-id="70302-177">错误消息</span><span class="sxs-lookup"><span data-stu-id="70302-177">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="70302-178">**startTime** 或 **endTime** 无效</span><span class="sxs-lookup"><span data-stu-id="70302-178">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="70302-179">400</span><span class="sxs-lookup"><span data-stu-id="70302-179">400</span></span> | <span data-ttu-id="70302-180">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="70302-180">RequestBodyRead</span></span> | <span data-ttu-id="70302-181">无法将文本“08”转换为预期类型“Edm.TimeOfDay”。</span><span class="sxs-lookup"><span data-stu-id="70302-181">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="70302-182">开始时间大于结束时间</span><span class="sxs-lookup"><span data-stu-id="70302-182">Start time is greater than end time</span></span> | <span data-ttu-id="70302-183">400</span><span class="sxs-lookup"><span data-stu-id="70302-183">400</span></span> | <span data-ttu-id="70302-184">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="70302-184">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="70302-185">开始时间应早于结束时间。</span><span class="sxs-lookup"><span data-stu-id="70302-185">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="70302-186">**daysOfWeek** 中的天数无效</span><span class="sxs-lookup"><span data-stu-id="70302-186">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="70302-187">400</span><span class="sxs-lookup"><span data-stu-id="70302-187">400</span></span> | <span data-ttu-id="70302-188">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="70302-188">InvalidArguments</span></span> | <span data-ttu-id="70302-189">未找到请求值“RandomDay”。</span><span class="sxs-lookup"><span data-stu-id="70302-189">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="70302-190">**timeZone** 无效</span><span class="sxs-lookup"><span data-stu-id="70302-190">Invalid **timeZone**</span></span> | <span data-ttu-id="70302-191">400</span><span class="sxs-lookup"><span data-stu-id="70302-191">400</span></span> | <span data-ttu-id="70302-192">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="70302-192">InvalidTimeZone</span></span> | <span data-ttu-id="70302-193">提供的时区设置无效。</span><span class="sxs-lookup"><span data-stu-id="70302-193">Time Zone settings provided are invalid.</span></span>|


## <a name="examples"></a><span data-ttu-id="70302-194">示例</span><span class="sxs-lookup"><span data-stu-id="70302-194">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="70302-195">示例 1</span><span class="sxs-lookup"><span data-stu-id="70302-195">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="70302-196">请求</span><span class="sxs-lookup"><span data-stu-id="70302-196">Request</span></span> 
<span data-ttu-id="70302-197">第一个示例通过设置 **automaticRepliesSetting** 属性的以下属性来启用对日期范围的自动答复：**status**、**scheduledStartDateTime** 和 **scheduledEndDateTime**。</span><span class="sxs-lookup"><span data-stu-id="70302-197">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="70302-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="70302-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings_1"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "scheduledStartDateTime": {
          "dateTime": "2016-03-20T18:00:00.0000000",
          "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
          "dateTime": "2016-03-28T18:00:00.0000000",
          "timeZone": "UTC"
        }
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70302-199">C#</span><span class="sxs-lookup"><span data-stu-id="70302-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70302-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70302-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70302-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70302-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="70302-202">响应</span><span class="sxs-lookup"><span data-stu-id="70302-202">Response</span></span>
<span data-ttu-id="70302-203">该响应包括自动答复的更新设置。</span><span class="sxs-lookup"><span data-stu-id="70302-203">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="70302-204">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="70302-204">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="70302-205">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70302-205">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "update_mailboxsettings_1",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "all",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-20T02:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T02:00:00.0000000",
            "timeZone": "UTC"
        },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    }
}
```

### <a name="example-2"></a><span data-ttu-id="70302-206">示例 2</span><span class="sxs-lookup"><span data-stu-id="70302-206">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="70302-207">请求</span><span class="sxs-lookup"><span data-stu-id="70302-207">Request</span></span>
<span data-ttu-id="70302-208">第二个示例通过将 **timeZone** 属性设置为[自定义时区](../resources/customtimezone.md)，为登录用户的工作时间自定义时区。</span><span class="sxs-lookup"><span data-stu-id="70302-208">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailboxSettings
Content-Type: application/json

{
  "workingHours": {
      "endTime" : "18:30:00.0000000", 
      "daysOfWeek": [ 
          "Monday", 
          "Tuesday", 
          "Wednesday", 
          "Thursday", 
          "Friday", 
          "Saturday" 
      ], 
      "timeZone" : { 
         "@odata.type": "#microsoft.graph.customTimeZone", 
         "bias":-300, 
         "name": "Customized Time Zone",
         "standardOffset":{   
           "time":"02:00:00.0000000", 
           "dayOccurrence":2, 
           "dayOfWeek":"Sunday", 
           "month":10, 
           "year":0 
         }, 
         "daylightOffset":{   
           "daylightBias":100, 
           "time":"02:00:00.0000000", 
           "dayOccurrence":4, 
           "dayOfWeek":"Sunday", 
           "month":5, 
           "year":0 
         } 
      } 
  }
} 
```
#### <a name="response"></a><span data-ttu-id="70302-209">响应</span><span class="sxs-lookup"><span data-stu-id="70302-209">Response</span></span>
<span data-ttu-id="70302-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70302-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
    "workingHours":{
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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
