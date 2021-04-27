---
title: 获取用户的邮箱设置
description: 更新用户邮箱的一个或多个设置。这包括自动答复（收到发件人的电子邮件时自动通知发件人）、区域设置（语言和国家/地区）、时区和工作时间的设置。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: af2c46084d09f8bb8b1799ac87a32e951038b610
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053340"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="535fe-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="535fe-104">Update user mailbox settings</span></span>

<span data-ttu-id="535fe-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="535fe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="535fe-106">在用户的 [mailboxSettings](../resources/mailboxsettings.md)中启用、配置或禁用以下一个或多个设置：</span><span class="sxs-lookup"><span data-stu-id="535fe-106">Enable, configure, or disable one or more of the following settings as part of a user's [mailboxSettings](../resources/mailboxsettings.md):</span></span>

- <span data-ttu-id="535fe-107">[自动答复](../resources/automaticrepliessetting.md)（收到发件人的电子邮件时自动通知发件人）</span><span class="sxs-lookup"><span data-stu-id="535fe-107">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="535fe-108">dateFormat</span><span class="sxs-lookup"><span data-stu-id="535fe-108">dateFormat</span></span>
- <span data-ttu-id="535fe-109">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="535fe-109">delegateMeetingMessageDeliveryOptions</span></span>
- <span data-ttu-id="535fe-110">[区域设置](../resources/localeinfo.md)（语言和国家/地区）</span><span class="sxs-lookup"><span data-stu-id="535fe-110">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="535fe-111">timeFormat</span><span class="sxs-lookup"><span data-stu-id="535fe-111">timeFormat</span></span>
- <span data-ttu-id="535fe-112">时区</span><span class="sxs-lookup"><span data-stu-id="535fe-112">time zone</span></span>
- [<span data-ttu-id="535fe-113">工作时间</span><span class="sxs-lookup"><span data-stu-id="535fe-113">working hours</span></span>](../resources/workinghours.md)

<span data-ttu-id="535fe-114">更新用户的首选日期或时间格式时，请分别以短日期 [或短时间](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) 格式 [指定它](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) 。</span><span class="sxs-lookup"><span data-stu-id="535fe-114">When updating the preferred date or time format for a user, specify it in respectively, the [short date](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) format.</span></span> 

<span data-ttu-id="535fe-115">更新用户的首选时区时，在 Windows 或 Internet 号码分配机构 ([IANA](https://www.iana.org/time-zones)) 时区 (也称为 Olson 时区) 格式进行指定。</span><span class="sxs-lookup"><span data-stu-id="535fe-115">When updating the preferred time zone for a user, specify it in the Windows or [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="535fe-116">您还可以进一步自定义时区，如下面的示例 [2](#example-2) 所示。</span><span class="sxs-lookup"><span data-stu-id="535fe-116">You can also further customize the time zone as shown in [example 2](#example-2) below.</span></span>

> [!TIP] 
> <span data-ttu-id="535fe-117">不能创建或删除任何邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="535fe-117">You cannot create or delete any mailbox settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="535fe-118">权限</span><span class="sxs-lookup"><span data-stu-id="535fe-118">Permissions</span></span>
<span data-ttu-id="535fe-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="535fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="535fe-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="535fe-121">Permission type</span></span>      | <span data-ttu-id="535fe-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="535fe-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="535fe-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="535fe-123">Delegated (work or school account)</span></span> | <span data-ttu-id="535fe-124">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="535fe-124">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="535fe-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="535fe-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="535fe-126">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="535fe-126">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="535fe-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="535fe-127">Application</span></span> | <span data-ttu-id="535fe-128">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="535fe-128">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="535fe-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="535fe-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="535fe-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="535fe-130">Optional query parameters</span></span>
<span data-ttu-id="535fe-131">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="535fe-131">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="535fe-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="535fe-132">Request headers</span></span>
| <span data-ttu-id="535fe-133">名称</span><span class="sxs-lookup"><span data-stu-id="535fe-133">Name</span></span>       | <span data-ttu-id="535fe-134">类型</span><span class="sxs-lookup"><span data-stu-id="535fe-134">Type</span></span> | <span data-ttu-id="535fe-135">说明</span><span class="sxs-lookup"><span data-stu-id="535fe-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="535fe-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="535fe-136">Authorization</span></span>  | <span data-ttu-id="535fe-137">string</span><span class="sxs-lookup"><span data-stu-id="535fe-137">string</span></span>  | <span data-ttu-id="535fe-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="535fe-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="535fe-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="535fe-140">Request body</span></span>
<span data-ttu-id="535fe-p105">在请求正文中，提供应更新的相关属性的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。以下是可写/可更新的属性：</span><span class="sxs-lookup"><span data-stu-id="535fe-p105">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="535fe-145">属性</span><span class="sxs-lookup"><span data-stu-id="535fe-145">Property</span></span>     | <span data-ttu-id="535fe-146">类型</span><span class="sxs-lookup"><span data-stu-id="535fe-146">Type</span></span>   |<span data-ttu-id="535fe-147">说明</span><span class="sxs-lookup"><span data-stu-id="535fe-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="535fe-148">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="535fe-148">automaticRepliesSetting</span></span>|[<span data-ttu-id="535fe-149">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="535fe-149">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="535fe-150">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="535fe-150">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="535fe-151">只能为将来的日期范围设置此类通知。</span><span class="sxs-lookup"><span data-stu-id="535fe-151">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="535fe-152">dateFormat</span><span class="sxs-lookup"><span data-stu-id="535fe-152">dateFormat</span></span>|<span data-ttu-id="535fe-153">string</span><span class="sxs-lookup"><span data-stu-id="535fe-153">string</span></span>|<span data-ttu-id="535fe-154">用户邮箱的日期格式。</span><span class="sxs-lookup"><span data-stu-id="535fe-154">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="535fe-155">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="535fe-155">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="535fe-156">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="535fe-156">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="535fe-157">如果用户具有日历代理，则指定代理人、邮箱所有者还是同时接收会议邮件和会议响应。</span><span class="sxs-lookup"><span data-stu-id="535fe-157">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="535fe-158">可取值为：`sendToDelegateAndInformationToPrincipal`、`sendToDelegateAndPrincipal`、`sendToDelegateOnly`。</span><span class="sxs-lookup"><span data-stu-id="535fe-158">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="535fe-159">语言</span><span class="sxs-lookup"><span data-stu-id="535fe-159">language</span></span>|[<span data-ttu-id="535fe-160">localeInfo</span><span class="sxs-lookup"><span data-stu-id="535fe-160">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="535fe-161">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="535fe-161">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="535fe-162">timeFormat</span><span class="sxs-lookup"><span data-stu-id="535fe-162">timeFormat</span></span>|<span data-ttu-id="535fe-163">string</span><span class="sxs-lookup"><span data-stu-id="535fe-163">string</span></span>|<span data-ttu-id="535fe-164">用户邮箱的时间格式。</span><span class="sxs-lookup"><span data-stu-id="535fe-164">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="535fe-165">timeZone</span><span class="sxs-lookup"><span data-stu-id="535fe-165">timeZone</span></span>|<span data-ttu-id="535fe-166">string</span><span class="sxs-lookup"><span data-stu-id="535fe-166">string</span></span>|<span data-ttu-id="535fe-167">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="535fe-167">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="535fe-168">workingHours</span><span class="sxs-lookup"><span data-stu-id="535fe-168">workingHours</span></span>|[<span data-ttu-id="535fe-169">workingHours</span><span class="sxs-lookup"><span data-stu-id="535fe-169">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="535fe-170">用户工作的小时数、一周的天数和时区。</span><span class="sxs-lookup"><span data-stu-id="535fe-170">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="535fe-171">响应</span><span class="sxs-lookup"><span data-stu-id="535fe-171">Response</span></span>

<span data-ttu-id="535fe-172">如果成功，此方法在响应 `200 OK` 正文中返回 [响应代码和 mailboxSettings](../resources/mailboxsettings.md) 对象的更新属性。</span><span class="sxs-lookup"><span data-stu-id="535fe-172">If successful, this method returns a `200 OK` response code and the updated properties of a [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="535fe-173">错误</span><span class="sxs-lookup"><span data-stu-id="535fe-173">Errors</span></span>

<span data-ttu-id="535fe-174">将工作时间设置为不适当的值可能会返回以下错误。</span><span class="sxs-lookup"><span data-stu-id="535fe-174">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="535fe-175">应用场景</span><span class="sxs-lookup"><span data-stu-id="535fe-175">Scenario</span></span>   | <span data-ttu-id="535fe-176">HTTP 状态代码</span><span class="sxs-lookup"><span data-stu-id="535fe-176">HTTP status code</span></span> | <span data-ttu-id="535fe-177">错误代码</span><span class="sxs-lookup"><span data-stu-id="535fe-177">Error code</span></span> | <span data-ttu-id="535fe-178">错误消息</span><span class="sxs-lookup"><span data-stu-id="535fe-178">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="535fe-179">**startTime** 或 **endTime** 无效</span><span class="sxs-lookup"><span data-stu-id="535fe-179">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="535fe-180">400</span><span class="sxs-lookup"><span data-stu-id="535fe-180">400</span></span> | <span data-ttu-id="535fe-181">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="535fe-181">RequestBodyRead</span></span> | <span data-ttu-id="535fe-182">无法将文本“08”转换为预期类型“Edm.TimeOfDay”。</span><span class="sxs-lookup"><span data-stu-id="535fe-182">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="535fe-183">开始时间大于结束时间</span><span class="sxs-lookup"><span data-stu-id="535fe-183">Start time is greater than end time</span></span> | <span data-ttu-id="535fe-184">400</span><span class="sxs-lookup"><span data-stu-id="535fe-184">400</span></span> | <span data-ttu-id="535fe-185">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="535fe-185">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="535fe-186">开始时间应早于结束时间。</span><span class="sxs-lookup"><span data-stu-id="535fe-186">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="535fe-187">**daysOfWeek** 中的天数无效</span><span class="sxs-lookup"><span data-stu-id="535fe-187">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="535fe-188">400</span><span class="sxs-lookup"><span data-stu-id="535fe-188">400</span></span> | <span data-ttu-id="535fe-189">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="535fe-189">InvalidArguments</span></span> | <span data-ttu-id="535fe-190">未找到请求值“RandomDay”。</span><span class="sxs-lookup"><span data-stu-id="535fe-190">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="535fe-191">**timeZone** 无效</span><span class="sxs-lookup"><span data-stu-id="535fe-191">Invalid **timeZone**</span></span> | <span data-ttu-id="535fe-192">400</span><span class="sxs-lookup"><span data-stu-id="535fe-192">400</span></span> | <span data-ttu-id="535fe-193">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="535fe-193">InvalidTimeZone</span></span> | <span data-ttu-id="535fe-194">提供的时区设置无效。</span><span class="sxs-lookup"><span data-stu-id="535fe-194">Time Zone settings provided are invalid.</span></span>|


## <a name="examples"></a><span data-ttu-id="535fe-195">示例</span><span class="sxs-lookup"><span data-stu-id="535fe-195">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="535fe-196">示例 1</span><span class="sxs-lookup"><span data-stu-id="535fe-196">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="535fe-197">请求</span><span class="sxs-lookup"><span data-stu-id="535fe-197">Request</span></span> 
<span data-ttu-id="535fe-198">第一个示例通过设置 **automaticRepliesSetting** 属性的以下属性来启用对日期范围的自动答复：**status**、**scheduledStartDateTime** 和 **scheduledEndDateTime**。</span><span class="sxs-lookup"><span data-stu-id="535fe-198">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="http"></a>[<span data-ttu-id="535fe-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="535fe-199">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="535fe-200">C#</span><span class="sxs-lookup"><span data-stu-id="535fe-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="535fe-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="535fe-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="535fe-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="535fe-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="535fe-203">Java</span><span class="sxs-lookup"><span data-stu-id="535fe-203">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailboxsettings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="535fe-204">响应</span><span class="sxs-lookup"><span data-stu-id="535fe-204">Response</span></span>
<span data-ttu-id="535fe-205">该响应包括自动答复的更新设置。</span><span class="sxs-lookup"><span data-stu-id="535fe-205">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="535fe-206">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="535fe-206">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2"></a><span data-ttu-id="535fe-207">示例 2</span><span class="sxs-lookup"><span data-stu-id="535fe-207">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="535fe-208">请求</span><span class="sxs-lookup"><span data-stu-id="535fe-208">Request</span></span>
<span data-ttu-id="535fe-209">第二个示例通过将 **timeZone** 属性设置为 [自定义时区](../resources/customtimezone.md)，为登录用户的工作时间自定义时区。</span><span class="sxs-lookup"><span data-stu-id="535fe-209">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>


# <a name="http"></a>[<span data-ttu-id="535fe-210">HTTP</span><span class="sxs-lookup"><span data-stu-id="535fe-210">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="535fe-211">C#</span><span class="sxs-lookup"><span data-stu-id="535fe-211">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="535fe-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="535fe-212">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="535fe-213">Objective-C</span><span class="sxs-lookup"><span data-stu-id="535fe-213">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="535fe-214">Java</span><span class="sxs-lookup"><span data-stu-id="535fe-214">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="535fe-215">响应</span><span class="sxs-lookup"><span data-stu-id="535fe-215">Response</span></span>
<span data-ttu-id="535fe-216">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="535fe-216">Here is an example of the response.</span></span> <span data-ttu-id="535fe-217">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="535fe-217">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
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
