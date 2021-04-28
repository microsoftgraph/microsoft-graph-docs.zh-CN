---
title: 'message: createReply'
description: 创建回复的草稿以指定邮件。 然后，可以更新草稿，将回复内容添加到 **正文**，或更改其他邮件属性，或者仅发送草稿。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 64d88663ca8dc0e4210f13ab33f6bb8168d6edc7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039438"
---
# <a name="message-createreply"></a><span data-ttu-id="6f1ee-104">message: createReply</span><span class="sxs-lookup"><span data-stu-id="6f1ee-104">message: createReply</span></span>

<span data-ttu-id="6f1ee-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f1ee-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f1ee-106">创建回复的草稿以指定[邮件](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="6f1ee-106">Create a draft of the reply to the specified [message](../resources/message.md).</span></span> <span data-ttu-id="6f1ee-107">然后，可以 [更新](../api/message-update.md)草稿，将回复内容添加到 **正文**，或更改其他邮件属性，或者仅 [发送](../api/message-send.md)草稿。</span><span class="sxs-lookup"><span data-stu-id="6f1ee-107">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f1ee-108">权限</span><span class="sxs-lookup"><span data-stu-id="6f1ee-108">Permissions</span></span>
<span data-ttu-id="6f1ee-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f1ee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f1ee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f1ee-111">Permission type</span></span>      | <span data-ttu-id="6f1ee-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f1ee-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f1ee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f1ee-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6f1ee-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f1ee-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6f1ee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f1ee-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f1ee-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f1ee-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6f1ee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f1ee-117">Application</span></span> | <span data-ttu-id="6f1ee-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f1ee-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f1ee-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f1ee-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="6f1ee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f1ee-120">Request headers</span></span>
| <span data-ttu-id="6f1ee-121">名称</span><span class="sxs-lookup"><span data-stu-id="6f1ee-121">Name</span></span>       | <span data-ttu-id="6f1ee-122">类型</span><span class="sxs-lookup"><span data-stu-id="6f1ee-122">Type</span></span> | <span data-ttu-id="6f1ee-123">说明</span><span class="sxs-lookup"><span data-stu-id="6f1ee-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6f1ee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f1ee-124">Authorization</span></span>  | <span data-ttu-id="6f1ee-125">string</span><span class="sxs-lookup"><span data-stu-id="6f1ee-125">string</span></span>  | <span data-ttu-id="6f1ee-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6f1ee-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f1ee-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f1ee-128">Request body</span></span>
<span data-ttu-id="6f1ee-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f1ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f1ee-130">响应</span><span class="sxs-lookup"><span data-stu-id="6f1ee-130">Response</span></span>

<span data-ttu-id="6f1ee-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6f1ee-131">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f1ee-132">示例</span><span class="sxs-lookup"><span data-stu-id="6f1ee-132">Example</span></span>
<span data-ttu-id="6f1ee-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6f1ee-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6f1ee-134">请求</span><span class="sxs-lookup"><span data-stu-id="6f1ee-134">Request</span></span>
<span data-ttu-id="6f1ee-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f1ee-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f1ee-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f1ee-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReply
```
# <a name="c"></a>[<span data-ttu-id="6f1ee-137">C#</span><span class="sxs-lookup"><span data-stu-id="6f1ee-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f1ee-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f1ee-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f1ee-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f1ee-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f1ee-140">Java</span><span class="sxs-lookup"><span data-stu-id="6f1ee-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6f1ee-141">响应</span><span class="sxs-lookup"><span data-stu-id="6f1ee-141">Response</span></span>
<span data-ttu-id="6f1ee-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6f1ee-142">Here is an example of the response.</span></span> <span data-ttu-id="6f1ee-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6f1ee-143">Note: The response object shown here might be shortened for readability.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

