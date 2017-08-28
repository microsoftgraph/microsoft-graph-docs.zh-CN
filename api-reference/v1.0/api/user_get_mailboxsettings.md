# <a name="get-user-mailbox-settings"></a><span data-ttu-id="857e6-101">获取用户的邮箱设置</span><span class="sxs-lookup"><span data-stu-id="857e6-101">Get user mailbox settings</span></span>

<span data-ttu-id="857e6-p101">获取用户的 [mailboxSettings](../resources/mailboxsettings.md)。这包括自动答复（收到发件人的电子邮件时自动通知发件人）、区域设置（语言和国家/地区）和时区设置。</span><span class="sxs-lookup"><span data-stu-id="857e6-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.</span></span>

<span data-ttu-id="857e6-104">可以查看所有的邮箱设置或获取特定设置。</span><span class="sxs-lookup"><span data-stu-id="857e6-104">You can view all mailbox settings, or, get specific settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="857e6-105">权限</span><span class="sxs-lookup"><span data-stu-id="857e6-105">Permissions</span></span>
<span data-ttu-id="857e6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="857e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="857e6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="857e6-108">Permission type</span></span>      | <span data-ttu-id="857e6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="857e6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="857e6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="857e6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="857e6-111">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="857e6-111">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="857e6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="857e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="857e6-113">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="857e6-113">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="857e6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="857e6-114">Application</span></span> | <span data-ttu-id="857e6-115">MailboxSettings.Read、MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="857e6-115">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="857e6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="857e6-116">HTTP request</span></span>
<span data-ttu-id="857e6-117">获取包括自动答复设置的所有邮箱设置：</span><span class="sxs-lookup"><span data-stu-id="857e6-117">To get all mailbox settings which include automatic replies settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="857e6-118">获取特定设置，例如，仅获取自动答复设置、区域设置或时区：</span><span class="sxs-lookup"><span data-stu-id="857e6-118">To get specific settings - for example, only the automatic replies settings, locale, or time zone:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
```
## <a name="optional-query-parameters"></a><span data-ttu-id="857e6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="857e6-119">Optional query parameters</span></span>
<span data-ttu-id="857e6-120">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="857e6-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="857e6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="857e6-121">Request headers</span></span>
| <span data-ttu-id="857e6-122">名称</span><span class="sxs-lookup"><span data-stu-id="857e6-122">Name</span></span>       | <span data-ttu-id="857e6-123">类型</span><span class="sxs-lookup"><span data-stu-id="857e6-123">Type</span></span> | <span data-ttu-id="857e6-124">说明</span><span class="sxs-lookup"><span data-stu-id="857e6-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="857e6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="857e6-125">Authorization</span></span>  | <span data-ttu-id="857e6-126">string</span><span class="sxs-lookup"><span data-stu-id="857e6-126">string</span></span>  | <span data-ttu-id="857e6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="857e6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="857e6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="857e6-129">Request body</span></span>
<span data-ttu-id="857e6-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="857e6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="857e6-131">响应</span><span class="sxs-lookup"><span data-stu-id="857e6-131">Response</span></span>

<span data-ttu-id="857e6-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和以下请求对象之一：</span><span class="sxs-lookup"><span data-stu-id="857e6-132">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="857e6-133">[mailboxSettings](../resources/mailboxsettings.md) 对象</span><span class="sxs-lookup"><span data-stu-id="857e6-133">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="857e6-134">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) 对象</span><span class="sxs-lookup"><span data-stu-id="857e6-134">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="857e6-135">[localeInfo](../resources/localeinfo.md) 对象</span><span class="sxs-lookup"><span data-stu-id="857e6-135">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="857e6-136">字符串（适用于 **timeZone**）</span><span class="sxs-lookup"><span data-stu-id="857e6-136">string (for **timeZone**)</span></span>

## <a name="example"></a><span data-ttu-id="857e6-137">示例</span><span class="sxs-lookup"><span data-stu-id="857e6-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="857e6-138">请求 1</span><span class="sxs-lookup"><span data-stu-id="857e6-138">Request 1</span></span>
<span data-ttu-id="857e6-139">第一个示例获取已登录用户邮箱的所有邮箱设置，其中包括自动答复设置、时区和语言设置。</span><span class="sxs-lookup"><span data-stu-id="857e6-139">The first example gets all the mailbox settings of the signed-in user's mailbox, which include automatic replies settings, time zone, and language settings.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="857e6-140">响应 1</span><span class="sxs-lookup"><span data-stu-id="857e6-140">Response 1</span></span>
<span data-ttu-id="857e6-p104">该响应包括所有的邮箱设置。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="857e6-p104">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="857e6-144">请求 2</span><span class="sxs-lookup"><span data-stu-id="857e6-144">Request 2</span></span>
<span data-ttu-id="857e6-145">第二个示例专门获取已登录用户邮箱的自动答复设置。</span><span class="sxs-lookup"><span data-stu-id="857e6-145">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="857e6-146">响应 2</span><span class="sxs-lookup"><span data-stu-id="857e6-146">Response 2</span></span>
<span data-ttu-id="857e6-p105">该响应仅包括自动答复设置。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="857e6-p105">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->