---
title: 消息：replyAll
description: 答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 84fc604be0bb62c5d68268d3234eb5f0b48a84e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028600"
---
# <a name="message-replyall"></a><span data-ttu-id="68667-104">消息：replyAll</span><span class="sxs-lookup"><span data-stu-id="68667-104">message: replyAll</span></span>

<span data-ttu-id="68667-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68667-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68667-p102">答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="68667-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="68667-108">权限</span><span class="sxs-lookup"><span data-stu-id="68667-108">Permissions</span></span>
<span data-ttu-id="68667-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68667-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68667-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="68667-111">Permission type</span></span>      | <span data-ttu-id="68667-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68667-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68667-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68667-113">Delegated (work or school account)</span></span> | <span data-ttu-id="68667-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="68667-114">Mail.Send</span></span>    |
|<span data-ttu-id="68667-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68667-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68667-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="68667-116">Mail.Send</span></span>    |
|<span data-ttu-id="68667-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="68667-117">Application</span></span> | <span data-ttu-id="68667-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="68667-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="68667-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68667-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="68667-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="68667-120">Request headers</span></span>
| <span data-ttu-id="68667-121">名称</span><span class="sxs-lookup"><span data-stu-id="68667-121">Name</span></span>       | <span data-ttu-id="68667-122">类型</span><span class="sxs-lookup"><span data-stu-id="68667-122">Type</span></span> | <span data-ttu-id="68667-123">说明</span><span class="sxs-lookup"><span data-stu-id="68667-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="68667-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="68667-124">Authorization</span></span>  | <span data-ttu-id="68667-125">string</span><span class="sxs-lookup"><span data-stu-id="68667-125">string</span></span>  | <span data-ttu-id="68667-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68667-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="68667-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68667-128">Content-Type</span></span> | <span data-ttu-id="68667-129">string</span><span class="sxs-lookup"><span data-stu-id="68667-129">string</span></span>  | <span data-ttu-id="68667-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="68667-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68667-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="68667-132">Request body</span></span>
<span data-ttu-id="68667-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="68667-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="68667-134">参数</span><span class="sxs-lookup"><span data-stu-id="68667-134">Parameter</span></span>    | <span data-ttu-id="68667-135">类型</span><span class="sxs-lookup"><span data-stu-id="68667-135">Type</span></span>   |<span data-ttu-id="68667-136">说明</span><span class="sxs-lookup"><span data-stu-id="68667-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68667-137">注释</span><span class="sxs-lookup"><span data-stu-id="68667-137">comment</span></span>|<span data-ttu-id="68667-138">String</span><span class="sxs-lookup"><span data-stu-id="68667-138">String</span></span>|<span data-ttu-id="68667-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="68667-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="68667-141">响应</span><span class="sxs-lookup"><span data-stu-id="68667-141">Response</span></span>

<span data-ttu-id="68667-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="68667-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68667-144">示例</span><span class="sxs-lookup"><span data-stu-id="68667-144">Example</span></span>
<span data-ttu-id="68667-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="68667-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="68667-146">请求</span><span class="sxs-lookup"><span data-stu-id="68667-146">Request</span></span>
<span data-ttu-id="68667-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="68667-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="68667-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="68667-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```
# <a name="c"></a>[<span data-ttu-id="68667-149">C#</span><span class="sxs-lookup"><span data-stu-id="68667-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68667-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68667-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68667-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68667-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68667-152">Java</span><span class="sxs-lookup"><span data-stu-id="68667-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="68667-153">响应</span><span class="sxs-lookup"><span data-stu-id="68667-153">Response</span></span>
<span data-ttu-id="68667-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="68667-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

