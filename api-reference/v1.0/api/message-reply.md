---
title: 消息：答复
description: 答复邮件发件人然后邮件保存在已发送邮件文件夹中。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7a65cf3e4313e89f9b9591e1551a18db2671f3e2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612519"
---
# <a name="message-reply"></a><span data-ttu-id="5bcdc-104">消息：答复</span><span class="sxs-lookup"><span data-stu-id="5bcdc-104">message: reply</span></span>

<span data-ttu-id="5bcdc-p102">答复邮件发件人然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="5bcdc-p102">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bcdc-107">权限</span><span class="sxs-lookup"><span data-stu-id="5bcdc-107">Permissions</span></span>
<span data-ttu-id="5bcdc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bcdc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bcdc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bcdc-110">Permission type</span></span>      | <span data-ttu-id="5bcdc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5bcdc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bcdc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bcdc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5bcdc-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5bcdc-113">Mail.Send</span></span>    |
|<span data-ttu-id="5bcdc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bcdc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bcdc-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5bcdc-115">Mail.Send</span></span>    |
|<span data-ttu-id="5bcdc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bcdc-116">Application</span></span> | <span data-ttu-id="5bcdc-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="5bcdc-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bcdc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bcdc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="5bcdc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bcdc-119">Request headers</span></span>
| <span data-ttu-id="5bcdc-120">名称</span><span class="sxs-lookup"><span data-stu-id="5bcdc-120">Name</span></span>       | <span data-ttu-id="5bcdc-121">类型</span><span class="sxs-lookup"><span data-stu-id="5bcdc-121">Type</span></span> | <span data-ttu-id="5bcdc-122">说明</span><span class="sxs-lookup"><span data-stu-id="5bcdc-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5bcdc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bcdc-123">Authorization</span></span>  | <span data-ttu-id="5bcdc-124">string</span><span class="sxs-lookup"><span data-stu-id="5bcdc-124">string</span></span>  | <span data-ttu-id="5bcdc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5bcdc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5bcdc-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5bcdc-127">Content-Type</span></span> | <span data-ttu-id="5bcdc-128">string</span><span class="sxs-lookup"><span data-stu-id="5bcdc-128">string</span></span>  | <span data-ttu-id="5bcdc-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="5bcdc-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bcdc-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bcdc-131">Request body</span></span>
<span data-ttu-id="5bcdc-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5bcdc-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5bcdc-133">参数</span><span class="sxs-lookup"><span data-stu-id="5bcdc-133">Parameter</span></span>    | <span data-ttu-id="5bcdc-134">类型</span><span class="sxs-lookup"><span data-stu-id="5bcdc-134">Type</span></span>   |<span data-ttu-id="5bcdc-135">说明</span><span class="sxs-lookup"><span data-stu-id="5bcdc-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bcdc-136">注释</span><span class="sxs-lookup"><span data-stu-id="5bcdc-136">comment</span></span>|<span data-ttu-id="5bcdc-137">String</span><span class="sxs-lookup"><span data-stu-id="5bcdc-137">String</span></span>|<span data-ttu-id="5bcdc-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="5bcdc-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="5bcdc-140">响应</span><span class="sxs-lookup"><span data-stu-id="5bcdc-140">Response</span></span>

<span data-ttu-id="5bcdc-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5bcdc-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bcdc-143">示例</span><span class="sxs-lookup"><span data-stu-id="5bcdc-143">Example</span></span>
<span data-ttu-id="5bcdc-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5bcdc-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5bcdc-145">请求</span><span class="sxs-lookup"><span data-stu-id="5bcdc-145">Request</span></span>
<span data-ttu-id="5bcdc-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5bcdc-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```

##### <a name="response"></a><span data-ttu-id="5bcdc-147">响应</span><span class="sxs-lookup"><span data-stu-id="5bcdc-147">Response</span></span>
##### <a name="response"></a><span data-ttu-id="5bcdc-148">响应</span><span class="sxs-lookup"><span data-stu-id="5bcdc-148">Response</span></span>
<span data-ttu-id="5bcdc-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5bcdc-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5bcdc-150">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5bcdc-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5bcdc-151">语言</span><span class="sxs-lookup"><span data-stu-id="5bcdc-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_reply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bcdc-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bcdc-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_reply-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-reply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-reply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
