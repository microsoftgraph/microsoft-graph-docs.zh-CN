---
title: 获取用户的邮箱设置
description: 更新用户邮箱的一个或多个设置。这包括自动答复（收到发件人的电子邮件时自动通知发件人）、区域设置（语言和国家/地区）、时区和工作时间的设置。
ms.openlocfilehash: fb4e3f49c014b9bebee3076db49594eb1aee0fa8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045980"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="718d9-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="718d9-104">Update user mailbox settings</span></span>

> <span data-ttu-id="718d9-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="718d9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="718d9-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="718d9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="718d9-p103">更新用户邮箱的一个或多个设置。这包括[自动答复](../resources/automaticrepliessetting.md)（收到发件人的电子邮件时自动通知发件人）、[区域设置](../resources/localeinfo.md)（语言和国家/地区）、时区和[工作时间](../resources/workinghours.md)的设置。</span><span class="sxs-lookup"><span data-stu-id="718d9-p103">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="718d9-109">可以作为 [mailboxSettings](../resources/mailboxsettings.md) 的一部分启用、配置或禁用其中的一个或多个设置。</span><span class="sxs-lookup"><span data-stu-id="718d9-109">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="718d9-110">**注意**：不能创建或删除任何邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="718d9-110">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="718d9-111">更新用户的首选时区时，可以指定 Windows 时区或 [Internet 号码分配局 (IANA) 时区](https://www.iana.org/time-zones)（亦称为“Olson 时区”）。</span><span class="sxs-lookup"><span data-stu-id="718d9-111">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="718d9-112">下面的[示例 2](#request-2)中所示，您便可以进一步自定义时区。</span><span class="sxs-lookup"><span data-stu-id="718d9-112">You can also further customize the time zone as shown in [example 2](#request-2) below.</span></span>

## <a name="permissions"></a><span data-ttu-id="718d9-113">权限</span><span class="sxs-lookup"><span data-stu-id="718d9-113">Permissions</span></span>
<span data-ttu-id="718d9-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="718d9-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="718d9-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="718d9-116">Permission type</span></span>      | <span data-ttu-id="718d9-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="718d9-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="718d9-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="718d9-118">Delegated (work or school account)</span></span> | <span data-ttu-id="718d9-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="718d9-119">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="718d9-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="718d9-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="718d9-121">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="718d9-121">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="718d9-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="718d9-122">Application</span></span> | <span data-ttu-id="718d9-123">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="718d9-123">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="718d9-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="718d9-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="718d9-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="718d9-125">Optional query parameters</span></span>
<span data-ttu-id="718d9-126">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="718d9-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="718d9-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="718d9-127">Request headers</span></span>
| <span data-ttu-id="718d9-128">名称</span><span class="sxs-lookup"><span data-stu-id="718d9-128">Name</span></span>       | <span data-ttu-id="718d9-129">类型</span><span class="sxs-lookup"><span data-stu-id="718d9-129">Type</span></span> | <span data-ttu-id="718d9-130">说明</span><span class="sxs-lookup"><span data-stu-id="718d9-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="718d9-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="718d9-131">Authorization</span></span>  | <span data-ttu-id="718d9-132">string</span><span class="sxs-lookup"><span data-stu-id="718d9-132">string</span></span>  | <span data-ttu-id="718d9-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="718d9-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="718d9-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="718d9-135">Request body</span></span>
<span data-ttu-id="718d9-p107">在请求正文中，提供应更新的相关属性的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。以下是可写/可更新的属性：</span><span class="sxs-lookup"><span data-stu-id="718d9-p107">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="718d9-140">属性</span><span class="sxs-lookup"><span data-stu-id="718d9-140">Property</span></span>     | <span data-ttu-id="718d9-141">类型</span><span class="sxs-lookup"><span data-stu-id="718d9-141">Type</span></span>   |<span data-ttu-id="718d9-142">说明</span><span class="sxs-lookup"><span data-stu-id="718d9-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="718d9-143">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="718d9-143">automaticRepliesSetting</span></span>|[<span data-ttu-id="718d9-144">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="718d9-144">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="718d9-145">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="718d9-145">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="718d9-146">还可以设置仅供将来的日期范围内的此类通知。</span><span class="sxs-lookup"><span data-stu-id="718d9-146">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="718d9-147">语言</span><span class="sxs-lookup"><span data-stu-id="718d9-147">language</span></span>|[<span data-ttu-id="718d9-148">localeInfo</span><span class="sxs-lookup"><span data-stu-id="718d9-148">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="718d9-149">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="718d9-149">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="718d9-150">timeZone</span><span class="sxs-lookup"><span data-stu-id="718d9-150">timeZone</span></span>|<span data-ttu-id="718d9-151">string</span><span class="sxs-lookup"><span data-stu-id="718d9-151">string</span></span>|<span data-ttu-id="718d9-152">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="718d9-152">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="718d9-153">workingHours</span><span class="sxs-lookup"><span data-stu-id="718d9-153">workingHours</span></span>|[<span data-ttu-id="718d9-154">workingHours</span><span class="sxs-lookup"><span data-stu-id="718d9-154">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="718d9-155">用户工作的小时数、一周的天数和时区。</span><span class="sxs-lookup"><span data-stu-id="718d9-155">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="718d9-156">响应</span><span class="sxs-lookup"><span data-stu-id="718d9-156">Response</span></span>

<span data-ttu-id="718d9-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailboxSettings](../resources/mailboxsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="718d9-157">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="718d9-158">错误</span><span class="sxs-lookup"><span data-stu-id="718d9-158">Errors</span></span>

<span data-ttu-id="718d9-159">将工作时间设置为不适当的值可能会返回以下错误。</span><span class="sxs-lookup"><span data-stu-id="718d9-159">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="718d9-160">应用场景</span><span class="sxs-lookup"><span data-stu-id="718d9-160">Scenario</span></span>   | <span data-ttu-id="718d9-161">HTTP 状态代码</span><span class="sxs-lookup"><span data-stu-id="718d9-161">HTTP status code</span></span> | <span data-ttu-id="718d9-162">错误代码</span><span class="sxs-lookup"><span data-stu-id="718d9-162">Error code</span></span> | <span data-ttu-id="718d9-163">错误消息</span><span class="sxs-lookup"><span data-stu-id="718d9-163">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="718d9-164">**startTime** 或 **endTime** 无效</span><span class="sxs-lookup"><span data-stu-id="718d9-164">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="718d9-165">400</span><span class="sxs-lookup"><span data-stu-id="718d9-165">400</span></span> | <span data-ttu-id="718d9-166">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="718d9-166">RequestBodyRead</span></span> | <span data-ttu-id="718d9-167">无法将文本“08”转换为预期类型“Edm.TimeOfDay”。</span><span class="sxs-lookup"><span data-stu-id="718d9-167">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="718d9-168">开始时间大于结束时间</span><span class="sxs-lookup"><span data-stu-id="718d9-168">Start time is greater than end time</span></span> | <span data-ttu-id="718d9-169">400</span><span class="sxs-lookup"><span data-stu-id="718d9-169">400</span></span> | <span data-ttu-id="718d9-170">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="718d9-170">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="718d9-171">开始时间应早于结束时间。</span><span class="sxs-lookup"><span data-stu-id="718d9-171">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="718d9-172">**daysOfWeek** 中的天数无效</span><span class="sxs-lookup"><span data-stu-id="718d9-172">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="718d9-173">400</span><span class="sxs-lookup"><span data-stu-id="718d9-173">400</span></span> | <span data-ttu-id="718d9-174">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="718d9-174">InvalidArguments</span></span> | <span data-ttu-id="718d9-175">未找到请求值“RandomDay”。</span><span class="sxs-lookup"><span data-stu-id="718d9-175">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="718d9-176">**timeZone** 无效</span><span class="sxs-lookup"><span data-stu-id="718d9-176">Invalid **timeZone**</span></span> | <span data-ttu-id="718d9-177">400</span><span class="sxs-lookup"><span data-stu-id="718d9-177">400</span></span> | <span data-ttu-id="718d9-178">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="718d9-178">InvalidTimeZone</span></span> | <span data-ttu-id="718d9-179">提供的时区设置无效。</span><span class="sxs-lookup"><span data-stu-id="718d9-179">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="718d9-180">示例</span><span class="sxs-lookup"><span data-stu-id="718d9-180">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="718d9-181">请求 1</span><span class="sxs-lookup"><span data-stu-id="718d9-181">Request 1</span></span>
<span data-ttu-id="718d9-182">第一个示例通过设置 **automaticRepliesSetting** 属性的以下属性来启用对日期范围的自动答复：**status**、**scheduledStartDateTime** 和 **scheduledEndDateTime**。</span><span class="sxs-lookup"><span data-stu-id="718d9-182">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

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
##### <a name="response-1"></a><span data-ttu-id="718d9-183">响应 1</span><span class="sxs-lookup"><span data-stu-id="718d9-183">Response 1</span></span>
<span data-ttu-id="718d9-184">该响应包括自动答复的更新设置。</span><span class="sxs-lookup"><span data-stu-id="718d9-184">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="718d9-185">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="718d9-185">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="718d9-186">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="718d9-186">All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="718d9-187">请求 2</span><span class="sxs-lookup"><span data-stu-id="718d9-187">Request 2</span></span>
<span data-ttu-id="718d9-188">第二个示例通过将 **timeZone** 属性设置为[自定义时区](../resources/customtimezone.md)，为登录用户的工作时间自定义时区。</span><span class="sxs-lookup"><span data-stu-id="718d9-188">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

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
##### <a name="response-2"></a><span data-ttu-id="718d9-189">响应 2</span><span class="sxs-lookup"><span data-stu-id="718d9-189">Response 2</span></span>
<span data-ttu-id="718d9-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="718d9-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->