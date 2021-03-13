---
author: chackman
description: 取消关注用户正在关注的项目。
title: 取消关注驱动器项
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: fcaa9f39163daa42e12fbea324f4ecbc93ae0977
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50776793"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="d3619-103">取消关注驱动器项</span><span class="sxs-lookup"><span data-stu-id="d3619-103">Unfollow drive item</span></span>

<span data-ttu-id="d3619-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3619-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3619-105">取消关注 [driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="d3619-105">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="d3619-106">**注意：** 若要关注某个项目，请参阅关注 [项目](driveitem-follow.md)。</span><span class="sxs-lookup"><span data-stu-id="d3619-106">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d3619-107">权限</span><span class="sxs-lookup"><span data-stu-id="d3619-107">Permissions</span></span>

<span data-ttu-id="d3619-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3619-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3619-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3619-110">Permission type</span></span>      | <span data-ttu-id="d3619-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3619-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3619-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3619-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d3619-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3619-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d3619-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3619-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3619-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3619-115">Not supported.</span></span>    |
|<span data-ttu-id="d3619-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3619-116">Application</span></span> | <span data-ttu-id="d3619-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3619-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3619-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3619-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id}
DELETE /users/{user-id}/drive/following/{item-id}
POST /me/drive/items/{item-id}/unfollow
POST /users/{user-id}/drive/items/{item-id}/unfollow
```

## <a name="request-body"></a><span data-ttu-id="d3619-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3619-119">Request body</span></span>

<span data-ttu-id="d3619-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3619-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="d3619-121">响应</span><span class="sxs-lookup"><span data-stu-id="d3619-121">Response</span></span>

<span data-ttu-id="d3619-122">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="d3619-122">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="d3619-123">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d3619-123">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3619-124">示例</span><span class="sxs-lookup"><span data-stu-id="d3619-124">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3619-125">请求</span><span class="sxs-lookup"><span data-stu-id="d3619-125">Request</span></span>
<span data-ttu-id="d3619-126">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3619-126">Here is an example of the request.</span></span>
<span data-ttu-id="d3619-127">本示例取消关注由 标识的项目 `{item-id}` 。</span><span class="sxs-lookup"><span data-stu-id="d3619-127">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="d3619-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3619-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/items/{item-id}/unfollow
```
# <a name="c"></a>[<span data-ttu-id="d3619-129">C#</span><span class="sxs-lookup"><span data-stu-id="d3619-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3619-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3619-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3619-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3619-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3619-132">Java</span><span class="sxs-lookup"><span data-stu-id="d3619-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d3619-133">响应</span><span class="sxs-lookup"><span data-stu-id="d3619-133">Response</span></span>
<!-- { 
    "blockType": "response", 
    "truncated": true 
} -->
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
  ]
}
-->


