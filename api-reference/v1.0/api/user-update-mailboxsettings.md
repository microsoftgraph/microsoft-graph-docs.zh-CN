---
title: 获取用户的邮箱设置
description: 更新用户邮箱的一个或多个设置。这包括自动答复（收到发件人的电子邮件时自动通知发件人）、区域设置（语言和国家/地区）、时区和工作时间的设置。
localization_priority: Normal
ms.openlocfilehash: cfc19337ed96a3cfefcfe5778807bc81e4c72fc7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840641"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="98110-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="98110-104">Update user mailbox settings</span></span>

<span data-ttu-id="98110-p102">更新用户邮箱的一个或多个设置。这包括[自动答复](../resources/automaticrepliessetting.md)（收到发件人的电子邮件时自动通知发件人）、[区域设置](../resources/localeinfo.md)（语言和国家/地区）、时区和[工作时间](../resources/workinghours.md)的设置。</span><span class="sxs-lookup"><span data-stu-id="98110-p102">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="98110-107">可以作为 [mailboxSettings](../resources/mailboxsettings.md) 的一部分启用、配置或禁用其中的一个或多个设置。</span><span class="sxs-lookup"><span data-stu-id="98110-107">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="98110-108">**注意**：不能创建或删除任何邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="98110-108">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="98110-109">更新用户的首选时区时，可以指定 Windows 时区或 [Internet 号码分配局 (IANA) 时区](https://www.iana.org/time-zones)（亦称为“Olson 时区”）。</span><span class="sxs-lookup"><span data-stu-id="98110-109">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span>

## <a name="permissions"></a><span data-ttu-id="98110-110">权限</span><span class="sxs-lookup"><span data-stu-id="98110-110">Permissions</span></span>
<span data-ttu-id="98110-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98110-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98110-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="98110-113">Permission type</span></span>      | <span data-ttu-id="98110-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98110-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98110-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98110-115">Delegated (work or school account)</span></span> | <span data-ttu-id="98110-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98110-116">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="98110-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98110-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98110-118">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98110-118">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="98110-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="98110-119">Application</span></span> | <span data-ttu-id="98110-120">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98110-120">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="98110-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98110-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="98110-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="98110-122">Optional query parameters</span></span>
<span data-ttu-id="98110-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="98110-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="98110-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="98110-124">Request headers</span></span>
| <span data-ttu-id="98110-125">名称</span><span class="sxs-lookup"><span data-stu-id="98110-125">Name</span></span>       | <span data-ttu-id="98110-126">类型</span><span class="sxs-lookup"><span data-stu-id="98110-126">Type</span></span> | <span data-ttu-id="98110-127">说明</span><span class="sxs-lookup"><span data-stu-id="98110-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="98110-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="98110-128">Authorization</span></span>  | <span data-ttu-id="98110-129">string</span><span class="sxs-lookup"><span data-stu-id="98110-129">string</span></span>  | <span data-ttu-id="98110-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98110-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98110-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="98110-132">Request body</span></span>
<span data-ttu-id="98110-p105">在请求正文中，提供应更新的相关属性的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。以下是可写/可更新的属性：</span><span class="sxs-lookup"><span data-stu-id="98110-p105">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="98110-137">属性</span><span class="sxs-lookup"><span data-stu-id="98110-137">Property</span></span>     | <span data-ttu-id="98110-138">类型</span><span class="sxs-lookup"><span data-stu-id="98110-138">Type</span></span>   |<span data-ttu-id="98110-139">说明</span><span class="sxs-lookup"><span data-stu-id="98110-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98110-140">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="98110-140">automaticRepliesSetting</span></span>|[<span data-ttu-id="98110-141">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="98110-141">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="98110-142">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="98110-142">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="98110-143">还可以设置仅供将来的日期范围内的此类通知。</span><span class="sxs-lookup"><span data-stu-id="98110-143">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="98110-144">语言</span><span class="sxs-lookup"><span data-stu-id="98110-144">language</span></span>|[<span data-ttu-id="98110-145">localeInfo</span><span class="sxs-lookup"><span data-stu-id="98110-145">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="98110-146">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="98110-146">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="98110-147">timeZone</span><span class="sxs-lookup"><span data-stu-id="98110-147">timeZone</span></span>|<span data-ttu-id="98110-148">string</span><span class="sxs-lookup"><span data-stu-id="98110-148">string</span></span>|<span data-ttu-id="98110-149">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="98110-149">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="98110-150">workingHours</span><span class="sxs-lookup"><span data-stu-id="98110-150">workingHours</span></span>|[<span data-ttu-id="98110-151">workingHours</span><span class="sxs-lookup"><span data-stu-id="98110-151">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="98110-152">用户工作的小时数、一周的天数和时区。</span><span class="sxs-lookup"><span data-stu-id="98110-152">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="98110-153">响应</span><span class="sxs-lookup"><span data-stu-id="98110-153">Response</span></span>

<span data-ttu-id="98110-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailboxSettings](../resources/mailboxsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98110-154">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>


## <a name="errors"></a><span data-ttu-id="98110-155">错误</span><span class="sxs-lookup"><span data-stu-id="98110-155">Errors</span></span>

<span data-ttu-id="98110-156">将工作时间设置为不适当的值可能会返回以下错误。</span><span class="sxs-lookup"><span data-stu-id="98110-156">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="98110-157">应用场景</span><span class="sxs-lookup"><span data-stu-id="98110-157">Scenario</span></span>   | <span data-ttu-id="98110-158">HTTP 状态代码</span><span class="sxs-lookup"><span data-stu-id="98110-158">HTTP status code</span></span> | <span data-ttu-id="98110-159">错误代码</span><span class="sxs-lookup"><span data-stu-id="98110-159">Error code</span></span> | <span data-ttu-id="98110-160">错误消息</span><span class="sxs-lookup"><span data-stu-id="98110-160">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="98110-161">**startTime** 或 **endTime** 无效</span><span class="sxs-lookup"><span data-stu-id="98110-161">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="98110-162">400</span><span class="sxs-lookup"><span data-stu-id="98110-162">400</span></span> | <span data-ttu-id="98110-163">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="98110-163">RequestBodyRead</span></span> | <span data-ttu-id="98110-164">无法将文本“08”转换为预期类型“Edm.TimeOfDay”。</span><span class="sxs-lookup"><span data-stu-id="98110-164">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="98110-165">开始时间大于结束时间</span><span class="sxs-lookup"><span data-stu-id="98110-165">Start time is greater than end time</span></span> | <span data-ttu-id="98110-166">400</span><span class="sxs-lookup"><span data-stu-id="98110-166">400</span></span> | <span data-ttu-id="98110-167">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="98110-167">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="98110-168">开始时间应早于结束时间。</span><span class="sxs-lookup"><span data-stu-id="98110-168">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="98110-169">**daysOfWeek** 中的天数无效</span><span class="sxs-lookup"><span data-stu-id="98110-169">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="98110-170">400</span><span class="sxs-lookup"><span data-stu-id="98110-170">400</span></span> | <span data-ttu-id="98110-171">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="98110-171">InvalidArguments</span></span> | <span data-ttu-id="98110-172">未找到请求值“RandomDay”。</span><span class="sxs-lookup"><span data-stu-id="98110-172">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="98110-173">**timeZone** 无效</span><span class="sxs-lookup"><span data-stu-id="98110-173">Invalid **timeZone**</span></span> | <span data-ttu-id="98110-174">400</span><span class="sxs-lookup"><span data-stu-id="98110-174">400</span></span> | <span data-ttu-id="98110-175">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="98110-175">InvalidTimeZone</span></span> | <span data-ttu-id="98110-176">提供的时区设置无效。</span><span class="sxs-lookup"><span data-stu-id="98110-176">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="98110-177">示例</span><span class="sxs-lookup"><span data-stu-id="98110-177">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98110-178">请求</span><span class="sxs-lookup"><span data-stu-id="98110-178">Request</span></span>
<span data-ttu-id="98110-179">第一个示例通过设置 **automaticRepliesSetting** 属性的以下属性来启用对日期范围的自动答复：**status**、**scheduledStartDateTime** 和 **scheduledEndDateTime**。</span><span class="sxs-lookup"><span data-stu-id="98110-179">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

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
##### <a name="response"></a><span data-ttu-id="98110-180">响应</span><span class="sxs-lookup"><span data-stu-id="98110-180">Response</span></span>
<span data-ttu-id="98110-181">该响应包括自动答复的更新设置。</span><span class="sxs-lookup"><span data-stu-id="98110-181">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="98110-182">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="98110-182">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="98110-183">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="98110-183">All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="98110-184">请求 2</span><span class="sxs-lookup"><span data-stu-id="98110-184">Request 2</span></span>
<span data-ttu-id="98110-185">第二个示例通过将 **timeZone** 属性设置为[自定义时区](../resources/customtimezone.md)，为登录用户的工作时间自定义时区。</span><span class="sxs-lookup"><span data-stu-id="98110-185">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

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
##### <a name="response-2"></a><span data-ttu-id="98110-186">响应 2</span><span class="sxs-lookup"><span data-stu-id="98110-186">Response 2</span></span>
<span data-ttu-id="98110-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="98110-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
