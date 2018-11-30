---
title: 用户： getMailTips
description: 获取已登录的用户作为可用的一个或多个收件人的邮件提示。
ms.openlocfilehash: 2291c8569d3e283e86598c0fd6fe5a0f487e79e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011135"
---
# <a name="user-getmailtips"></a><span data-ttu-id="8c75d-103">用户： getMailTips</span><span class="sxs-lookup"><span data-stu-id="8c75d-103">user: getMailTips</span></span>

<span data-ttu-id="8c75d-104">获取有空登录[用户](../resources/user.md)的一个或多个收件人的邮件提示。</span><span class="sxs-lookup"><span data-stu-id="8c75d-104">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="8c75d-105">请注意，通过使`POST`调用`getMailTips`操作，您可以请求对特定类型的邮件提示，一次返回多个收件人。</span><span class="sxs-lookup"><span data-stu-id="8c75d-105">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="8c75d-106">[邮件提示](../resources/mailtips.md)集合中返回请求的邮件提示。</span><span class="sxs-lookup"><span data-stu-id="8c75d-106">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c75d-107">权限</span><span class="sxs-lookup"><span data-stu-id="8c75d-107">Permissions</span></span>
<span data-ttu-id="8c75d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c75d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c75d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c75d-110">Permission type</span></span>      | <span data-ttu-id="8c75d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c75d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c75d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c75d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c75d-113">Mail.Read Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="8c75d-113">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="8c75d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c75d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c75d-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8c75d-115">Mail.Read</span></span>    |
|<span data-ttu-id="8c75d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c75d-116">Application</span></span> | <span data-ttu-id="8c75d-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8c75d-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c75d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c75d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c75d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8c75d-119">Optional query parameters</span></span>
<span data-ttu-id="8c75d-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8c75d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8c75d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c75d-121">Request headers</span></span>
| <span data-ttu-id="8c75d-122">标头</span><span class="sxs-lookup"><span data-stu-id="8c75d-122">Header</span></span>       | <span data-ttu-id="8c75d-123">值</span><span class="sxs-lookup"><span data-stu-id="8c75d-123">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="8c75d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c75d-124">Authorization</span></span> | <span data-ttu-id="8c75d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c75d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c75d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c75d-127">Content-Type</span></span>  | <span data-ttu-id="8c75d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8c75d-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c75d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c75d-129">Request body</span></span>
<span data-ttu-id="8c75d-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8c75d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c75d-131">属性</span><span class="sxs-lookup"><span data-stu-id="8c75d-131">Property</span></span>     | <span data-ttu-id="8c75d-132">类型</span><span class="sxs-lookup"><span data-stu-id="8c75d-132">Type</span></span>   |<span data-ttu-id="8c75d-133">说明</span><span class="sxs-lookup"><span data-stu-id="8c75d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c75d-134">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="8c75d-134">EmailAddresses</span></span>|<span data-ttu-id="8c75d-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="8c75d-135">String collection</span></span>|<span data-ttu-id="8c75d-136">要获取的邮件提示的收件人的 SMTP 地址的集合。</span><span class="sxs-lookup"><span data-stu-id="8c75d-136">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="8c75d-137">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="8c75d-137">MailTipsOptions</span></span>|<span data-ttu-id="8c75d-138">字符串</span><span class="sxs-lookup"><span data-stu-id="8c75d-138">String</span></span>|<span data-ttu-id="8c75d-139">Flags 一个枚举值，该值代表请求邮件提示。</span><span class="sxs-lookup"><span data-stu-id="8c75d-139">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="8c75d-140">可能的值为： `automaticReplies`， `customMailTip`， `deliveryRestriction`， `externalMemberCount`， `mailboxFullStatus`， `maxMessageSize`， `moderationStatus`， `recipientScope`， `recipientSuggestions`，和`totalMemberCount`。</span><span class="sxs-lookup"><span data-stu-id="8c75d-140">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="8c75d-141">响应</span><span class="sxs-lookup"><span data-stu-id="8c75d-141">Response</span></span>

<span data-ttu-id="8c75d-142">如果成功，此方法返回`200 OK`响应代码和响应正文中的[邮件提示](../resources/mailtips.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="8c75d-142">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c75d-143">示例</span><span class="sxs-lookup"><span data-stu-id="8c75d-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c75d-144">请求</span><span class="sxs-lookup"><span data-stu-id="8c75d-144">Request</span></span>
<span data-ttu-id="8c75d-145">下面的示例获取指定的收件人，任何自动答复设置和邮箱完全状态邮件提示。</span><span class="sxs-lookup"><span data-stu-id="8c75d-145">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

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

##### <a name="response"></a><span data-ttu-id="8c75d-146">响应</span><span class="sxs-lookup"><span data-stu-id="8c75d-146">Response</span></span>
<span data-ttu-id="8c75d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c75d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
