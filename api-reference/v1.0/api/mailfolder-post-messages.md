---
title: 创建邮件
description: 使用此 API 在 mailfolder 中新建邮件。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a50d222830aeee573c4c7b5824ce2ccee9e9c7de
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055916"
---
# <a name="create-message"></a><span data-ttu-id="0ec93-103">创建邮件</span><span class="sxs-lookup"><span data-stu-id="0ec93-103">Create Message</span></span>

<span data-ttu-id="0ec93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ec93-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0ec93-105">使用此 API 在 mailfolder 中新建邮件。</span><span class="sxs-lookup"><span data-stu-id="0ec93-105">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ec93-106">权限</span><span class="sxs-lookup"><span data-stu-id="0ec93-106">Permissions</span></span>
<span data-ttu-id="0ec93-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ec93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ec93-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ec93-109">Permission type</span></span>      | <span data-ttu-id="0ec93-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ec93-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ec93-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ec93-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ec93-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ec93-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0ec93-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ec93-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ec93-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ec93-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0ec93-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ec93-115">Application</span></span> | <span data-ttu-id="0ec93-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ec93-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ec93-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ec93-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="0ec93-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ec93-118">Request headers</span></span>
| <span data-ttu-id="0ec93-119">标头</span><span class="sxs-lookup"><span data-stu-id="0ec93-119">Header</span></span>       | <span data-ttu-id="0ec93-120">值</span><span class="sxs-lookup"><span data-stu-id="0ec93-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0ec93-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ec93-121">Authorization</span></span>  | <span data-ttu-id="0ec93-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ec93-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0ec93-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ec93-124">Content-Type</span></span>  | <span data-ttu-id="0ec93-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0ec93-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0ec93-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ec93-127">Request body</span></span>
<span data-ttu-id="0ec93-128">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ec93-128">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0ec93-129">响应</span><span class="sxs-lookup"><span data-stu-id="0ec93-129">Response</span></span>

<span data-ttu-id="0ec93-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ec93-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ec93-131">示例</span><span class="sxs-lookup"><span data-stu-id="0ec93-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ec93-132">请求</span><span class="sxs-lookup"><span data-stu-id="0ec93-132">Request</span></span>
<span data-ttu-id="0ec93-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ec93-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0ec93-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ec93-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
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
# <a name="c"></a>[<span data-ttu-id="0ec93-135">C#</span><span class="sxs-lookup"><span data-stu-id="0ec93-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ec93-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ec93-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ec93-137">Java</span><span class="sxs-lookup"><span data-stu-id="0ec93-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0ec93-138">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ec93-138">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0ec93-139">响应</span><span class="sxs-lookup"><span data-stu-id="0ec93-139">Response</span></span>
<span data-ttu-id="0ec93-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0ec93-140">Here is an example of the response.</span></span> <span data-ttu-id="0ec93-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ec93-141">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

