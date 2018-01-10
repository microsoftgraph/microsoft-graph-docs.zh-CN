# <a name="update-user-mailbox-settings"></a><span data-ttu-id="b9c71-101">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="b9c71-101">Update user mailbox settings</span></span>

<span data-ttu-id="b9c71-p101">更新用户邮箱的一个或多个设置。这包括自动答复（收到发件人的电子邮件时自动通知发件人）、区域设置或时区设置。</span><span class="sxs-lookup"><span data-stu-id="b9c71-p101">Update one or more settings for the user's mailbox. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale, or time zone.</span></span>

<span data-ttu-id="b9c71-104">可以作为 [mailboxSettings](../resources/mailboxsettings.md) 的一部分启用、配置或禁用其中的一个或多个设置。</span><span class="sxs-lookup"><span data-stu-id="b9c71-104">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="b9c71-105">**注意**：不能创建或删除任何邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="b9c71-105">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="b9c71-106">更新用户的首选时区时，可以指定 Windows 时区或 [Internet 号码分配局 (IANA) 时区]((http://www.iana.org/time-zones))（亦称为“Olson 时区”）。</span><span class="sxs-lookup"><span data-stu-id="b9c71-106">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone]((http://www.iana.org/time-zones)) (also known as Olson time zone) format.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9c71-107">权限</span><span class="sxs-lookup"><span data-stu-id="b9c71-107">Permissions</span></span>
<span data-ttu-id="b9c71-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b9c71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9c71-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9c71-110">Permission type</span></span>      | <span data-ttu-id="b9c71-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9c71-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9c71-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c71-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b9c71-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9c71-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b9c71-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c71-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9c71-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9c71-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b9c71-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9c71-116">Application</span></span> | <span data-ttu-id="b9c71-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9c71-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9c71-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9c71-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9c71-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b9c71-119">Optional query parameters</span></span>
<span data-ttu-id="b9c71-120">此方法支持 [OData 查询参数]((http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters)) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b9c71-120">This method supports the [OData Query Parameters]((http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b9c71-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9c71-121">Request headers</span></span>
| <span data-ttu-id="b9c71-122">名称</span><span class="sxs-lookup"><span data-stu-id="b9c71-122">Name</span></span>       | <span data-ttu-id="b9c71-123">类型</span><span class="sxs-lookup"><span data-stu-id="b9c71-123">Type</span></span> | <span data-ttu-id="b9c71-124">说明</span><span class="sxs-lookup"><span data-stu-id="b9c71-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b9c71-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9c71-125">Authorization</span></span>  | <span data-ttu-id="b9c71-126">string</span><span class="sxs-lookup"><span data-stu-id="b9c71-126">string</span></span>  | <span data-ttu-id="b9c71-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9c71-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9c71-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9c71-129">Request body</span></span>
<span data-ttu-id="b9c71-p104">在请求正文中，提供应更新的相关属性的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。以下是可写/可更新的属性：</span><span class="sxs-lookup"><span data-stu-id="b9c71-p104">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="b9c71-134">属性</span><span class="sxs-lookup"><span data-stu-id="b9c71-134">Property</span></span>     | <span data-ttu-id="b9c71-135">类型</span><span class="sxs-lookup"><span data-stu-id="b9c71-135">Type</span></span>   |<span data-ttu-id="b9c71-136">说明</span><span class="sxs-lookup"><span data-stu-id="b9c71-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9c71-137">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="b9c71-137">automaticRepliesSetting</span></span>|[<span data-ttu-id="b9c71-138">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="b9c71-138">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="b9c71-139">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="b9c71-139">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="b9c71-140">语言</span><span class="sxs-lookup"><span data-stu-id="b9c71-140">language</span></span>|[<span data-ttu-id="b9c71-141">localeInfo</span><span class="sxs-lookup"><span data-stu-id="b9c71-141">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="b9c71-142">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="b9c71-142">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="b9c71-143">timeZone</span><span class="sxs-lookup"><span data-stu-id="b9c71-143">timeZone</span></span>|<span data-ttu-id="b9c71-144">string</span><span class="sxs-lookup"><span data-stu-id="b9c71-144">string</span></span>|<span data-ttu-id="b9c71-145">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="b9c71-145">The default time zone for the user's mailbox.</span></span>|

## <a name="response"></a><span data-ttu-id="b9c71-146">响应</span><span class="sxs-lookup"><span data-stu-id="b9c71-146">Response</span></span>

<span data-ttu-id="b9c71-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailboxSettings](../resources/mailboxSettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9c71-147">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxSettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9c71-148">示例</span><span class="sxs-lookup"><span data-stu-id="b9c71-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9c71-149">请求</span><span class="sxs-lookup"><span data-stu-id="b9c71-149">Request</span></span>
<span data-ttu-id="b9c71-150">以下示例通过设置 **automaticRepliesSetting** 属性的以下属性来启用对日期范围的自动答复：**status**、**scheduledStartDateTime** 和 **scheduledEndDateTime**。</span><span class="sxs-lookup"><span data-stu-id="b9c71-150">The following example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings"
}-->
```http
PATCH https://graph.microsoft.com/api/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings",
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
##### <a name="response"></a><span data-ttu-id="b9c71-151">响应</span><span class="sxs-lookup"><span data-stu-id="b9c71-151">Response</span></span>
<span data-ttu-id="b9c71-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9c71-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "none",
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
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
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