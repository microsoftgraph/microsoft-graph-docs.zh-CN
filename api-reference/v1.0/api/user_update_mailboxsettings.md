# <a name="update-user-mailbox-settings"></a><span data-ttu-id="19a72-101">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="19a72-101">Update user mailbox settings</span></span>

<span data-ttu-id="19a72-p101">更新用户邮箱的一个或多个设置。这包括[自动答复](../resources/automaticrepliessetting.md)（收到发件人的电子邮件时自动通知发件人）、[区域设置](../resources/localeinfo.md)（语言和国家/地区）、时区和[工作时间](../resources/workinghours.md)的设置。</span><span class="sxs-lookup"><span data-stu-id="19a72-p101">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="19a72-104">可以作为 [mailboxSettings](../resources/mailboxsettings.md) 的一部分启用、配置或禁用其中的一个或多个设置。</span><span class="sxs-lookup"><span data-stu-id="19a72-104">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="19a72-105">**注意**：不能创建或删除任何邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="19a72-105">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="19a72-106">更新用户的首选时区时，可以指定 Windows 时区或 [Internet 号码分配局 (IANA) 时区](https://www.iana.org/time-zones)（亦称为“Olson 时区”）。</span><span class="sxs-lookup"><span data-stu-id="19a72-106">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span>

## <a name="permissions"></a><span data-ttu-id="19a72-107">权限</span><span class="sxs-lookup"><span data-stu-id="19a72-107">Permissions</span></span>
<span data-ttu-id="19a72-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="19a72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="19a72-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="19a72-110">Permission type</span></span>      | <span data-ttu-id="19a72-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19a72-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19a72-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19a72-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19a72-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a72-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="19a72-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19a72-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19a72-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a72-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="19a72-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="19a72-116">Application</span></span> | <span data-ttu-id="19a72-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a72-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="19a72-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19a72-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="19a72-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="19a72-119">Optional query parameters</span></span>
<span data-ttu-id="19a72-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="19a72-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="19a72-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="19a72-121">Request headers</span></span>
| <span data-ttu-id="19a72-122">名称</span><span class="sxs-lookup"><span data-stu-id="19a72-122">Name</span></span>       | <span data-ttu-id="19a72-123">类型</span><span class="sxs-lookup"><span data-stu-id="19a72-123">Type</span></span> | <span data-ttu-id="19a72-124">说明</span><span class="sxs-lookup"><span data-stu-id="19a72-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="19a72-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="19a72-125">Authorization</span></span>  | <span data-ttu-id="19a72-126">string</span><span class="sxs-lookup"><span data-stu-id="19a72-126">string</span></span>  | <span data-ttu-id="19a72-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19a72-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19a72-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="19a72-129">Request body</span></span>
<span data-ttu-id="19a72-p104">在请求正文中，提供应更新的相关属性的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。以下是可写/可更新的属性：</span><span class="sxs-lookup"><span data-stu-id="19a72-p104">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="19a72-134">属性</span><span class="sxs-lookup"><span data-stu-id="19a72-134">Property</span></span>     | <span data-ttu-id="19a72-135">类型</span><span class="sxs-lookup"><span data-stu-id="19a72-135">Type</span></span>   |<span data-ttu-id="19a72-136">说明</span><span class="sxs-lookup"><span data-stu-id="19a72-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19a72-137">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="19a72-137">automaticRepliesSetting</span></span>|[<span data-ttu-id="19a72-138">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="19a72-138">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="19a72-139">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="19a72-139">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="19a72-140">还可以设置仅供将来的日期范围内的此类通知。</span><span class="sxs-lookup"><span data-stu-id="19a72-140">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="19a72-141">语言</span><span class="sxs-lookup"><span data-stu-id="19a72-141">language</span></span>|[<span data-ttu-id="19a72-142">localeInfo</span><span class="sxs-lookup"><span data-stu-id="19a72-142">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="19a72-143">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="19a72-143">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="19a72-144">timeZone</span><span class="sxs-lookup"><span data-stu-id="19a72-144">timeZone</span></span>|<span data-ttu-id="19a72-145">string</span><span class="sxs-lookup"><span data-stu-id="19a72-145">string</span></span>|<span data-ttu-id="19a72-146">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="19a72-146">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="19a72-147">workingHours</span><span class="sxs-lookup"><span data-stu-id="19a72-147">workingHours</span></span>|[<span data-ttu-id="19a72-148">workingHours</span><span class="sxs-lookup"><span data-stu-id="19a72-148">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="19a72-149">用户工作的小时数、一周的天数和时区。</span><span class="sxs-lookup"><span data-stu-id="19a72-149">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="19a72-150">响应</span><span class="sxs-lookup"><span data-stu-id="19a72-150">Response</span></span>

<span data-ttu-id="19a72-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailboxSettings](../resources/mailboxSettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19a72-151">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxSettings.md) object in the response body.</span></span>


## <a name="errors"></a><span data-ttu-id="19a72-152">错误</span><span class="sxs-lookup"><span data-stu-id="19a72-152">Errors</span></span>

<span data-ttu-id="19a72-153">将工作时间设置为不适当的值可能会返回以下错误。</span><span class="sxs-lookup"><span data-stu-id="19a72-153">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="19a72-154">应用场景</span><span class="sxs-lookup"><span data-stu-id="19a72-154">Scenario</span></span>   | <span data-ttu-id="19a72-155">HTTP 状态代码</span><span class="sxs-lookup"><span data-stu-id="19a72-155">HTTP status code</span></span> | <span data-ttu-id="19a72-156">错误代码</span><span class="sxs-lookup"><span data-stu-id="19a72-156">Error code</span></span> | <span data-ttu-id="19a72-157">错误消息</span><span class="sxs-lookup"><span data-stu-id="19a72-157">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="19a72-158">**startTime** 或 **endTime** 无效</span><span class="sxs-lookup"><span data-stu-id="19a72-158">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="19a72-159">400</span><span class="sxs-lookup"><span data-stu-id="19a72-159">400</span></span> | <span data-ttu-id="19a72-160">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="19a72-160">RequestBodyRead</span></span> | <span data-ttu-id="19a72-161">无法将文本“08”转换为预期类型“Edm.TimeOfDay”。</span><span class="sxs-lookup"><span data-stu-id="19a72-161">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="19a72-162">开始时间大于结束时间</span><span class="sxs-lookup"><span data-stu-id="19a72-162">Start time is greater than end time</span></span> | <span data-ttu-id="19a72-163">400</span><span class="sxs-lookup"><span data-stu-id="19a72-163">400</span></span> | <span data-ttu-id="19a72-164">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="19a72-164">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="19a72-165">开始时间应早于结束时间。</span><span class="sxs-lookup"><span data-stu-id="19a72-165">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="19a72-166">**daysOfWeek** 中的天数无效</span><span class="sxs-lookup"><span data-stu-id="19a72-166">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="19a72-167">400</span><span class="sxs-lookup"><span data-stu-id="19a72-167">400</span></span> | <span data-ttu-id="19a72-168">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="19a72-168">InvalidArguments</span></span> | <span data-ttu-id="19a72-169">未找到请求值“RandomDay”。</span><span class="sxs-lookup"><span data-stu-id="19a72-169">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="19a72-170">**timeZone** 无效</span><span class="sxs-lookup"><span data-stu-id="19a72-170">Invalid **timeZone**</span></span> | <span data-ttu-id="19a72-171">400</span><span class="sxs-lookup"><span data-stu-id="19a72-171">400</span></span> | <span data-ttu-id="19a72-172">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="19a72-172">InvalidTimeZone</span></span> | <span data-ttu-id="19a72-173">提供的时区设置无效。</span><span class="sxs-lookup"><span data-stu-id="19a72-173">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="19a72-174">示例</span><span class="sxs-lookup"><span data-stu-id="19a72-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19a72-175">请求</span><span class="sxs-lookup"><span data-stu-id="19a72-175">Request</span></span>
<span data-ttu-id="19a72-176">第一个示例通过设置 **automaticRepliesSetting** 属性的以下属性来启用对日期范围的自动答复：**status**、**scheduledStartDateTime** 和 **scheduledEndDateTime**。</span><span class="sxs-lookup"><span data-stu-id="19a72-176">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings"
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
##### <a name="response"></a><span data-ttu-id="19a72-177">响应</span><span class="sxs-lookup"><span data-stu-id="19a72-177">Response</span></span>
<span data-ttu-id="19a72-178">该响应包括自动答复的更新设置。</span><span class="sxs-lookup"><span data-stu-id="19a72-178">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="19a72-179">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="19a72-179">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="19a72-180">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19a72-180">All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="19a72-181">请求 2</span><span class="sxs-lookup"><span data-stu-id="19a72-181">Request 2</span></span>
<span data-ttu-id="19a72-182">第二个示例通过将 **timeZone** 属性设置为[自定义时区](../resources/customtimezone.md)，为登录用户的工作时间自定义时区。</span><span class="sxs-lookup"><span data-stu-id="19a72-182">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

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
##### <a name="response-2"></a><span data-ttu-id="19a72-183">响应 2</span><span class="sxs-lookup"><span data-stu-id="19a72-183">Response 2</span></span>
<span data-ttu-id="19a72-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19a72-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->