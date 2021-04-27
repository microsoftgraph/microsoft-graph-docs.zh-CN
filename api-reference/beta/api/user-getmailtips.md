---
title: user： getMailTips
description: 获取登录用户可用的一个或多个收件人的邮件提示。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4fb7e85c4a3590bf4b5688588e4c6cc29326b181
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052619"
---
# <a name="user-getmailtips"></a><span data-ttu-id="f86bc-103">user： getMailTips</span><span class="sxs-lookup"><span data-stu-id="f86bc-103">user: getMailTips</span></span>

<span data-ttu-id="f86bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f86bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f86bc-105">获取登录用户可用的一个或多个收件人的邮件 [提示](../resources/user.md)。</span><span class="sxs-lookup"><span data-stu-id="f86bc-105">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="f86bc-106">请注意，通过调用操作，可以请求同时为多个收件人返回特定类型的邮件 `POST` `getMailTips` 提示。</span><span class="sxs-lookup"><span data-stu-id="f86bc-106">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="f86bc-107">请求的邮件提示在邮件 [提示](../resources/mailtips.md) 集合中返回。</span><span class="sxs-lookup"><span data-stu-id="f86bc-107">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="f86bc-108">权限</span><span class="sxs-lookup"><span data-stu-id="f86bc-108">Permissions</span></span>
<span data-ttu-id="f86bc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f86bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f86bc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f86bc-111">Permission type</span></span>      | <span data-ttu-id="f86bc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f86bc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f86bc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f86bc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f86bc-114">Mail.Read、Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="f86bc-114">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="f86bc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f86bc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f86bc-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f86bc-116">Mail.Read</span></span>    |
|<span data-ttu-id="f86bc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f86bc-117">Application</span></span> | <span data-ttu-id="f86bc-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f86bc-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f86bc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f86bc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f86bc-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f86bc-120">Optional query parameters</span></span>
<span data-ttu-id="f86bc-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f86bc-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f86bc-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f86bc-122">Request headers</span></span>
| <span data-ttu-id="f86bc-123">标头</span><span class="sxs-lookup"><span data-stu-id="f86bc-123">Header</span></span>       | <span data-ttu-id="f86bc-124">值</span><span class="sxs-lookup"><span data-stu-id="f86bc-124">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="f86bc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f86bc-125">Authorization</span></span> | <span data-ttu-id="f86bc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f86bc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f86bc-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f86bc-128">Content-Type</span></span>  | <span data-ttu-id="f86bc-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f86bc-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f86bc-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f86bc-130">Request body</span></span>
<span data-ttu-id="f86bc-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f86bc-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f86bc-132">属性</span><span class="sxs-lookup"><span data-stu-id="f86bc-132">Property</span></span>     | <span data-ttu-id="f86bc-133">类型</span><span class="sxs-lookup"><span data-stu-id="f86bc-133">Type</span></span>   |<span data-ttu-id="f86bc-134">说明</span><span class="sxs-lookup"><span data-stu-id="f86bc-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f86bc-135">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="f86bc-135">EmailAddresses</span></span>|<span data-ttu-id="f86bc-136">字符串集合</span><span class="sxs-lookup"><span data-stu-id="f86bc-136">String collection</span></span>|<span data-ttu-id="f86bc-137">要获取邮件提示的收件人的 SMTP 地址的集合。</span><span class="sxs-lookup"><span data-stu-id="f86bc-137">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="f86bc-138">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="f86bc-138">MailTipsOptions</span></span>|<span data-ttu-id="f86bc-139">String</span><span class="sxs-lookup"><span data-stu-id="f86bc-139">String</span></span>|<span data-ttu-id="f86bc-140">表示请求的邮件提示的标志的枚举。</span><span class="sxs-lookup"><span data-stu-id="f86bc-140">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="f86bc-141">可能的值是 `automaticReplies` `customMailTip` `deliveryRestriction` ：、、、、、、、、 `externalMemberCount` `mailboxFullStatus` `maxMessageSize` 和 `moderationStatus` `recipientScope` `recipientSuggestions` `totalMemberCount` 。</span><span class="sxs-lookup"><span data-stu-id="f86bc-141">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="f86bc-142">响应</span><span class="sxs-lookup"><span data-stu-id="f86bc-142">Response</span></span>

<span data-ttu-id="f86bc-143">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [mailTips](../resources/mailtips.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f86bc-143">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f86bc-144">示例</span><span class="sxs-lookup"><span data-stu-id="f86bc-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f86bc-145">请求</span><span class="sxs-lookup"><span data-stu-id="f86bc-145">Request</span></span>
<span data-ttu-id="f86bc-146">下面的示例获取任何自动答复设置和邮箱已满状态的指定收件人的邮件提示。</span><span class="sxs-lookup"><span data-stu-id="f86bc-146">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>


# <a name="http"></a>[<span data-ttu-id="f86bc-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="f86bc-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f86bc-148">C#</span><span class="sxs-lookup"><span data-stu-id="f86bc-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmailtips-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f86bc-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f86bc-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmailtips-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f86bc-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f86bc-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmailtips-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f86bc-151">Java</span><span class="sxs-lookup"><span data-stu-id="f86bc-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmailtips-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f86bc-152">响应</span><span class="sxs-lookup"><span data-stu-id="f86bc-152">Response</span></span>
<span data-ttu-id="f86bc-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f86bc-153">Here is an example of the response.</span></span> <span data-ttu-id="f86bc-154">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f86bc-154">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
