---
title: 获取用户的邮箱设置
description: 更新用户邮箱的一个或多个设置。 这包括自动答复的设置 (在收到电子邮件时自动通知人员)、区域设置 (语言和国家/地区)、时区和工作时间。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c93f4479652b2a2120e49cd83b35bbfb51c069fb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457637"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="99027-104">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="99027-104">Update user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99027-p102">更新用户邮箱的一个或多个设置。这包括[自动答复](../resources/automaticrepliessetting.md)（收到发件人的电子邮件时自动通知发件人）、[区域设置](../resources/localeinfo.md)（语言和国家/地区）、时区和[工作时间](../resources/workinghours.md)的设置。</span><span class="sxs-lookup"><span data-stu-id="99027-p102">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="99027-107">可以作为 [mailboxSettings](../resources/mailboxsettings.md) 的一部分启用、配置或禁用其中的一个或多个设置。</span><span class="sxs-lookup"><span data-stu-id="99027-107">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="99027-108">**注意**：不能创建或删除任何邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="99027-108">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="99027-109">更新用户的首选时区时，可以指定 Windows 时区或 [Internet 号码分配局 (IANA) 时区](https://www.iana.org/time-zones)（亦称为“Olson 时区”）。</span><span class="sxs-lookup"><span data-stu-id="99027-109">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="99027-110">您还可以进一步自定义时区, 如下面的[示例 2](#request-2)所示。</span><span class="sxs-lookup"><span data-stu-id="99027-110">You can also further customize the time zone as shown in [example 2](#request-2) below.</span></span>

## <a name="permissions"></a><span data-ttu-id="99027-111">权限</span><span class="sxs-lookup"><span data-stu-id="99027-111">Permissions</span></span>
<span data-ttu-id="99027-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99027-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99027-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="99027-114">Permission type</span></span>      | <span data-ttu-id="99027-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99027-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99027-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99027-116">Delegated (work or school account)</span></span> | <span data-ttu-id="99027-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99027-117">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="99027-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99027-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99027-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99027-119">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="99027-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="99027-120">Application</span></span> | <span data-ttu-id="99027-121">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99027-121">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="99027-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99027-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="99027-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="99027-123">Optional query parameters</span></span>
<span data-ttu-id="99027-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="99027-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="99027-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="99027-125">Request headers</span></span>
| <span data-ttu-id="99027-126">名称</span><span class="sxs-lookup"><span data-stu-id="99027-126">Name</span></span>       | <span data-ttu-id="99027-127">类型</span><span class="sxs-lookup"><span data-stu-id="99027-127">Type</span></span> | <span data-ttu-id="99027-128">说明</span><span class="sxs-lookup"><span data-stu-id="99027-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="99027-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="99027-129">Authorization</span></span>  | <span data-ttu-id="99027-130">string</span><span class="sxs-lookup"><span data-stu-id="99027-130">string</span></span>  | <span data-ttu-id="99027-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99027-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99027-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="99027-133">Request body</span></span>
<span data-ttu-id="99027-p106">在请求正文中，提供应更新的相关属性的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。以下是可写/可更新的属性：</span><span class="sxs-lookup"><span data-stu-id="99027-p106">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="99027-138">属性</span><span class="sxs-lookup"><span data-stu-id="99027-138">Property</span></span>     | <span data-ttu-id="99027-139">类型</span><span class="sxs-lookup"><span data-stu-id="99027-139">Type</span></span>   |<span data-ttu-id="99027-140">说明</span><span class="sxs-lookup"><span data-stu-id="99027-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99027-141">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="99027-141">automaticRepliesSetting</span></span>|[<span data-ttu-id="99027-142">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="99027-142">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="99027-143">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="99027-143">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="99027-144">只能将此类通知设置为将来日期范围。</span><span class="sxs-lookup"><span data-stu-id="99027-144">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="99027-145">语言</span><span class="sxs-lookup"><span data-stu-id="99027-145">language</span></span>|[<span data-ttu-id="99027-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="99027-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="99027-147">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="99027-147">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="99027-148">timeZone</span><span class="sxs-lookup"><span data-stu-id="99027-148">timeZone</span></span>|<span data-ttu-id="99027-149">string</span><span class="sxs-lookup"><span data-stu-id="99027-149">string</span></span>|<span data-ttu-id="99027-150">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="99027-150">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="99027-151">workingHours</span><span class="sxs-lookup"><span data-stu-id="99027-151">workingHours</span></span>|[<span data-ttu-id="99027-152">workingHours</span><span class="sxs-lookup"><span data-stu-id="99027-152">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="99027-153">用户工作的小时数、一周的天数和时区。</span><span class="sxs-lookup"><span data-stu-id="99027-153">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="99027-154">响应</span><span class="sxs-lookup"><span data-stu-id="99027-154">Response</span></span>

<span data-ttu-id="99027-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailboxSettings](../resources/mailboxsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99027-155">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="99027-156">错误</span><span class="sxs-lookup"><span data-stu-id="99027-156">Errors</span></span>

<span data-ttu-id="99027-157">将工作时间设置为不适当的值可能会返回以下错误。</span><span class="sxs-lookup"><span data-stu-id="99027-157">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="99027-158">应用场景</span><span class="sxs-lookup"><span data-stu-id="99027-158">Scenario</span></span>   | <span data-ttu-id="99027-159">HTTP 状态代码</span><span class="sxs-lookup"><span data-stu-id="99027-159">HTTP status code</span></span> | <span data-ttu-id="99027-160">错误代码</span><span class="sxs-lookup"><span data-stu-id="99027-160">Error code</span></span> | <span data-ttu-id="99027-161">错误消息</span><span class="sxs-lookup"><span data-stu-id="99027-161">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="99027-162">**startTime** 或 **endTime** 无效</span><span class="sxs-lookup"><span data-stu-id="99027-162">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="99027-163">400</span><span class="sxs-lookup"><span data-stu-id="99027-163">400</span></span> | <span data-ttu-id="99027-164">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="99027-164">RequestBodyRead</span></span> | <span data-ttu-id="99027-165">无法将文本“08”转换为预期类型“Edm.TimeOfDay”。</span><span class="sxs-lookup"><span data-stu-id="99027-165">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="99027-166">开始时间大于结束时间</span><span class="sxs-lookup"><span data-stu-id="99027-166">Start time is greater than end time</span></span> | <span data-ttu-id="99027-167">400</span><span class="sxs-lookup"><span data-stu-id="99027-167">400</span></span> | <span data-ttu-id="99027-168">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="99027-168">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="99027-169">开始时间应早于结束时间。</span><span class="sxs-lookup"><span data-stu-id="99027-169">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="99027-170">**daysOfWeek** 中的天数无效</span><span class="sxs-lookup"><span data-stu-id="99027-170">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="99027-171">400</span><span class="sxs-lookup"><span data-stu-id="99027-171">400</span></span> | <span data-ttu-id="99027-172">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="99027-172">InvalidArguments</span></span> | <span data-ttu-id="99027-173">未找到请求值“RandomDay”。</span><span class="sxs-lookup"><span data-stu-id="99027-173">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="99027-174">**timeZone** 无效</span><span class="sxs-lookup"><span data-stu-id="99027-174">Invalid **timeZone**</span></span> | <span data-ttu-id="99027-175">400</span><span class="sxs-lookup"><span data-stu-id="99027-175">400</span></span> | <span data-ttu-id="99027-176">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="99027-176">InvalidTimeZone</span></span> | <span data-ttu-id="99027-177">提供的时区设置无效。</span><span class="sxs-lookup"><span data-stu-id="99027-177">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="99027-178">示例</span><span class="sxs-lookup"><span data-stu-id="99027-178">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="99027-179">请求 1</span><span class="sxs-lookup"><span data-stu-id="99027-179">Request 1</span></span>
<span data-ttu-id="99027-180">第一个示例通过设置 **automaticRepliesSetting** 属性的以下属性来启用对日期范围的自动答复：**status**、**scheduledStartDateTime** 和 **scheduledEndDateTime**。</span><span class="sxs-lookup"><span data-stu-id="99027-180">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="99027-181">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="99027-181">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="99027-182">C#</span><span class="sxs-lookup"><span data-stu-id="99027-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99027-183">Javascript</span><span class="sxs-lookup"><span data-stu-id="99027-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99027-184">目标-C</span><span class="sxs-lookup"><span data-stu-id="99027-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="99027-185">响应 1</span><span class="sxs-lookup"><span data-stu-id="99027-185">Response 1</span></span>
<span data-ttu-id="99027-186">该响应包括自动答复的更新设置。</span><span class="sxs-lookup"><span data-stu-id="99027-186">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="99027-187">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="99027-187">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="99027-188">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99027-188">All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="99027-189">请求 2</span><span class="sxs-lookup"><span data-stu-id="99027-189">Request 2</span></span>
<span data-ttu-id="99027-190">第二个示例通过将 **timeZone** 属性设置为[自定义时区](../resources/customtimezone.md)，为登录用户的工作时间自定义时区。</span><span class="sxs-lookup"><span data-stu-id="99027-190">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

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
##### <a name="response-2"></a><span data-ttu-id="99027-191">响应 2</span><span class="sxs-lookup"><span data-stu-id="99027-191">Response 2</span></span>
<span data-ttu-id="99027-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99027-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
