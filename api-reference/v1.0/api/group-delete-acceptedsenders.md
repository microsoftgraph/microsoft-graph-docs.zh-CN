---
title: 删除 acceptedSender
description: '从接受的发件人列表中删除用户或组。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 10e095d00955addf6e5f1f65d8abb576018144ee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337543"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="77de9-103">删除 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="77de9-103">Remove acceptedSender</span></span>
<span data-ttu-id="77de9-104">从接受的发件人列表中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="77de9-104">Remove a user or group from the accepted-senders list.</span></span> 

## <a name="permissions"></a><span data-ttu-id="77de9-105">权限</span><span class="sxs-lookup"><span data-stu-id="77de9-105">Permissions</span></span>
<span data-ttu-id="77de9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77de9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77de9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="77de9-108">Permission type</span></span>                        | <span data-ttu-id="77de9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77de9-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="77de9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77de9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="77de9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77de9-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="77de9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77de9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77de9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="77de9-113">Not supported.</span></span> |
| <span data-ttu-id="77de9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="77de9-114">Application</span></span>                            | <span data-ttu-id="77de9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="77de9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77de9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77de9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="77de9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="77de9-117">Request headers</span></span>
| <span data-ttu-id="77de9-118">标头</span><span class="sxs-lookup"><span data-stu-id="77de9-118">Header</span></span>         | <span data-ttu-id="77de9-119">值</span><span class="sxs-lookup"><span data-stu-id="77de9-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="77de9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="77de9-120">Authorization</span></span>  | <span data-ttu-id="77de9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77de9-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="77de9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="77de9-123">Request body</span></span>
<span data-ttu-id="77de9-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77de9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77de9-125">响应</span><span class="sxs-lookup"><span data-stu-id="77de9-125">Response</span></span>
<span data-ttu-id="77de9-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="77de9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77de9-128">示例</span><span class="sxs-lookup"><span data-stu-id="77de9-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="77de9-129">请求</span><span class="sxs-lookup"><span data-stu-id="77de9-129">Request</span></span>
<span data-ttu-id="77de9-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="77de9-130">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="77de9-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="77de9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_acceptedsenders_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77de9-132">C#</span><span class="sxs-lookup"><span data-stu-id="77de9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-acceptedsenders-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77de9-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77de9-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-acceptedsenders-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77de9-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="77de9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-acceptedsenders-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77de9-135">Java</span><span class="sxs-lookup"><span data-stu-id="77de9-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-acceptedsenders-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="77de9-136">响应</span><span class="sxs-lookup"><span data-stu-id="77de9-136">Response</span></span>
<span data-ttu-id="77de9-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="77de9-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
