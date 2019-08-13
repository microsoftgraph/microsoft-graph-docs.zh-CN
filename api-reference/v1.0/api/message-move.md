---
title: 'message: move'
description: 将邮件移动到文件夹。 该操作会在目标文件夹中创建邮件的新副本并删除原始邮件。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e51deede6ff3f05cc0f9c4549975a3c46bf56356
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374720"
---
# <a name="message-move"></a><span data-ttu-id="7590d-104">message: move</span><span class="sxs-lookup"><span data-stu-id="7590d-104">message: move</span></span>

<span data-ttu-id="7590d-105">将邮件移动到文件夹。</span><span class="sxs-lookup"><span data-stu-id="7590d-105">Move a message to a folder.</span></span> <span data-ttu-id="7590d-106">该操作会在目标文件夹中创建邮件的新副本并删除原始邮件。</span><span class="sxs-lookup"><span data-stu-id="7590d-106">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="7590d-107">权限</span><span class="sxs-lookup"><span data-stu-id="7590d-107">Permissions</span></span>

<span data-ttu-id="7590d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7590d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7590d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7590d-110">Permission type</span></span> | <span data-ttu-id="7590d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7590d-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="7590d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7590d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7590d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7590d-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7590d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7590d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7590d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7590d-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7590d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7590d-116">Application</span></span> | <span data-ttu-id="7590d-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7590d-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7590d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7590d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="7590d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7590d-119">Request headers</span></span>

| <span data-ttu-id="7590d-120">标头</span><span class="sxs-lookup"><span data-stu-id="7590d-120">Header</span></span> | <span data-ttu-id="7590d-121">值</span><span class="sxs-lookup"><span data-stu-id="7590d-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="7590d-122">授权</span><span class="sxs-lookup"><span data-stu-id="7590d-122">Authorization</span></span> | <span data-ttu-id="7590d-123">`Bearer {token}`（）。</span><span class="sxs-lookup"><span data-stu-id="7590d-123">`Bearer {token}`.</span></span> <span data-ttu-id="7590d-124">必需。</span><span class="sxs-lookup"><span data-stu-id="7590d-124">Required.</span></span> |
| <span data-ttu-id="7590d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7590d-125">Content-Type</span></span> | <span data-ttu-id="7590d-126">`application/json`（）。</span><span class="sxs-lookup"><span data-stu-id="7590d-126">`application/json`.</span></span> <span data-ttu-id="7590d-127">必需。</span><span class="sxs-lookup"><span data-stu-id="7590d-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7590d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7590d-128">Request body</span></span>

<span data-ttu-id="7590d-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7590d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7590d-130">参数</span><span class="sxs-lookup"><span data-stu-id="7590d-130">Parameter</span></span>   | <span data-ttu-id="7590d-131">类型</span><span class="sxs-lookup"><span data-stu-id="7590d-131">Type</span></span> |<span data-ttu-id="7590d-132">说明</span><span class="sxs-lookup"><span data-stu-id="7590d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7590d-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="7590d-133">destinationId</span></span>|<span data-ttu-id="7590d-134">String</span><span class="sxs-lookup"><span data-stu-id="7590d-134">String</span></span>|<span data-ttu-id="7590d-135">目标文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="7590d-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="7590d-136">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="7590d-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="7590d-137">响应</span><span class="sxs-lookup"><span data-stu-id="7590d-137">Response</span></span>

<span data-ttu-id="7590d-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="7590d-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7590d-139">示例</span><span class="sxs-lookup"><span data-stu-id="7590d-139">Example</span></span>

<span data-ttu-id="7590d-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7590d-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7590d-141">请求</span><span class="sxs-lookup"><span data-stu-id="7590d-141">Request</span></span>

<span data-ttu-id="7590d-142">以下请求会将制定邮件移至“已删除邮件”文件夹，由其已知文件夹名称 `deleteditems` 标识。</span><span class="sxs-lookup"><span data-stu-id="7590d-142">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7590d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="7590d-143">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7590d-144">C#</span><span class="sxs-lookup"><span data-stu-id="7590d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-move-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7590d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7590d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-move-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7590d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7590d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-move-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7590d-147">Java</span><span class="sxs-lookup"><span data-stu-id="7590d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-move-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7590d-148">响应</span><span class="sxs-lookup"><span data-stu-id="7590d-148">Response</span></span>

<span data-ttu-id="7590d-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7590d-149">Here is an example of the response.</span></span>

> <span data-ttu-id="7590d-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7590d-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7590d-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7590d-151">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#message",
    "@odata.type":"#microsoft.graph.message",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "createdDateTime":"2018-08-12T08:43:22Z",
    "lastModifiedDateTime":"2018-08-15T19:47:54Z",
    "changeKey":"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB",
    "categories":[

    ],
    "receivedDateTime":"2018-08-12T08:43:22Z",
    "sentDateTime":"2018-08-12T08:43:20Z",
    "hasAttachments":false,
    "internetMessageId":"<00535324-5988-4b6a-b9af-d44cf2d0b691@MWHPR2201MB1022.namprd22.prod.outlook.com>",
    "subject":"Undeliverable: Meet for lunch?",
    "bodyPreview":"Delivery has failed to these recipients or groups:\r\n\r\nfannyd@contoso.onmicrosoft.com (fannyd@contoso.onmicrosoft.com)\r\nYour message couldn't be delivered. Despite repeated attempts to deliver your message, querying the Domain Name System (DNS) for the rec",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEKAAA=",
    "conversationId":"AAQkADhJzfbkARFhe5kKhjihSA=",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhAAAW%2FVPeAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html></html>"
    },
    "sender":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"fannyd@contoso.onmicrosoft.com",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        },
        {
            "emailAddress":{
                "name":"danas@contoso.onmicrosoft.com",
                "address":"danas@contoso.onmicrosoft.com"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
