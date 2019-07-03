---
title: 删除照片
description: 删除照片。
localization_priority: Normal
ms.openlocfilehash: 9ca65416ecce815f99dbf8a0ff84724322f75df2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458864"
---
# <a name="delete-photo"></a><span data-ttu-id="6b977-103">删除照片</span><span class="sxs-lookup"><span data-stu-id="6b977-103">Delete photo</span></span>

<span data-ttu-id="6b977-104">删除照片。</span><span class="sxs-lookup"><span data-stu-id="6b977-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b977-105">权限</span><span class="sxs-lookup"><span data-stu-id="6b977-105">Permissions</span></span>
<span data-ttu-id="6b977-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b977-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b977-108">Permission type</span></span>      | <span data-ttu-id="6b977-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b977-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b977-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b977-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6b977-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b977-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6b977-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b977-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b977-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b977-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6b977-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b977-114">Application</span></span> | <span data-ttu-id="6b977-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b977-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b977-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b977-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="6b977-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b977-117">Request headers</span></span>
| <span data-ttu-id="6b977-118">名称</span><span class="sxs-lookup"><span data-stu-id="6b977-118">Name</span></span>       | <span data-ttu-id="6b977-119">类型</span><span class="sxs-lookup"><span data-stu-id="6b977-119">Type</span></span> | <span data-ttu-id="6b977-120">说明</span><span class="sxs-lookup"><span data-stu-id="6b977-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6b977-121">if-match</span><span class="sxs-lookup"><span data-stu-id="6b977-121">if-match</span></span>  | <span data-ttu-id="6b977-122">string</span><span class="sxs-lookup"><span data-stu-id="6b977-122">string</span></span>  | <span data-ttu-id="6b977-123">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="6b977-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="6b977-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b977-124">Authorization</span></span>  | <span data-ttu-id="6b977-125">string</span><span class="sxs-lookup"><span data-stu-id="6b977-125">string</span></span>  | <span data-ttu-id="6b977-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b977-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b977-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b977-128">Request body</span></span>
<span data-ttu-id="6b977-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b977-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b977-130">响应</span><span class="sxs-lookup"><span data-stu-id="6b977-130">Response</span></span>

<span data-ttu-id="6b977-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6b977-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b977-133">示例</span><span class="sxs-lookup"><span data-stu-id="6b977-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b977-134">请求</span><span class="sxs-lookup"><span data-stu-id="6b977-134">Request</span></span>
<span data-ttu-id="6b977-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b977-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6b977-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6b977-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b977-137">C#</span><span class="sxs-lookup"><span data-stu-id="6b977-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b977-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="6b977-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b977-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="6b977-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b977-140">响应</span><span class="sxs-lookup"><span data-stu-id="6b977-140">Response</span></span>
<span data-ttu-id="6b977-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6b977-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
