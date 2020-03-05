---
title: 删除照片
description: 删除照片。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8003e77a908b5242635c36b54a1cdfe6d257d54b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455849"
---
# <a name="delete-photo"></a><span data-ttu-id="924c2-103">删除照片</span><span class="sxs-lookup"><span data-stu-id="924c2-103">Delete photo</span></span>

<span data-ttu-id="924c2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="924c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="924c2-105">删除照片。</span><span class="sxs-lookup"><span data-stu-id="924c2-105">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="924c2-106">权限</span><span class="sxs-lookup"><span data-stu-id="924c2-106">Permissions</span></span>
<span data-ttu-id="924c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="924c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="924c2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="924c2-109">Permission type</span></span>      | <span data-ttu-id="924c2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="924c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="924c2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="924c2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="924c2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="924c2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="924c2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="924c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="924c2-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="924c2-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="924c2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="924c2-115">Application</span></span> | <span data-ttu-id="924c2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="924c2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="924c2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="924c2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="924c2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="924c2-118">Request headers</span></span>
| <span data-ttu-id="924c2-119">名称</span><span class="sxs-lookup"><span data-stu-id="924c2-119">Name</span></span>       | <span data-ttu-id="924c2-120">类型</span><span class="sxs-lookup"><span data-stu-id="924c2-120">Type</span></span> | <span data-ttu-id="924c2-121">说明</span><span class="sxs-lookup"><span data-stu-id="924c2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="924c2-122">if-match</span><span class="sxs-lookup"><span data-stu-id="924c2-122">if-match</span></span>  | <span data-ttu-id="924c2-123">string</span><span class="sxs-lookup"><span data-stu-id="924c2-123">string</span></span>  | <span data-ttu-id="924c2-124">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="924c2-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="924c2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="924c2-125">Authorization</span></span>  | <span data-ttu-id="924c2-126">string</span><span class="sxs-lookup"><span data-stu-id="924c2-126">string</span></span>  | <span data-ttu-id="924c2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="924c2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="924c2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="924c2-129">Request body</span></span>
<span data-ttu-id="924c2-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="924c2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="924c2-131">响应</span><span class="sxs-lookup"><span data-stu-id="924c2-131">Response</span></span>

<span data-ttu-id="924c2-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="924c2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="924c2-134">示例</span><span class="sxs-lookup"><span data-stu-id="924c2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="924c2-135">请求</span><span class="sxs-lookup"><span data-stu-id="924c2-135">Request</span></span>
<span data-ttu-id="924c2-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="924c2-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="924c2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="924c2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
# <a name="c"></a>[<span data-ttu-id="924c2-138">C#</span><span class="sxs-lookup"><span data-stu-id="924c2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="924c2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="924c2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="924c2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="924c2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="924c2-141">响应</span><span class="sxs-lookup"><span data-stu-id="924c2-141">Response</span></span>
<span data-ttu-id="924c2-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="924c2-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
