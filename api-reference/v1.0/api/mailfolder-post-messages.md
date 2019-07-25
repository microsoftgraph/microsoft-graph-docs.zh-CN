---
title: 创建邮件
description: 使用此 API 在 mailfolder 中新建邮件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8e5598fc3d56aa753e35bbe393ed166eae7daba9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856343"
---
# <a name="create-message"></a><span data-ttu-id="48267-103">创建邮件</span><span class="sxs-lookup"><span data-stu-id="48267-103">Create Message</span></span>

<span data-ttu-id="48267-104">使用此 API 在 mailfolder 中新建邮件。</span><span class="sxs-lookup"><span data-stu-id="48267-104">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="48267-105">权限</span><span class="sxs-lookup"><span data-stu-id="48267-105">Permissions</span></span>
<span data-ttu-id="48267-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48267-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48267-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="48267-108">Permission type</span></span>      | <span data-ttu-id="48267-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48267-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48267-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48267-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48267-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48267-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="48267-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48267-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48267-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48267-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="48267-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="48267-114">Application</span></span> | <span data-ttu-id="48267-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48267-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="48267-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48267-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="48267-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="48267-117">Request headers</span></span>
| <span data-ttu-id="48267-118">标头</span><span class="sxs-lookup"><span data-stu-id="48267-118">Header</span></span>       | <span data-ttu-id="48267-119">值</span><span class="sxs-lookup"><span data-stu-id="48267-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="48267-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="48267-120">Authorization</span></span>  | <span data-ttu-id="48267-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="48267-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48267-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48267-123">Content-Type</span></span>  | <span data-ttu-id="48267-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="48267-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="48267-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="48267-126">Request body</span></span>
<span data-ttu-id="48267-127">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48267-127">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="48267-128">响应</span><span class="sxs-lookup"><span data-stu-id="48267-128">Response</span></span>

<span data-ttu-id="48267-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="48267-129">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48267-130">示例</span><span class="sxs-lookup"><span data-stu-id="48267-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48267-131">请求</span><span class="sxs-lookup"><span data-stu-id="48267-131">Request</span></span>
<span data-ttu-id="48267-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48267-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48267-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="48267-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="48267-134">C#</span><span class="sxs-lookup"><span data-stu-id="48267-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48267-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="48267-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="48267-136">Java</span><span class="sxs-lookup"><span data-stu-id="48267-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="48267-137">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48267-137">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="48267-138">响应</span><span class="sxs-lookup"><span data-stu-id="48267-138">Response</span></span>
<span data-ttu-id="48267-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48267-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
