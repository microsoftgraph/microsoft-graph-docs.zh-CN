---
title: 'message: move'
description: 将邮件移动到文件夹。 该操作会在目标文件夹中创建邮件的新副本并删除原始邮件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 77b78bafa1ffb02d74ea025704b98673bdab5b42
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266519"
---
# <a name="message-move"></a><span data-ttu-id="12612-104">message: move</span><span class="sxs-lookup"><span data-stu-id="12612-104">message: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12612-105">将邮件移动到文件夹。</span><span class="sxs-lookup"><span data-stu-id="12612-105">Move a message to a folder.</span></span> <span data-ttu-id="12612-106">该操作会在目标文件夹中创建邮件的新副本并删除原始邮件。</span><span class="sxs-lookup"><span data-stu-id="12612-106">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="12612-107">权限</span><span class="sxs-lookup"><span data-stu-id="12612-107">Permissions</span></span>

<span data-ttu-id="12612-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12612-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12612-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="12612-110">Permission type</span></span> | <span data-ttu-id="12612-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12612-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="12612-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12612-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12612-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12612-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="12612-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12612-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12612-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12612-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="12612-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="12612-116">Application</span></span> | <span data-ttu-id="12612-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12612-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="12612-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12612-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="12612-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="12612-119">Request headers</span></span>

| <span data-ttu-id="12612-120">标头</span><span class="sxs-lookup"><span data-stu-id="12612-120">Header</span></span> | <span data-ttu-id="12612-121">值</span><span class="sxs-lookup"><span data-stu-id="12612-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="12612-122">授权</span><span class="sxs-lookup"><span data-stu-id="12612-122">Authorization</span></span> | <span data-ttu-id="12612-123">`Bearer {token}`（）。</span><span class="sxs-lookup"><span data-stu-id="12612-123">`Bearer {token}`.</span></span> <span data-ttu-id="12612-124">必需。</span><span class="sxs-lookup"><span data-stu-id="12612-124">Required.</span></span> |
| <span data-ttu-id="12612-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12612-125">Content-Type</span></span> | <span data-ttu-id="12612-126">`application/json`（）。</span><span class="sxs-lookup"><span data-stu-id="12612-126">`application/json`.</span></span> <span data-ttu-id="12612-127">必需。</span><span class="sxs-lookup"><span data-stu-id="12612-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12612-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="12612-128">Request body</span></span>

<span data-ttu-id="12612-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="12612-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="12612-130">参数</span><span class="sxs-lookup"><span data-stu-id="12612-130">Parameter</span></span>   | <span data-ttu-id="12612-131">类型</span><span class="sxs-lookup"><span data-stu-id="12612-131">Type</span></span> |<span data-ttu-id="12612-132">说明</span><span class="sxs-lookup"><span data-stu-id="12612-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12612-133">DestinationId</span><span class="sxs-lookup"><span data-stu-id="12612-133">DestinationId</span></span>|<span data-ttu-id="12612-134">String</span><span class="sxs-lookup"><span data-stu-id="12612-134">String</span></span>|<span data-ttu-id="12612-135">目标文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="12612-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="12612-136">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="12612-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="12612-137">响应</span><span class="sxs-lookup"><span data-stu-id="12612-137">Response</span></span>

<span data-ttu-id="12612-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [message](../resources/message.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="12612-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12612-139">示例</span><span class="sxs-lookup"><span data-stu-id="12612-139">Example</span></span>

<span data-ttu-id="12612-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="12612-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="12612-141">请求</span><span class="sxs-lookup"><span data-stu-id="12612-141">Request</span></span>

<span data-ttu-id="12612-142">以下请求会将制定邮件移至“已删除邮件”文件夹，由其已知文件夹名称 `deleteditems` 标识。</span><span class="sxs-lookup"><span data-stu-id="12612-142">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```

##### <a name="response"></a><span data-ttu-id="12612-143">响应</span><span class="sxs-lookup"><span data-stu-id="12612-143">Response</span></span>

<span data-ttu-id="12612-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="12612-144">Here is an example of the response.</span></span>

> <span data-ttu-id="12612-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="12612-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="12612-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="12612-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#message",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="12612-147">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="12612-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="12612-148">C#</span><span class="sxs-lookup"><span data-stu-id="12612-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_move-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="12612-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="12612-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_move-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="12612-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="12612-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_move-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-move.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-move.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-move.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
