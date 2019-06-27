---
author: chackman
ms.author: chackman
title: 取消追随驱动器项目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9d43121f4db421bb934e2cce0f045386138b36af
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260016"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="6b1f0-102">取消追随驱动器项目</span><span class="sxs-lookup"><span data-stu-id="6b1f0-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b1f0-103">取消追随[driveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="6b1f0-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="6b1f0-104">**注意:** 若要关注某个项目, 请参阅 "[关注项](driveitem-follow.md)"。</span><span class="sxs-lookup"><span data-stu-id="6b1f0-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b1f0-105">权限</span><span class="sxs-lookup"><span data-stu-id="6b1f0-105">Permissions</span></span>

<span data-ttu-id="6b1f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b1f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b1f0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b1f0-108">Permission type</span></span>      | <span data-ttu-id="6b1f0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b1f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b1f0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b1f0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6b1f0-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b1f0-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b1f0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b1f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b1f0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b1f0-113">Not supported.</span></span>    |
|<span data-ttu-id="6b1f0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b1f0-114">Application</span></span> | <span data-ttu-id="6b1f0-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b1f0-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b1f0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b1f0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="6b1f0-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b1f0-117">Request body</span></span>

<span data-ttu-id="6b1f0-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b1f0-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="6b1f0-119">响应</span><span class="sxs-lookup"><span data-stu-id="6b1f0-119">Response</span></span>

<span data-ttu-id="6b1f0-120">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="6b1f0-120">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="6b1f0-121">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6b1f0-121">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b1f0-122">示例</span><span class="sxs-lookup"><span data-stu-id="6b1f0-122">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b1f0-123">请求</span><span class="sxs-lookup"><span data-stu-id="6b1f0-123">Request</span></span>
<span data-ttu-id="6b1f0-124">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b1f0-124">Here is an example of the request.</span></span>
<span data-ttu-id="6b1f0-125">本示例将 unfollows 标识为的`{item-id}`项目。</span><span class="sxs-lookup"><span data-stu-id="6b1f0-125">This example unfollows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```
### <a name="response"></a><span data-ttu-id="6b1f0-126">响应</span><span class="sxs-lookup"><span data-stu-id="6b1f0-126">Response</span></span>
<!-- { 
    "blockType": "response", 
    "truncated": true 
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6b1f0-127">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6b1f0-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6b1f0-128">C#</span><span class="sxs-lookup"><span data-stu-id="6b1f0-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/unfollow-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b1f0-129">Javascript</span><span class="sxs-lookup"><span data-stu-id="6b1f0-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/unfollow-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6b1f0-130">目标-C</span><span class="sxs-lookup"><span data-stu-id="6b1f0-130">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/unfollow-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-unfollow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
