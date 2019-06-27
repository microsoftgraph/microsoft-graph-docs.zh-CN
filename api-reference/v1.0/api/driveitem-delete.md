---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 删除文件或文件夹
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e6e91323403964a57784fd745563425d277bf5ff
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276977"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="dbb89-102">删除 DriveItem</span><span class="sxs-lookup"><span data-stu-id="dbb89-102">Delete a DriveItem</span></span>

<span data-ttu-id="dbb89-p101">通过使用其 ID 或路径删除 [DriveItem](../resources/driveitem.md)。注意，使用此方法删除项将把项移动到回收站中，而不是永久删除该项。</span><span class="sxs-lookup"><span data-stu-id="dbb89-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbb89-105">权限</span><span class="sxs-lookup"><span data-stu-id="dbb89-105">Permissions</span></span>

<span data-ttu-id="dbb89-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbb89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbb89-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbb89-108">Permission type</span></span>      | <span data-ttu-id="dbb89-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dbb89-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbb89-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbb89-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dbb89-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbb89-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbb89-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbb89-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbb89-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbb89-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbb89-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbb89-114">Application</span></span> | <span data-ttu-id="dbb89-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbb89-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbb89-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbb89-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="dbb89-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="dbb89-117">Optional request headers</span></span>

| <span data-ttu-id="dbb89-118">名称</span><span class="sxs-lookup"><span data-stu-id="dbb89-118">Name</span></span>          | <span data-ttu-id="dbb89-119">类型</span><span class="sxs-lookup"><span data-stu-id="dbb89-119">Type</span></span>   | <span data-ttu-id="dbb89-120">说明</span><span class="sxs-lookup"><span data-stu-id="dbb89-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="dbb89-121">if-match</span><span class="sxs-lookup"><span data-stu-id="dbb89-121">if-match</span></span>      | <span data-ttu-id="dbb89-122">String</span><span class="sxs-lookup"><span data-stu-id="dbb89-122">String</span></span> | <span data-ttu-id="dbb89-123">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="dbb89-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="dbb89-124">示例</span><span class="sxs-lookup"><span data-stu-id="dbb89-124">Example</span></span>

<span data-ttu-id="dbb89-125">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="dbb89-125">Here is an example of how to call this API.</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="dbb89-126">响应</span><span class="sxs-lookup"><span data-stu-id="dbb89-126">Response</span></span>

<span data-ttu-id="dbb89-127">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="dbb89-127">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dbb89-128">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dbb89-128">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dbb89-129">C#</span><span class="sxs-lookup"><span data-stu-id="dbb89-129">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbb89-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="dbb89-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dbb89-131">目标-C</span><span class="sxs-lookup"><span data-stu-id="dbb89-131">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-responses"></a><span data-ttu-id="dbb89-132">错误响应</span><span class="sxs-lookup"><span data-stu-id="dbb89-132">Error responses</span></span>

<span data-ttu-id="dbb89-133">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="dbb89-133">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
