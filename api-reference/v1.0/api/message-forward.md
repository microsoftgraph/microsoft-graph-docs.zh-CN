---
title: 邮件：转发
description: 转发邮件。邮件保存在已发送邮件文件夹中。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bf50b58b215eb4ec277c79d15c89e159882ee831
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128384"
---
# <a name="message-forward"></a><span data-ttu-id="ebb46-104">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="ebb46-104">message: forward</span></span>

<span data-ttu-id="ebb46-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebb46-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ebb46-p102">转发邮件。邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="ebb46-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebb46-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="ebb46-108">Permissions</span></span>
<span data-ttu-id="ebb46-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebb46-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebb46-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebb46-111">Permission type</span></span>      | <span data-ttu-id="ebb46-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebb46-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebb46-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebb46-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ebb46-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ebb46-114">Mail.Send</span></span>    |
|<span data-ttu-id="ebb46-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebb46-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebb46-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ebb46-116">Mail.Send</span></span>    |
|<span data-ttu-id="ebb46-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebb46-117">Application</span></span> | <span data-ttu-id="ebb46-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ebb46-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebb46-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebb46-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="ebb46-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebb46-120">Request headers</span></span>
| <span data-ttu-id="ebb46-121">名称</span><span class="sxs-lookup"><span data-stu-id="ebb46-121">Name</span></span>       | <span data-ttu-id="ebb46-122">类型</span><span class="sxs-lookup"><span data-stu-id="ebb46-122">Type</span></span> | <span data-ttu-id="ebb46-123">说明</span><span class="sxs-lookup"><span data-stu-id="ebb46-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ebb46-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebb46-124">Authorization</span></span>  | <span data-ttu-id="ebb46-125">string</span><span class="sxs-lookup"><span data-stu-id="ebb46-125">string</span></span>  | <span data-ttu-id="ebb46-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebb46-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebb46-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebb46-128">Content-Type</span></span> | <span data-ttu-id="ebb46-129">string</span><span class="sxs-lookup"><span data-stu-id="ebb46-129">string</span></span>  | <span data-ttu-id="ebb46-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="ebb46-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebb46-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebb46-132">Request body</span></span>
<span data-ttu-id="ebb46-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ebb46-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ebb46-134">参数</span><span class="sxs-lookup"><span data-stu-id="ebb46-134">Parameter</span></span>    | <span data-ttu-id="ebb46-135">类型</span><span class="sxs-lookup"><span data-stu-id="ebb46-135">Type</span></span>   |<span data-ttu-id="ebb46-136">说明</span><span class="sxs-lookup"><span data-stu-id="ebb46-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebb46-137">注释</span><span class="sxs-lookup"><span data-stu-id="ebb46-137">comment</span></span>|<span data-ttu-id="ebb46-138">String</span><span class="sxs-lookup"><span data-stu-id="ebb46-138">String</span></span>|<span data-ttu-id="ebb46-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="ebb46-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="ebb46-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="ebb46-141">toRecipients</span></span>|<span data-ttu-id="ebb46-142">[Recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="ebb46-142">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="ebb46-143">收件人列表</span><span class="sxs-lookup"><span data-stu-id="ebb46-143">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="ebb46-144">响应</span><span class="sxs-lookup"><span data-stu-id="ebb46-144">Response</span></span>

<span data-ttu-id="ebb46-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ebb46-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebb46-147">示例</span><span class="sxs-lookup"><span data-stu-id="ebb46-147">Example</span></span>
<span data-ttu-id="ebb46-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ebb46-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ebb46-149">请求</span><span class="sxs-lookup"><span data-stu-id="ebb46-149">Request</span></span>
<span data-ttu-id="ebb46-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebb46-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebb46-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebb46-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ebb46-152">C#</span><span class="sxs-lookup"><span data-stu-id="ebb46-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebb46-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebb46-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebb46-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebb46-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebb46-155">Java</span><span class="sxs-lookup"><span data-stu-id="ebb46-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ebb46-156">响应</span><span class="sxs-lookup"><span data-stu-id="ebb46-156">Response</span></span>
##### <a name="response"></a><span data-ttu-id="ebb46-157">响应</span><span class="sxs-lookup"><span data-stu-id="ebb46-157">Response</span></span>
<span data-ttu-id="ebb46-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ebb46-158">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

