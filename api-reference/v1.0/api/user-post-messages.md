---
title: 创建邮件
description: 采用 JSON 或 MIME 格式创建新邮件的草稿。
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6419ec8bef225964b5797e84cce0f3ecf7609b30
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870393"
---
# <a name="create-message"></a><span data-ttu-id="551f3-103">创建邮件</span><span class="sxs-lookup"><span data-stu-id="551f3-103">Create message</span></span>

<span data-ttu-id="551f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="551f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="551f3-105">采用 JSON 或 MIME 格式创建新[邮件](../resources/message.md)的草稿。</span><span class="sxs-lookup"><span data-stu-id="551f3-105">Create a draft of a new [message](../resources/message.md) in either JSON or MIME format.</span></span>

<span data-ttu-id="551f3-106">使用 JSON 格式时，可以：</span><span class="sxs-lookup"><span data-stu-id="551f3-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="551f3-107">包含 [附件](../resources/attachment.md)到 **邮件** 中。</span><span class="sxs-lookup"><span data-stu-id="551f3-107">Include an [attachment](../resources/attachment.md) to the **message**.</span></span>
- <span data-ttu-id="551f3-108">随后 [更新](../api/message-update.md)草稿以将内容添加到 **正文**，或更改其他邮件属性。</span><span class="sxs-lookup"><span data-stu-id="551f3-108">[Update](../api/message-update.md) the draft later to add content to the **body** or change other message properties.</span></span>

<span data-ttu-id="551f3-109">使用 MIME 格式时：</span><span class="sxs-lookup"><span data-stu-id="551f3-109">When using MIME format:</span></span>
- <span data-ttu-id="551f3-110">提供适用的 [Internet 邮件头](https://tools.ietf.org/html/rfc2076) 和 [MIME 内容](https://tools.ietf.org/html/rfc2045)，所有内容在请求正文中都通过 **base64** 格式进行编码。</span><span class="sxs-lookup"><span data-stu-id="551f3-110">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="551f3-111">向 MIME 内容添加任何附件和 S/MIME 属性。</span><span class="sxs-lookup"><span data-stu-id="551f3-111">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="551f3-112">默认情况下，此操作将草稿保存在“草稿”文件夹中。</span><span class="sxs-lookup"><span data-stu-id="551f3-112">By default, this operation saves the draft in the Drafts folder.</span></span>

<span data-ttu-id="551f3-113">在后续操作中[发送](/graph/api-reference/beta/api/message-send.md)草稿消息。</span><span class="sxs-lookup"><span data-stu-id="551f3-113">[Send](/graph/api-reference/beta/api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="551f3-114">或者，通过一次操作[发送新邮件](../api/user-sendmail.md) ，或创建一个草稿以[转发](../api/message-createforward.md)、[答复](../api/message-createreply.md)和[答复所有](../api/message-createreplyall.md)现有邮件。</span><span class="sxs-lookup"><span data-stu-id="551f3-114">Alternatively, [send a new message](../api/user-sendmail.md) in a single operation, or create a draft to [forward](../api/message-createforward.md), [reply](../api/message-createreply.md) and [reply-all](../api/message-createreplyall.md) to an existing message.</span></span>

## <a name="permissions"></a><span data-ttu-id="551f3-115">权限</span><span class="sxs-lookup"><span data-stu-id="551f3-115">Permissions</span></span>
<span data-ttu-id="551f3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="551f3-p101">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="551f3-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="551f3-118">Permission type</span></span>      | <span data-ttu-id="551f3-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="551f3-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="551f3-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="551f3-120">Delegated (work or school account)</span></span> | <span data-ttu-id="551f3-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="551f3-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="551f3-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="551f3-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="551f3-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="551f3-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="551f3-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="551f3-124">Application</span></span> | <span data-ttu-id="551f3-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="551f3-125">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="551f3-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="551f3-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="551f3-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="551f3-127">Request headers</span></span>
| <span data-ttu-id="551f3-128">名称</span><span class="sxs-lookup"><span data-stu-id="551f3-128">Name</span></span>       | <span data-ttu-id="551f3-129">类型</span><span class="sxs-lookup"><span data-stu-id="551f3-129">Type</span></span> | <span data-ttu-id="551f3-130">说明</span><span class="sxs-lookup"><span data-stu-id="551f3-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="551f3-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="551f3-131">Authorization</span></span>  | <span data-ttu-id="551f3-132">string</span><span class="sxs-lookup"><span data-stu-id="551f3-132">string</span></span>  | <span data-ttu-id="551f3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="551f3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="551f3-135">Content-Length</span><span class="sxs-lookup"><span data-stu-id="551f3-135">Content-Length</span></span> | <span data-ttu-id="551f3-136">number</span><span class="sxs-lookup"><span data-stu-id="551f3-136">number</span></span> | <span data-ttu-id="551f3-137">0。必需。</span><span class="sxs-lookup"><span data-stu-id="551f3-137">0. Required.</span></span> |
| <span data-ttu-id="551f3-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="551f3-138">Content-Type</span></span> | <span data-ttu-id="551f3-139">string</span><span class="sxs-lookup"><span data-stu-id="551f3-139">string</span></span>  | <span data-ttu-id="551f3-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="551f3-p103">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="551f3-142">对 JSON 对象使用 `application/json`，对 MIME 内容使用 `text/plain`。</span><span class="sxs-lookup"><span data-stu-id="551f3-142">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="551f3-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="551f3-143">Request body</span></span>
<span data-ttu-id="551f3-144">使用 JSON 格式时，请提供[消息](../resources/message.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="551f3-144">When using JSON format, provide a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="551f3-145">当指定 MIME 格式的正文时，请提供 MIME 内容与适用的 Internet 邮件头（“收件人”、“抄送”、“密件抄送”、“主题”）所有内容在请求正文中编码为 **base64** 格式。</span><span class="sxs-lookup"><span data-stu-id="551f3-145">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

<span data-ttu-id="551f3-146">由于 **邮件** 资源支持 [扩展](/graph/extensibility-overview)因此可以使用 `POST` 操作，并在创建邮件时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="551f3-146">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="551f3-147">响应</span><span class="sxs-lookup"><span data-stu-id="551f3-147">Response</span></span>

<span data-ttu-id="551f3-148">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="551f3-148">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="551f3-149">如果请求正文包含错误的 MIME 内容，此方法将返回 `400 Bad request` 和以下错误消息：“无效的 base64 字符串 MIME 内容”。</span><span class="sxs-lookup"><span data-stu-id="551f3-149">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="551f3-150">示例</span><span class="sxs-lookup"><span data-stu-id="551f3-150">Examples</span></span>
### <a name="example-1-create-a-new-message-draft-using-json-format"></a><span data-ttu-id="551f3-151">示例 1：使用 JSON 格式创建新邮件草稿</span><span class="sxs-lookup"><span data-stu-id="551f3-151">Example 1: Create a new message draft using JSON format</span></span>
#### <a name="request"></a><span data-ttu-id="551f3-152">请求</span><span class="sxs-lookup"><span data-stu-id="551f3-152">Request</span></span> 
<span data-ttu-id="551f3-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="551f3-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="551f3-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="551f3-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: application/json

{
    "subject":"Did you see last night's game?",
    "importance":"Low",
    "body":{
        "contentType":"HTML",
        "content":"They were <b>awesome</b>!"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="551f3-155">C#</span><span class="sxs-lookup"><span data-stu-id="551f3-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="551f3-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="551f3-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="551f3-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="551f3-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="551f3-158">Java</span><span class="sxs-lookup"><span data-stu-id="551f3-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="551f3-159">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="551f3-159">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="551f3-160">响应</span><span class="sxs-lookup"><span data-stu-id="551f3-160">Response</span></span> 
<span data-ttu-id="551f3-p104">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="551f3-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti\"",
    "id":"AAMkADNlNYjSAAA=",
    "createdDateTime":"2017-07-22T01:53:56Z",
    "lastModifiedDateTime":"2017-07-22T01:53:57Z",
    "changeKey":"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti",
    "categories":[

    ],
    "receivedDateTime":"2017-07-22T01:53:57Z",
    "sentDateTime":"2017-07-22T01:53:57Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB@MWHPR1301MB.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkADNlNWAAAAAAEPAAA=",
    "conversationId":"AAQkADNlNFdXGBnqtY=",
    "conversationIndex":"AQHTe7/VAniOJVgCxEmtF1z6ZY1rFQ==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADNlNYjSAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ]
}
```

### <a name="example-2-create-message-draft-that-includes-custom-message-headers"></a><span data-ttu-id="551f3-163">示例 2：创建包含自定义邮件头的邮件草稿</span><span class="sxs-lookup"><span data-stu-id="551f3-163">Example 2: Create message draft that includes custom message headers</span></span>
#### <a name="request"></a><span data-ttu-id="551f3-164">请求</span><span class="sxs-lookup"><span data-stu-id="551f3-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="551f3-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="551f3-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: application/json

{
    "subject":"9/8/2018: concert",
    "body":{
        "contentType":"HTML",
        "content":"The group represents Washington."
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "internetMessageHeaders":[
        {
            "name":"x-custom-header-group-name",
            "value":"Washington"
        },
        {
            "name":"x-custom-header-group-id",
            "value":"WA001"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="551f3-166">C#</span><span class="sxs-lookup"><span data-stu-id="551f3-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-headers-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="551f3-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="551f3-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-headers-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="551f3-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="551f3-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-headers-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="551f3-169">Java</span><span class="sxs-lookup"><span data-stu-id="551f3-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-headers-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="551f3-170">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="551f3-170">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="551f3-171">响应</span><span class="sxs-lookup"><span data-stu-id="551f3-171">Response</span></span>
<span data-ttu-id="551f3-172">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="551f3-172">Here is an example of the response.</span></span> <span data-ttu-id="551f3-173">注意：默认情况下，POST 响应中不会返回 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="551f3-173">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="551f3-174">为简洁起见，也可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="551f3-174">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="551f3-175">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="551f3-175">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_with_headers_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE\"",
    "id":"AAMkADhNmAAA=",
    "createdDateTime":"2018-09-09T02:54:56Z",
    "lastModifiedDateTime":"2018-09-09T02:54:56Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T02:54:56Z",
    "sentDateTime":"2018-09-09T02:54:56Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR220MB1120.namprd22.prod.outlook.com>",
    "subject":"9/8/2018: concert",
    "bodyPreview":"The group represents Washington.",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEPAAA=",
    "conversationId":"AAQkADhNCuP8OKSm-0NE=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhNmAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Washington.\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

### <a name="example-3-create-a-new-message-draft-using-mime-format"></a><span data-ttu-id="551f3-176">示例 3：使用 MIME 格式创建新邮件草稿</span><span class="sxs-lookup"><span data-stu-id="551f3-176">Example 3: Create a new message draft using MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="551f3-177">请求</span><span class="sxs-lookup"><span data-stu-id="551f3-177">Request</span></span>


<!-- {
  "blockType": "ignored",
  "name": "message_create_draft_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np...

```


#### <a name="response"></a><span data-ttu-id="551f3-178">响应</span><span class="sxs-lookup"><span data-stu-id="551f3-178">Response</span></span>
<span data-ttu-id="551f3-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="551f3-179">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.message",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('0aaa0aa0-0000-0a00-a00a-0000009000a0')/messages/$entity",
    "@odata.etag": "W/\"AAAAAAAAAAAa00AAAa0aAaAa0a0AAAaAAAAaAa0a\"",
    "id": "AAMkADA1MTAAAAqldOAAA=",
    "createdDateTime": "2021-04-23T18:13:44Z",
    "lastModifiedDateTime": "2021-04-23T18:13:44Z",
    "changeKey": "AAAAAAAAAAAA00aaaa000aaA",
    "categories": [],
    "receivedDateTime": "2021-04-23T18:13:44Z",
    "sentDateTime": "2021-02-28T07:15:00Z",
    "hasAttachments": false,
    "internetMessageId": "<AAAAAAAAAA@AAAAAAA0001AA0000.codcod00.prod.outlook.com>",
    "subject": "Internal Resume Submission: Sales Associate",
    "bodyPreview": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here...",
    "importance": "normal",
    "parentFolderId": "LKJDSKJHkjhfakKJHFKWKKJHKJdhkjHDK==",
    "conversationId": "SDSFSmFSDGI5LWZhYjc4fsdfsd=",
    "conversationIndex": "Adfsdfsdfsdfw==",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": true,
    "isDraft": true,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkAGNhOWAvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "body": {
        "contentType": "text",
        "content": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here... Regards,Alex"
    },
    "sender": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    }
}

```

<span data-ttu-id="551f3-180">如果请求正文包含错误的 MIME 内容，此方法返回以下错误消息。</span><span class="sxs-lookup"><span data-stu-id="551f3-180">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 400 Bad Request
Content-type: application/json

{
    "error": {
        "code": "ErrorMimeContentInvalidBase64String",
        "message": "Invalid base64 string for MIME content."
    }
}
```

## <a name="see-also"></a><span data-ttu-id="551f3-181">另请参阅</span><span class="sxs-lookup"><span data-stu-id="551f3-181">See also</span></span>

- [<span data-ttu-id="551f3-182">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="551f3-182">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="551f3-183">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="551f3-183">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

