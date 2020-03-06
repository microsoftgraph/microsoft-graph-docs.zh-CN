---
title: 用户： getMailTips
description: 获取一个或多个收件人对登录用户可用的邮件提示。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 28f4dead5edab55f30c80b524d0f124473d2acd2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509179"
---
# <a name="user-getmailtips"></a><span data-ttu-id="08878-103">用户： getMailTips</span><span class="sxs-lookup"><span data-stu-id="08878-103">user: getMailTips</span></span>

<span data-ttu-id="08878-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08878-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08878-105">获取一个或多个收件人对登录[用户](../resources/user.md)可用的邮件提示。</span><span class="sxs-lookup"><span data-stu-id="08878-105">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="08878-106">请注意，通过`POST`调用`getMailTips`操作，您可以请求一次为多个收件人返回特定类型的邮件提示。</span><span class="sxs-lookup"><span data-stu-id="08878-106">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="08878-107">在[邮件](../resources/mailtips.md)提示集合中返回请求的邮件提示。</span><span class="sxs-lookup"><span data-stu-id="08878-107">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="08878-108">权限</span><span class="sxs-lookup"><span data-stu-id="08878-108">Permissions</span></span>
<span data-ttu-id="08878-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08878-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08878-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="08878-111">Permission type</span></span>      | <span data-ttu-id="08878-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08878-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08878-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08878-113">Delegated (work or school account)</span></span> | <span data-ttu-id="08878-114">已阅读 "邮件"、"读取"、"共享"</span><span class="sxs-lookup"><span data-stu-id="08878-114">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="08878-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08878-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08878-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="08878-116">Mail.Read</span></span>    |
|<span data-ttu-id="08878-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="08878-117">Application</span></span> | <span data-ttu-id="08878-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="08878-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="08878-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08878-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="08878-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="08878-120">Optional query parameters</span></span>
<span data-ttu-id="08878-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="08878-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="08878-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="08878-122">Request headers</span></span>
| <span data-ttu-id="08878-123">标头</span><span class="sxs-lookup"><span data-stu-id="08878-123">Header</span></span>       | <span data-ttu-id="08878-124">值</span><span class="sxs-lookup"><span data-stu-id="08878-124">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="08878-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="08878-125">Authorization</span></span> | <span data-ttu-id="08878-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08878-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08878-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08878-128">Content-Type</span></span>  | <span data-ttu-id="08878-129">application/json</span><span class="sxs-lookup"><span data-stu-id="08878-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08878-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="08878-130">Request body</span></span>
<span data-ttu-id="08878-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="08878-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08878-132">属性</span><span class="sxs-lookup"><span data-stu-id="08878-132">Property</span></span>     | <span data-ttu-id="08878-133">类型</span><span class="sxs-lookup"><span data-stu-id="08878-133">Type</span></span>   |<span data-ttu-id="08878-134">说明</span><span class="sxs-lookup"><span data-stu-id="08878-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08878-135">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="08878-135">EmailAddresses</span></span>|<span data-ttu-id="08878-136">String collection</span><span class="sxs-lookup"><span data-stu-id="08878-136">String collection</span></span>|<span data-ttu-id="08878-137">要获取其邮件提示的收件人的 SMTP 地址集合。</span><span class="sxs-lookup"><span data-stu-id="08878-137">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="08878-138">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="08878-138">MailTipsOptions</span></span>|<span data-ttu-id="08878-139">字符串</span><span class="sxs-lookup"><span data-stu-id="08878-139">String</span></span>|<span data-ttu-id="08878-140">表示请求的邮件提示的标志的枚举。</span><span class="sxs-lookup"><span data-stu-id="08878-140">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="08878-141">可能的值为`automaticReplies`： `customMailTip`、 `deliveryRestriction`、 `externalMemberCount` `mailboxFullStatus` `maxMessageSize` `moderationStatus` `recipientScope`、、、、、、和`totalMemberCount` `recipientSuggestions`</span><span class="sxs-lookup"><span data-stu-id="08878-141">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="08878-142">响应</span><span class="sxs-lookup"><span data-stu-id="08878-142">Response</span></span>

<span data-ttu-id="08878-143">如果成功，此方法在响应`200 OK`正文中返回响应代码和[邮件](../resources/mailtips.md)提示对象集合。</span><span class="sxs-lookup"><span data-stu-id="08878-143">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08878-144">示例</span><span class="sxs-lookup"><span data-stu-id="08878-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08878-145">请求</span><span class="sxs-lookup"><span data-stu-id="08878-145">Request</span></span>
<span data-ttu-id="08878-146">下面的示例获取指定收件人的邮件提示，以获取自动答复设置和邮箱完整状态。</span><span class="sxs-lookup"><span data-stu-id="08878-146">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>


# <a name="http"></a>[<span data-ttu-id="08878-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="08878-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="08878-148">C#</span><span class="sxs-lookup"><span data-stu-id="08878-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmailtips-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08878-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08878-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmailtips-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08878-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08878-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmailtips-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08878-151">Java</span><span class="sxs-lookup"><span data-stu-id="08878-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmailtips-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08878-152">响应</span><span class="sxs-lookup"><span data-stu-id="08878-152">Response</span></span>
<span data-ttu-id="08878-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08878-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
