# <a name="user-getmailtips"></a><span data-ttu-id="0618f-101">user: getMailTips</span><span class="sxs-lookup"><span data-stu-id="0618f-101">user: getMailTips</span></span>

<span data-ttu-id="0618f-102">获取登录[用户](../resources/user.md)的一个或多个可用联系人的邮件提醒。</span><span class="sxs-lookup"><span data-stu-id="0618f-102">Return the MailTips of one or more recipients as available to the signed-in user.</span></span>

<span data-ttu-id="0618f-103">请注意，通过使 `POST` 调用 `getMailTips` 操作，可以请求一次向一个以上的收件人返回特定类型的邮件提醒。</span><span class="sxs-lookup"><span data-stu-id="0618f-103">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="0618f-104">被请求的邮件提示被返回到 [mailTips](../resources/mailtips.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="0618f-104">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="0618f-105">权限</span><span class="sxs-lookup"><span data-stu-id="0618f-105">Permissions</span></span>
<span data-ttu-id="0618f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0618f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0618f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0618f-108">Permission type</span></span>      | <span data-ttu-id="0618f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0618f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0618f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0618f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0618f-111">Mail.Read, Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="0618f-111">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="0618f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0618f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0618f-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0618f-113">Mail.Read</span></span>    |
|<span data-ttu-id="0618f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0618f-114">Application</span></span> | <span data-ttu-id="0618f-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0618f-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="0618f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0618f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0618f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0618f-117">Optional query parameters</span></span>
<span data-ttu-id="0618f-118">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0618f-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0618f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0618f-119">Request headers</span></span>
| <span data-ttu-id="0618f-120">标头</span><span class="sxs-lookup"><span data-stu-id="0618f-120">Header</span></span>       | <span data-ttu-id="0618f-121">值</span><span class="sxs-lookup"><span data-stu-id="0618f-121">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="0618f-122">授权</span><span class="sxs-lookup"><span data-stu-id="0618f-122">Authorization</span></span> | <span data-ttu-id="0618f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0618f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0618f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0618f-125">Content-Type</span></span>  | <span data-ttu-id="0618f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0618f-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0618f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0618f-127">Request body</span></span>
<span data-ttu-id="0618f-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0618f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0618f-129">属性</span><span class="sxs-lookup"><span data-stu-id="0618f-129">Property</span></span>     | <span data-ttu-id="0618f-130">类型</span><span class="sxs-lookup"><span data-stu-id="0618f-130">Type</span></span>   |<span data-ttu-id="0618f-131">说明</span><span class="sxs-lookup"><span data-stu-id="0618f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0618f-132">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="0618f-132">EmailAddresses</span></span>|<span data-ttu-id="0618f-133">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0618f-133">String collection</span></span>|<span data-ttu-id="0618f-134">用于获取“邮件提醒”的收件人 SMTP 地址的集合。</span><span class="sxs-lookup"><span data-stu-id="0618f-134">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="0618f-135">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="0618f-135">MailTipsOptions</span></span>|<span data-ttu-id="0618f-136">字符串</span><span class="sxs-lookup"><span data-stu-id="0618f-136">String</span></span>|<span data-ttu-id="0618f-137">枚举代​​表请求的邮件提醒的标志。</span><span class="sxs-lookup"><span data-stu-id="0618f-137">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="0618f-138">可取值为：`automaticReplies`、`customMailTip`、`deliveryRestriction`、`externalMemberCount`、`mailboxFullStatus`、`maxMessageSize`、`moderationStatus`、`recipientScope`、`recipientSuggestions` 和  `totalMemberCount`。</span><span class="sxs-lookup"><span data-stu-id="0618f-138">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`,`mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="0618f-139">响应</span><span class="sxs-lookup"><span data-stu-id="0618f-139">Response</span></span>

<span data-ttu-id="0618f-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailTips](../resources/mailtips.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0618f-140">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0618f-141">示例</span><span class="sxs-lookup"><span data-stu-id="0618f-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0618f-142">请求</span><span class="sxs-lookup"><span data-stu-id="0618f-142">Request</span></span>
<span data-ttu-id="0618f-143">以下示例获取指定收件人的“邮件提醒”，以获取任何自动回复设置和邮箱全状态。</span><span class="sxs-lookup"><span data-stu-id="0618f-143">The following example gets MailTips for the specified recipients, for any automatic reply settings and mailbox full status.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a><span data-ttu-id="0618f-144">响应</span><span class="sxs-lookup"><span data-stu-id="0618f-144">Response</span></span>
<span data-ttu-id="0618f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0618f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailTips",
  isCollection: true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.mailTips)",
    "value":[
        {
            "emailAddress":{
                "name":"",
                "address":"danas@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":"<style type=\"text/css\" style=\"\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n<div dir=\"ltr\">\r\n<div id=\"x_divtagdefaultwrapper\" style=\"font-size:12pt; color:#000000; background-color:#FFFFFF; font-family:Calibri,Arial,Helvetica,sans-serif\">\r\n<p>Hi, I am on vacation right now. I'll get back to you after I return.<br>\r\n</p>\r\n</div>\r\n</div>",
                "messageLanguage":{
                    "locale":"en-US",
                    "displayName":"English (United States)"
                },
                "scheduledStartTime": {
                    "dateTime": "2018-08-07T02:00:00.0000000",
                    "timeZone": "UTC"
                },
                "scheduledEndTime": {
                    "dateTime": "2018-08-09T02:00:00.0000000",
                    "timeZone": "UTC"
                }
            },
            "mailboxFull":false
        },
        {
            "emailAddress":{
                "name":"",
                "address":"fannyd@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":""
            },
            "mailboxFull":false
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
