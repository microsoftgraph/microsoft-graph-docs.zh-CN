---
title: 创建邮件
description: 使用此 API 在 mailfolder 中新建邮件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b3e73c0d7e9d8355ef59ce2e5b35f36d06f651af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511598"
---
# <a name="create-message"></a><span data-ttu-id="97567-103">创建邮件</span><span class="sxs-lookup"><span data-stu-id="97567-103">Create Message</span></span>

<span data-ttu-id="97567-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97567-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97567-105">使用此 API 在 mailfolder 中新建邮件。</span><span class="sxs-lookup"><span data-stu-id="97567-105">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="97567-106">权限</span><span class="sxs-lookup"><span data-stu-id="97567-106">Permissions</span></span>
<span data-ttu-id="97567-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97567-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97567-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="97567-109">Permission type</span></span>      | <span data-ttu-id="97567-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97567-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97567-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97567-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97567-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97567-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="97567-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97567-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97567-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97567-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="97567-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="97567-115">Application</span></span> | <span data-ttu-id="97567-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97567-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="97567-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97567-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="97567-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="97567-118">Request headers</span></span>
| <span data-ttu-id="97567-119">标头</span><span class="sxs-lookup"><span data-stu-id="97567-119">Header</span></span>       | <span data-ttu-id="97567-120">值</span><span class="sxs-lookup"><span data-stu-id="97567-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97567-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="97567-121">Authorization</span></span>  | <span data-ttu-id="97567-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97567-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97567-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97567-124">Content-Type</span></span>  | <span data-ttu-id="97567-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="97567-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97567-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="97567-127">Request body</span></span>
<span data-ttu-id="97567-128">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97567-128">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="97567-129">响应</span><span class="sxs-lookup"><span data-stu-id="97567-129">Response</span></span>

<span data-ttu-id="97567-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97567-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97567-131">示例</span><span class="sxs-lookup"><span data-stu-id="97567-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97567-132">请求</span><span class="sxs-lookup"><span data-stu-id="97567-132">Request</span></span>
<span data-ttu-id="97567-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97567-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97567-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="97567-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="97567-135">C#</span><span class="sxs-lookup"><span data-stu-id="97567-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97567-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97567-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97567-137">Java</span><span class="sxs-lookup"><span data-stu-id="97567-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="97567-138">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97567-138">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="97567-139">响应</span><span class="sxs-lookup"><span data-stu-id="97567-139">Response</span></span>
<span data-ttu-id="97567-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97567-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
