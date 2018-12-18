---
title: 用户： getMailTips
description: 获取已登录的用户作为可用的一个或多个收件人的邮件提示。
author: dkershaw10
ms.openlocfilehash: 039d86c728c2394153ebe1a5aebba1243d40d726
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304044"
---
# <a name="user-getmailtips"></a><span data-ttu-id="5b02b-103">用户： getMailTips</span><span class="sxs-lookup"><span data-stu-id="5b02b-103">user: getMailTips</span></span>

> <span data-ttu-id="5b02b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5b02b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b02b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b02b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b02b-106">获取有空登录[用户](../resources/user.md)的一个或多个收件人的邮件提示。</span><span class="sxs-lookup"><span data-stu-id="5b02b-106">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="5b02b-107">请注意，通过使`POST`调用`getMailTips`操作，您可以请求对特定类型的邮件提示，一次返回多个收件人。</span><span class="sxs-lookup"><span data-stu-id="5b02b-107">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="5b02b-108">[邮件提示](../resources/mailtips.md)集合中返回请求的邮件提示。</span><span class="sxs-lookup"><span data-stu-id="5b02b-108">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b02b-109">权限</span><span class="sxs-lookup"><span data-stu-id="5b02b-109">Permissions</span></span>
<span data-ttu-id="5b02b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b02b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b02b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b02b-112">Permission type</span></span>      | <span data-ttu-id="5b02b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b02b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b02b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b02b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5b02b-115">Mail.Read Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="5b02b-115">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="5b02b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b02b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b02b-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5b02b-117">Mail.Read</span></span>    |
|<span data-ttu-id="5b02b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b02b-118">Application</span></span> | <span data-ttu-id="5b02b-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5b02b-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b02b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b02b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b02b-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5b02b-121">Optional query parameters</span></span>
<span data-ttu-id="5b02b-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5b02b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5b02b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b02b-123">Request headers</span></span>
| <span data-ttu-id="5b02b-124">标头</span><span class="sxs-lookup"><span data-stu-id="5b02b-124">Header</span></span>       | <span data-ttu-id="5b02b-125">值</span><span class="sxs-lookup"><span data-stu-id="5b02b-125">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="5b02b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b02b-126">Authorization</span></span> | <span data-ttu-id="5b02b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b02b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b02b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b02b-129">Content-Type</span></span>  | <span data-ttu-id="5b02b-130">application/json</span><span class="sxs-lookup"><span data-stu-id="5b02b-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b02b-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b02b-131">Request body</span></span>
<span data-ttu-id="5b02b-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5b02b-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5b02b-133">属性</span><span class="sxs-lookup"><span data-stu-id="5b02b-133">Property</span></span>     | <span data-ttu-id="5b02b-134">类型</span><span class="sxs-lookup"><span data-stu-id="5b02b-134">Type</span></span>   |<span data-ttu-id="5b02b-135">说明</span><span class="sxs-lookup"><span data-stu-id="5b02b-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b02b-136">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="5b02b-136">EmailAddresses</span></span>|<span data-ttu-id="5b02b-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="5b02b-137">String collection</span></span>|<span data-ttu-id="5b02b-138">要获取的邮件提示的收件人的 SMTP 地址的集合。</span><span class="sxs-lookup"><span data-stu-id="5b02b-138">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="5b02b-139">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="5b02b-139">MailTipsOptions</span></span>|<span data-ttu-id="5b02b-140">字符串</span><span class="sxs-lookup"><span data-stu-id="5b02b-140">String</span></span>|<span data-ttu-id="5b02b-141">Flags 一个枚举值，该值代表请求邮件提示。</span><span class="sxs-lookup"><span data-stu-id="5b02b-141">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="5b02b-142">可能的值为： `automaticReplies`， `customMailTip`， `deliveryRestriction`， `externalMemberCount`， `mailboxFullStatus`， `maxMessageSize`， `moderationStatus`， `recipientScope`， `recipientSuggestions`，和`totalMemberCount`。</span><span class="sxs-lookup"><span data-stu-id="5b02b-142">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="5b02b-143">响应</span><span class="sxs-lookup"><span data-stu-id="5b02b-143">Response</span></span>

<span data-ttu-id="5b02b-144">如果成功，此方法返回`200 OK`响应代码和响应正文中的[邮件提示](../resources/mailtips.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5b02b-144">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b02b-145">示例</span><span class="sxs-lookup"><span data-stu-id="5b02b-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b02b-146">请求</span><span class="sxs-lookup"><span data-stu-id="5b02b-146">Request</span></span>
<span data-ttu-id="5b02b-147">下面的示例获取指定的收件人，任何自动答复设置和邮箱完全状态邮件提示。</span><span class="sxs-lookup"><span data-stu-id="5b02b-147">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a><span data-ttu-id="5b02b-148">响应</span><span class="sxs-lookup"><span data-stu-id="5b02b-148">Response</span></span>
<span data-ttu-id="5b02b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b02b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailTips)",
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
