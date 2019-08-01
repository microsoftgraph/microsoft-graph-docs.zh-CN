---
title: 消息：replyAll
description: 答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a5a285becea0fd351011e8d74cfbcb5d70fd2e84
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022857"
---
# <a name="message-replyall"></a><span data-ttu-id="a3ede-104">消息：replyAll</span><span class="sxs-lookup"><span data-stu-id="a3ede-104">message: replyAll</span></span>

<span data-ttu-id="a3ede-p102">答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="a3ede-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3ede-107">权限</span><span class="sxs-lookup"><span data-stu-id="a3ede-107">Permissions</span></span>
<span data-ttu-id="a3ede-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3ede-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3ede-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3ede-110">Permission type</span></span>      | <span data-ttu-id="a3ede-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3ede-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3ede-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3ede-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a3ede-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a3ede-113">Mail.Send</span></span>    |
|<span data-ttu-id="a3ede-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3ede-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3ede-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a3ede-115">Mail.Send</span></span>    |
|<span data-ttu-id="a3ede-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3ede-116">Application</span></span> | <span data-ttu-id="a3ede-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="a3ede-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3ede-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3ede-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="a3ede-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3ede-119">Request headers</span></span>
| <span data-ttu-id="a3ede-120">名称</span><span class="sxs-lookup"><span data-stu-id="a3ede-120">Name</span></span>       | <span data-ttu-id="a3ede-121">类型</span><span class="sxs-lookup"><span data-stu-id="a3ede-121">Type</span></span> | <span data-ttu-id="a3ede-122">说明</span><span class="sxs-lookup"><span data-stu-id="a3ede-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3ede-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3ede-123">Authorization</span></span>  | <span data-ttu-id="a3ede-124">string</span><span class="sxs-lookup"><span data-stu-id="a3ede-124">string</span></span>  | <span data-ttu-id="a3ede-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3ede-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a3ede-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3ede-127">Content-Type</span></span> | <span data-ttu-id="a3ede-128">string</span><span class="sxs-lookup"><span data-stu-id="a3ede-128">string</span></span>  | <span data-ttu-id="a3ede-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="a3ede-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3ede-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3ede-131">Request body</span></span>
<span data-ttu-id="a3ede-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a3ede-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a3ede-133">参数</span><span class="sxs-lookup"><span data-stu-id="a3ede-133">Parameter</span></span>    | <span data-ttu-id="a3ede-134">类型</span><span class="sxs-lookup"><span data-stu-id="a3ede-134">Type</span></span>   |<span data-ttu-id="a3ede-135">说明</span><span class="sxs-lookup"><span data-stu-id="a3ede-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3ede-136">注释</span><span class="sxs-lookup"><span data-stu-id="a3ede-136">comment</span></span>|<span data-ttu-id="a3ede-137">String</span><span class="sxs-lookup"><span data-stu-id="a3ede-137">String</span></span>|<span data-ttu-id="a3ede-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="a3ede-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="a3ede-140">响应</span><span class="sxs-lookup"><span data-stu-id="a3ede-140">Response</span></span>

<span data-ttu-id="a3ede-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a3ede-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3ede-143">示例</span><span class="sxs-lookup"><span data-stu-id="a3ede-143">Example</span></span>
<span data-ttu-id="a3ede-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a3ede-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a3ede-145">请求</span><span class="sxs-lookup"><span data-stu-id="a3ede-145">Request</span></span>
<span data-ttu-id="a3ede-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3ede-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a3ede-147">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a3ede-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3ede-148">C#</span><span class="sxs-lookup"><span data-stu-id="a3ede-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3ede-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3ede-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3ede-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="a3ede-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3ede-151">Java</span><span class="sxs-lookup"><span data-stu-id="a3ede-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="a3ede-152">响应</span><span class="sxs-lookup"><span data-stu-id="a3ede-152">Response</span></span>
<span data-ttu-id="a3ede-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a3ede-153">Here is an example of the response.</span></span>
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
