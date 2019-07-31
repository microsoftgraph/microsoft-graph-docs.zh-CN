---
author: chackman
ms.author: chackman
description: 取消追随用户正在关注的项目。
title: 取消追随驱动器项目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 93d07621b745755cd57afaff458d711498e02863
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956945"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="baf40-103">取消追随驱动器项目</span><span class="sxs-lookup"><span data-stu-id="baf40-103">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baf40-104">取消追随[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="baf40-104">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="baf40-105">**注意:** 若要关注某个项目, 请参阅 "[关注项](driveitem-follow.md)"。</span><span class="sxs-lookup"><span data-stu-id="baf40-105">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="baf40-106">权限</span><span class="sxs-lookup"><span data-stu-id="baf40-106">Permissions</span></span>

<span data-ttu-id="baf40-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="baf40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baf40-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="baf40-109">Permission type</span></span>      | <span data-ttu-id="baf40-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="baf40-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baf40-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="baf40-111">Delegated (work or school account)</span></span> | <span data-ttu-id="baf40-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baf40-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="baf40-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="baf40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baf40-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="baf40-114">Not supported.</span></span>    |
|<span data-ttu-id="baf40-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="baf40-115">Application</span></span> | <span data-ttu-id="baf40-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baf40-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="baf40-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="baf40-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id}
DELETE /users/{user-id}/drive/following/{item-id}
POST /me/drive/items/{item-id}/unfollow
POST /users/{user-id}/drive/items/{item-id}/unfollow
```

## <a name="request-body"></a><span data-ttu-id="baf40-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="baf40-118">Request body</span></span>

<span data-ttu-id="baf40-119">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="baf40-119">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="baf40-120">响应</span><span class="sxs-lookup"><span data-stu-id="baf40-120">Response</span></span>

<span data-ttu-id="baf40-121">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="baf40-121">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="baf40-122">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="baf40-122">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baf40-123">示例</span><span class="sxs-lookup"><span data-stu-id="baf40-123">Example</span></span>
### <a name="request"></a><span data-ttu-id="baf40-124">请求</span><span class="sxs-lookup"><span data-stu-id="baf40-124">Request</span></span>
<span data-ttu-id="baf40-125">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="baf40-125">Here is an example of the request.</span></span>
<span data-ttu-id="baf40-126">本示例将 unfollows 标识为的`{item-id}`项目。</span><span class="sxs-lookup"><span data-stu-id="baf40-126">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="baf40-127">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="baf40-127">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/items/{item-id}/unfollow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="baf40-128">C#</span><span class="sxs-lookup"><span data-stu-id="baf40-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="baf40-129">Javascript</span><span class="sxs-lookup"><span data-stu-id="baf40-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="baf40-130">目标-C</span><span class="sxs-lookup"><span data-stu-id="baf40-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="baf40-131">Java</span><span class="sxs-lookup"><span data-stu-id="baf40-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="baf40-132">响应</span><span class="sxs-lookup"><span data-stu-id="baf40-132">Response</span></span>
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
