---
title: 'message: createReply'
description: 创建回复的草稿以指定邮件。 然后，可以更新草稿，将回复内容添加到**正文**，或更改其他邮件属性，或者仅发送草稿。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 85b88669ba7852150d6311ea22b0ab42bc29b29b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274926"
---
# <a name="message-createreply"></a><span data-ttu-id="1cbf2-104">message: createReply</span><span class="sxs-lookup"><span data-stu-id="1cbf2-104">message: createReply</span></span>

<span data-ttu-id="1cbf2-105">创建回复的草稿以指定[邮件](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="1cbf2-105">Create a draft of the reply to the specified [message](../resources/message.md).</span></span> <span data-ttu-id="1cbf2-106">然后，可以[更新](../api/message-update.md)草稿，将回复内容添加到**正文**，或更改其他邮件属性，或者仅[发送](../api/message-send.md)草稿。</span><span class="sxs-lookup"><span data-stu-id="1cbf2-106">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cbf2-107">权限</span><span class="sxs-lookup"><span data-stu-id="1cbf2-107">Permissions</span></span>
<span data-ttu-id="1cbf2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1cbf2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cbf2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1cbf2-110">Permission type</span></span>      | <span data-ttu-id="1cbf2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1cbf2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cbf2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1cbf2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1cbf2-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cbf2-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1cbf2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1cbf2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cbf2-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cbf2-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1cbf2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1cbf2-116">Application</span></span> | <span data-ttu-id="1cbf2-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cbf2-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cbf2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1cbf2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="1cbf2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1cbf2-119">Request headers</span></span>
| <span data-ttu-id="1cbf2-120">名称</span><span class="sxs-lookup"><span data-stu-id="1cbf2-120">Name</span></span>       | <span data-ttu-id="1cbf2-121">类型</span><span class="sxs-lookup"><span data-stu-id="1cbf2-121">Type</span></span> | <span data-ttu-id="1cbf2-122">说明</span><span class="sxs-lookup"><span data-stu-id="1cbf2-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1cbf2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cbf2-123">Authorization</span></span>  | <span data-ttu-id="1cbf2-124">string</span><span class="sxs-lookup"><span data-stu-id="1cbf2-124">string</span></span>  | <span data-ttu-id="1cbf2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1cbf2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cbf2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1cbf2-127">Request body</span></span>
<span data-ttu-id="1cbf2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1cbf2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cbf2-129">响应</span><span class="sxs-lookup"><span data-stu-id="1cbf2-129">Response</span></span>

<span data-ttu-id="1cbf2-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1cbf2-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cbf2-131">示例</span><span class="sxs-lookup"><span data-stu-id="1cbf2-131">Example</span></span>
<span data-ttu-id="1cbf2-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1cbf2-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1cbf2-133">请求</span><span class="sxs-lookup"><span data-stu-id="1cbf2-133">Request</span></span>
<span data-ttu-id="1cbf2-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1cbf2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReply
```

##### <a name="response"></a><span data-ttu-id="1cbf2-135">响应</span><span class="sxs-lookup"><span data-stu-id="1cbf2-135">Response</span></span>
<span data-ttu-id="1cbf2-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1cbf2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1cbf2-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1cbf2-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1cbf2-140">C#</span><span class="sxs-lookup"><span data-stu-id="1cbf2-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_createreply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1cbf2-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="1cbf2-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_createreply-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1cbf2-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="1cbf2-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_createreply-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-createreply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-createreply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-createreply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
