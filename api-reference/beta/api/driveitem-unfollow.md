---
author: chackman
ms.author: chackman
title: 取消追随驱动器项目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c2e687cb93d64994036cc46e8a245e707dd58b16
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436240"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="8e55c-102">取消追随驱动器项目</span><span class="sxs-lookup"><span data-stu-id="8e55c-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e55c-103">取消追随[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="8e55c-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="8e55c-104">**注意:** 若要关注某个项目, 请参阅 "[关注项](driveitem-follow.md)"。</span><span class="sxs-lookup"><span data-stu-id="8e55c-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e55c-105">权限</span><span class="sxs-lookup"><span data-stu-id="8e55c-105">Permissions</span></span>

<span data-ttu-id="8e55c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e55c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e55c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e55c-108">Permission type</span></span>      | <span data-ttu-id="8e55c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e55c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e55c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e55c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8e55c-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e55c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e55c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e55c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e55c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e55c-113">Not supported.</span></span>    |
|<span data-ttu-id="8e55c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e55c-114">Application</span></span> | <span data-ttu-id="8e55c-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e55c-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e55c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e55c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="8e55c-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e55c-117">Request body</span></span>

<span data-ttu-id="8e55c-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e55c-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="8e55c-119">响应</span><span class="sxs-lookup"><span data-stu-id="8e55c-119">Response</span></span>

<span data-ttu-id="8e55c-120">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="8e55c-120">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="8e55c-121">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8e55c-121">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e55c-122">示例</span><span class="sxs-lookup"><span data-stu-id="8e55c-122">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e55c-123">请求</span><span class="sxs-lookup"><span data-stu-id="8e55c-123">Request</span></span>
<span data-ttu-id="8e55c-124">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e55c-124">Here is an example of the request.</span></span>
<span data-ttu-id="8e55c-125">本示例将 unfollows 标识为的`{item-id}`项目。</span><span class="sxs-lookup"><span data-stu-id="8e55c-125">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8e55c-126">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8e55c-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e55c-127">C#</span><span class="sxs-lookup"><span data-stu-id="8e55c-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e55c-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="8e55c-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e55c-129">目标-C</span><span class="sxs-lookup"><span data-stu-id="8e55c-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8e55c-130">响应</span><span class="sxs-lookup"><span data-stu-id="8e55c-130">Response</span></span>
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
