---
author: chackman
ms.author: chackman
description: 取消追随用户正在关注的项目。
title: 取消追随驱动器项目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 29c07176a2d37f7e38deaa4c4020287d82495834
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432325"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="a5edd-103">取消追随驱动器项目</span><span class="sxs-lookup"><span data-stu-id="a5edd-103">Unfollow drive item</span></span>

<span data-ttu-id="a5edd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a5edd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5edd-105">取消追随[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="a5edd-105">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="a5edd-106">**注意：** 若要关注某个项目，请参阅 "[关注项](driveitem-follow.md)"。</span><span class="sxs-lookup"><span data-stu-id="a5edd-106">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a5edd-107">权限</span><span class="sxs-lookup"><span data-stu-id="a5edd-107">Permissions</span></span>

<span data-ttu-id="a5edd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5edd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5edd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5edd-110">Permission type</span></span>      | <span data-ttu-id="a5edd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5edd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5edd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5edd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5edd-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5edd-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5edd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5edd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5edd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5edd-115">Not supported.</span></span>    |
|<span data-ttu-id="a5edd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5edd-116">Application</span></span> | <span data-ttu-id="a5edd-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5edd-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5edd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5edd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id}
DELETE /users/{user-id}/drive/following/{item-id}
POST /me/drive/items/{item-id}/unfollow
POST /users/{user-id}/drive/items/{item-id}/unfollow
```

## <a name="request-body"></a><span data-ttu-id="a5edd-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5edd-119">Request body</span></span>

<span data-ttu-id="a5edd-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="a5edd-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="a5edd-121">响应</span><span class="sxs-lookup"><span data-stu-id="a5edd-121">Response</span></span>

<span data-ttu-id="a5edd-122">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="a5edd-122">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="a5edd-123">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a5edd-123">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5edd-124">示例</span><span class="sxs-lookup"><span data-stu-id="a5edd-124">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5edd-125">请求</span><span class="sxs-lookup"><span data-stu-id="a5edd-125">Request</span></span>
<span data-ttu-id="a5edd-126">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a5edd-126">Here is an example of the request.</span></span>
<span data-ttu-id="a5edd-127">本示例将 unfollows 标识为的`{item-id}`项目。</span><span class="sxs-lookup"><span data-stu-id="a5edd-127">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="a5edd-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5edd-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/items/{item-id}/unfollow
```
# <a name="c"></a>[<span data-ttu-id="a5edd-129">C#</span><span class="sxs-lookup"><span data-stu-id="a5edd-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5edd-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5edd-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5edd-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5edd-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a5edd-132">响应</span><span class="sxs-lookup"><span data-stu-id="a5edd-132">Response</span></span>
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
