---
title: 获取用户的邮箱设置
description: 更新用户邮箱的一个或多个设置。 这包括自动答复的设置（在收到电子邮件时自动通知人员）、区域设置（语言和国家/地区）、时区和工作时间。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0a224df7acdc0396d13743433d2cb407eb500d06
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402828"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="e97bb-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="e97bb-104">Update user mailbox settings</span></span>

<span data-ttu-id="e97bb-105">启用、配置或禁用以下一个或多个设置作为用户的[mailboxSettings](../resources/mailboxsettings.md)的一部分：</span><span class="sxs-lookup"><span data-stu-id="e97bb-105">Enable, configure, or disable one or more of the following settings as part of a user's [mailboxSettings](../resources/mailboxsettings.md):</span></span>

- <span data-ttu-id="e97bb-106">[自动答复](../resources/automaticrepliessetting.md)（收到电子邮件后自动通知人员）</span><span class="sxs-lookup"><span data-stu-id="e97bb-106">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="e97bb-107">dateFormat</span><span class="sxs-lookup"><span data-stu-id="e97bb-107">dateFormat</span></span>
- <span data-ttu-id="e97bb-108">[区域设置](../resources/localeinfo.md)（语言和国家/地区）</span><span class="sxs-lookup"><span data-stu-id="e97bb-108">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="e97bb-109">timeFormat</span><span class="sxs-lookup"><span data-stu-id="e97bb-109">timeFormat</span></span>
- <span data-ttu-id="e97bb-110">时区</span><span class="sxs-lookup"><span data-stu-id="e97bb-110">time zone</span></span>
- [<span data-ttu-id="e97bb-111">working hours － 工作时间</span><span class="sxs-lookup"><span data-stu-id="e97bb-111">working hours</span></span>](../resources/workinghours.md)

<span data-ttu-id="e97bb-112">更新用户的首选日期或时间格式时，请分别指定[短日期](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate)或[短时间](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime)格式。</span><span class="sxs-lookup"><span data-stu-id="e97bb-112">When updating the preferred date or time format for a user, specify it in respectively, the [short date](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) format.</span></span> 

<span data-ttu-id="e97bb-113">更新用户的首选时区时，在 Windows 或[Internet 分配的号码颁发机构（IANA）](https://www.iana.org/time-zones)的时区（也称为 "Olson 时区"）格式中指定它。</span><span class="sxs-lookup"><span data-stu-id="e97bb-113">When updating the preferred time zone for a user, specify it in the Windows or [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="e97bb-114">您还可以进一步自定义时区，如下面的[示例 2](#example-2)所示。</span><span class="sxs-lookup"><span data-stu-id="e97bb-114">You can also further customize the time zone as shown in [example 2](#example-2) below.</span></span>

> [!TIP] 
> <span data-ttu-id="e97bb-115">您不能创建或删除任何邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="e97bb-115">You cannot create or delete any mailbox settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="e97bb-116">权限</span><span class="sxs-lookup"><span data-stu-id="e97bb-116">Permissions</span></span>
<span data-ttu-id="e97bb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e97bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e97bb-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="e97bb-119">Permission type</span></span>      | <span data-ttu-id="e97bb-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e97bb-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e97bb-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e97bb-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e97bb-122">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e97bb-122">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e97bb-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e97bb-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e97bb-124">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e97bb-124">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e97bb-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="e97bb-125">Application</span></span> | <span data-ttu-id="e97bb-126">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e97bb-126">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e97bb-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e97bb-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e97bb-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e97bb-128">Optional query parameters</span></span>
<span data-ttu-id="e97bb-129">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e97bb-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e97bb-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="e97bb-130">Request headers</span></span>
| <span data-ttu-id="e97bb-131">名称</span><span class="sxs-lookup"><span data-stu-id="e97bb-131">Name</span></span>       | <span data-ttu-id="e97bb-132">类型</span><span class="sxs-lookup"><span data-stu-id="e97bb-132">Type</span></span> | <span data-ttu-id="e97bb-133">说明</span><span class="sxs-lookup"><span data-stu-id="e97bb-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e97bb-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="e97bb-134">Authorization</span></span>  | <span data-ttu-id="e97bb-135">string</span><span class="sxs-lookup"><span data-stu-id="e97bb-135">string</span></span>  | <span data-ttu-id="e97bb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e97bb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e97bb-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="e97bb-138">Request body</span></span>
<span data-ttu-id="e97bb-p105">在请求正文中，提供应更新的相关属性的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。以下是可写/可更新的属性：</span><span class="sxs-lookup"><span data-stu-id="e97bb-p105">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="e97bb-143">属性</span><span class="sxs-lookup"><span data-stu-id="e97bb-143">Property</span></span>     | <span data-ttu-id="e97bb-144">类型</span><span class="sxs-lookup"><span data-stu-id="e97bb-144">Type</span></span>   |<span data-ttu-id="e97bb-145">说明</span><span class="sxs-lookup"><span data-stu-id="e97bb-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e97bb-146">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="e97bb-146">automaticRepliesSetting</span></span>|[<span data-ttu-id="e97bb-147">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="e97bb-147">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="e97bb-148">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="e97bb-148">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="e97bb-149">只能将此类通知设置为将来日期范围。</span><span class="sxs-lookup"><span data-stu-id="e97bb-149">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="e97bb-150">dateFormat</span><span class="sxs-lookup"><span data-stu-id="e97bb-150">dateFormat</span></span>|<span data-ttu-id="e97bb-151">string</span><span class="sxs-lookup"><span data-stu-id="e97bb-151">string</span></span>|<span data-ttu-id="e97bb-152">用户邮箱的日期格式。</span><span class="sxs-lookup"><span data-stu-id="e97bb-152">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="e97bb-153">语言</span><span class="sxs-lookup"><span data-stu-id="e97bb-153">language</span></span>|[<span data-ttu-id="e97bb-154">localeInfo</span><span class="sxs-lookup"><span data-stu-id="e97bb-154">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="e97bb-155">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="e97bb-155">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="e97bb-156">timeFormat</span><span class="sxs-lookup"><span data-stu-id="e97bb-156">timeFormat</span></span>|<span data-ttu-id="e97bb-157">string</span><span class="sxs-lookup"><span data-stu-id="e97bb-157">string</span></span>|<span data-ttu-id="e97bb-158">用户邮箱的时间格式。</span><span class="sxs-lookup"><span data-stu-id="e97bb-158">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="e97bb-159">timeZone</span><span class="sxs-lookup"><span data-stu-id="e97bb-159">timeZone</span></span>|<span data-ttu-id="e97bb-160">string</span><span class="sxs-lookup"><span data-stu-id="e97bb-160">string</span></span>|<span data-ttu-id="e97bb-161">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="e97bb-161">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="e97bb-162">workingHours</span><span class="sxs-lookup"><span data-stu-id="e97bb-162">workingHours</span></span>|[<span data-ttu-id="e97bb-163">workingHours</span><span class="sxs-lookup"><span data-stu-id="e97bb-163">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="e97bb-164">用户工作的小时数、一周的天数和时区。</span><span class="sxs-lookup"><span data-stu-id="e97bb-164">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="e97bb-165">响应</span><span class="sxs-lookup"><span data-stu-id="e97bb-165">Response</span></span>

<span data-ttu-id="e97bb-166">如果成功，此方法在响应`200 OK`正文中返回响应代码和[mailboxSettings](../resources/mailboxsettings.md)对象的更新的属性。</span><span class="sxs-lookup"><span data-stu-id="e97bb-166">If successful, this method returns a `200 OK` response code and the updated properties of a [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="e97bb-167">错误</span><span class="sxs-lookup"><span data-stu-id="e97bb-167">Errors</span></span>

<span data-ttu-id="e97bb-168">将工作时间设置为不适当的值可能会返回以下错误。</span><span class="sxs-lookup"><span data-stu-id="e97bb-168">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="e97bb-169">应用场景</span><span class="sxs-lookup"><span data-stu-id="e97bb-169">Scenario</span></span>   | <span data-ttu-id="e97bb-170">HTTP 状态代码</span><span class="sxs-lookup"><span data-stu-id="e97bb-170">HTTP status code</span></span> | <span data-ttu-id="e97bb-171">错误代码</span><span class="sxs-lookup"><span data-stu-id="e97bb-171">Error code</span></span> | <span data-ttu-id="e97bb-172">错误消息</span><span class="sxs-lookup"><span data-stu-id="e97bb-172">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="e97bb-173">**startTime** 或 **endTime** 无效</span><span class="sxs-lookup"><span data-stu-id="e97bb-173">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="e97bb-174">400</span><span class="sxs-lookup"><span data-stu-id="e97bb-174">400</span></span> | <span data-ttu-id="e97bb-175">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="e97bb-175">RequestBodyRead</span></span> | <span data-ttu-id="e97bb-176">无法将文本“08”转换为预期类型“Edm.TimeOfDay”。</span><span class="sxs-lookup"><span data-stu-id="e97bb-176">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="e97bb-177">开始时间大于结束时间</span><span class="sxs-lookup"><span data-stu-id="e97bb-177">Start time is greater than end time</span></span> | <span data-ttu-id="e97bb-178">400</span><span class="sxs-lookup"><span data-stu-id="e97bb-178">400</span></span> | <span data-ttu-id="e97bb-179">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="e97bb-179">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="e97bb-180">开始时间应早于结束时间。</span><span class="sxs-lookup"><span data-stu-id="e97bb-180">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="e97bb-181">**daysOfWeek** 中的天数无效</span><span class="sxs-lookup"><span data-stu-id="e97bb-181">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="e97bb-182">400</span><span class="sxs-lookup"><span data-stu-id="e97bb-182">400</span></span> | <span data-ttu-id="e97bb-183">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="e97bb-183">InvalidArguments</span></span> | <span data-ttu-id="e97bb-184">未找到请求值“RandomDay”。</span><span class="sxs-lookup"><span data-stu-id="e97bb-184">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="e97bb-185">**timeZone** 无效</span><span class="sxs-lookup"><span data-stu-id="e97bb-185">Invalid **timeZone**</span></span> | <span data-ttu-id="e97bb-186">400</span><span class="sxs-lookup"><span data-stu-id="e97bb-186">400</span></span> | <span data-ttu-id="e97bb-187">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="e97bb-187">InvalidTimeZone</span></span> | <span data-ttu-id="e97bb-188">提供的时区设置无效。</span><span class="sxs-lookup"><span data-stu-id="e97bb-188">Time Zone settings provided are invalid.</span></span>|


## <a name="examples"></a><span data-ttu-id="e97bb-189">示例</span><span class="sxs-lookup"><span data-stu-id="e97bb-189">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="e97bb-190">示例 1</span><span class="sxs-lookup"><span data-stu-id="e97bb-190">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="e97bb-191">请求</span><span class="sxs-lookup"><span data-stu-id="e97bb-191">Request</span></span> 
<span data-ttu-id="e97bb-192">第一个示例通过设置 **automaticRepliesSetting** 属性的以下属性来启用对日期范围的自动答复：**status**、**scheduledStartDateTime** 和 **scheduledEndDateTime**。</span><span class="sxs-lookup"><span data-stu-id="e97bb-192">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e97bb-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="e97bb-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings_1"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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

#### <a name="response"></a><span data-ttu-id="e97bb-194">响应</span><span class="sxs-lookup"><span data-stu-id="e97bb-194">Response</span></span>
<span data-ttu-id="e97bb-195">该响应包括自动答复的更新设置。</span><span class="sxs-lookup"><span data-stu-id="e97bb-195">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="e97bb-196">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e97bb-196">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e97bb-197">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e97bb-197">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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

### <a name="example-2"></a><span data-ttu-id="e97bb-198">示例 2</span><span class="sxs-lookup"><span data-stu-id="e97bb-198">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="e97bb-199">请求</span><span class="sxs-lookup"><span data-stu-id="e97bb-199">Request</span></span>
<span data-ttu-id="e97bb-200">第二个示例通过将 **timeZone** 属性设置为[自定义时区](../resources/customtimezone.md)，为登录用户的工作时间自定义时区。</span><span class="sxs-lookup"><span data-stu-id="e97bb-200">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
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
#### <a name="response"></a><span data-ttu-id="e97bb-201">响应</span><span class="sxs-lookup"><span data-stu-id="e97bb-201">Response</span></span>
<span data-ttu-id="e97bb-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e97bb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
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
<!-- {
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
