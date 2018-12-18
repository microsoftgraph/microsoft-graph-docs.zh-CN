---
title: 'message: move'
description: 将邮件移动到文件夹中。 此目标文件夹中创建新邮件的副本，并删除原始邮件。
author: angelgolfer-ms
ms.openlocfilehash: 46f62d8793a20db41d19c1677b3d6f48aa7dbd14
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311695"
---
# <a name="message-move"></a><span data-ttu-id="cc709-104">message: move</span><span class="sxs-lookup"><span data-stu-id="cc709-104">message: move</span></span>

> <span data-ttu-id="cc709-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cc709-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc709-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc709-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc709-107">将邮件移动到文件夹中。</span><span class="sxs-lookup"><span data-stu-id="cc709-107">Move a message to a folder.</span></span> <span data-ttu-id="cc709-108">此目标文件夹中创建新邮件的副本，并删除原始邮件。</span><span class="sxs-lookup"><span data-stu-id="cc709-108">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc709-109">权限</span><span class="sxs-lookup"><span data-stu-id="cc709-109">Permissions</span></span>

<span data-ttu-id="cc709-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc709-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc709-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc709-112">Permission type</span></span> | <span data-ttu-id="cc709-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc709-113">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="cc709-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc709-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cc709-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc709-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cc709-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc709-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc709-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc709-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cc709-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc709-118">Application</span></span> | <span data-ttu-id="cc709-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc709-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc709-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc709-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="cc709-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc709-121">Request headers</span></span>

| <span data-ttu-id="cc709-122">标头</span><span class="sxs-lookup"><span data-stu-id="cc709-122">Header</span></span> | <span data-ttu-id="cc709-123">值</span><span class="sxs-lookup"><span data-stu-id="cc709-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="cc709-124">授权</span><span class="sxs-lookup"><span data-stu-id="cc709-124">Authorization</span></span> | <span data-ttu-id="cc709-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="cc709-125"></span></span> <span data-ttu-id="cc709-126">必需。</span><span class="sxs-lookup"><span data-stu-id="cc709-126">Required.</span></span> |
| <span data-ttu-id="cc709-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc709-127">Content-Type</span></span> | <span data-ttu-id="cc709-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="cc709-128"></span></span> <span data-ttu-id="cc709-129">必需。</span><span class="sxs-lookup"><span data-stu-id="cc709-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc709-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc709-130">Request body</span></span>

<span data-ttu-id="cc709-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cc709-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cc709-132">参数</span><span class="sxs-lookup"><span data-stu-id="cc709-132">Parameter</span></span>   | <span data-ttu-id="cc709-133">Type</span><span class="sxs-lookup"><span data-stu-id="cc709-133">Type</span></span> |<span data-ttu-id="cc709-134">说明</span><span class="sxs-lookup"><span data-stu-id="cc709-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc709-135">DestinationId</span><span class="sxs-lookup"><span data-stu-id="cc709-135">DestinationId</span></span>|<span data-ttu-id="cc709-136">String</span><span class="sxs-lookup"><span data-stu-id="cc709-136">String</span></span>|<span data-ttu-id="cc709-137">目标文件夹 ID 或已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="cc709-137">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="cc709-138">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="cc709-138">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="cc709-139">响应</span><span class="sxs-lookup"><span data-stu-id="cc709-139">Response</span></span>

<span data-ttu-id="cc709-140">如果成功，此方法返回`201 Created`响应代码和响应正文的[邮件](../resources/message.md)资源。</span><span class="sxs-lookup"><span data-stu-id="cc709-140">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc709-141">示例</span><span class="sxs-lookup"><span data-stu-id="cc709-141">Example</span></span>

<span data-ttu-id="cc709-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="cc709-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="cc709-143">请求</span><span class="sxs-lookup"><span data-stu-id="cc709-143">Request</span></span>

<span data-ttu-id="cc709-144">以下请求将指定的邮件移动到已删除邮件文件夹，由其已知文件夹名称标识`deleteditems`。</span><span class="sxs-lookup"><span data-stu-id="cc709-144">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
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

##### <a name="response"></a><span data-ttu-id="cc709-145">响应</span><span class="sxs-lookup"><span data-stu-id="cc709-145">Response</span></span>

<span data-ttu-id="cc709-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cc709-146">Here is an example of the response.</span></span>

> <span data-ttu-id="cc709-147">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cc709-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cc709-148">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cc709-148">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
