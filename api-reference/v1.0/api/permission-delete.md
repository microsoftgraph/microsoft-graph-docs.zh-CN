---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 删除对项目的访问权限
localization_priority: Normal
ms.openlocfilehash: ebbc3388e1e207b83ec3cd7ea45635a49f5f7a01
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275542"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="f166e-102">从文件或文件夹中删除共享权限</span><span class="sxs-lookup"><span data-stu-id="f166e-102">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="f166e-103">删除 [DriveItem](../resources/driveitem.md) 访问权限。</span><span class="sxs-lookup"><span data-stu-id="f166e-103">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="f166e-104">只能删除**非**继承的共享权限。</span><span class="sxs-lookup"><span data-stu-id="f166e-104">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="f166e-105">**InheritedFrom** 属性必须为 `null`。</span><span class="sxs-lookup"><span data-stu-id="f166e-105">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="f166e-106">权限</span><span class="sxs-lookup"><span data-stu-id="f166e-106">Permissions</span></span>

<span data-ttu-id="f166e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f166e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f166e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f166e-109">Permission type</span></span>      | <span data-ttu-id="f166e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f166e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f166e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f166e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f166e-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f166e-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f166e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f166e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f166e-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f166e-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f166e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f166e-115">Application</span></span> | <span data-ttu-id="f166e-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f166e-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f166e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f166e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="f166e-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="f166e-118">Optional request headers</span></span>

| <span data-ttu-id="f166e-119">名称</span><span class="sxs-lookup"><span data-stu-id="f166e-119">Name</span></span>          | <span data-ttu-id="f166e-120">类型</span><span class="sxs-lookup"><span data-stu-id="f166e-120">Type</span></span>   | <span data-ttu-id="f166e-121">说明</span><span class="sxs-lookup"><span data-stu-id="f166e-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f166e-122">if-match</span><span class="sxs-lookup"><span data-stu-id="f166e-122">if-match</span></span>      | <span data-ttu-id="f166e-123">string</span><span class="sxs-lookup"><span data-stu-id="f166e-123">string</span></span> | <span data-ttu-id="f166e-124">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="f166e-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="f166e-125">响应</span><span class="sxs-lookup"><span data-stu-id="f166e-125">Response</span></span>

<span data-ttu-id="f166e-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f166e-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f166e-127">示例</span><span class="sxs-lookup"><span data-stu-id="f166e-127">Example</span></span>

<span data-ttu-id="f166e-128">本示例从当前用户 OneDrive 的项 {item-id} 中删除标识为 {perm-id} 的权限。</span><span class="sxs-lookup"><span data-stu-id="f166e-128">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite", "tags": "service.graph" }-->

```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="f166e-129">响应</span><span class="sxs-lookup"><span data-stu-id="f166e-129">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f166e-130">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f166e-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f166e-131">C#</span><span class="sxs-lookup"><span data-stu-id="f166e-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-permission-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f166e-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="f166e-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-permission-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f166e-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="f166e-133">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete-permission-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="f166e-134">注解</span><span class="sxs-lookup"><span data-stu-id="f166e-134">Remarks</span></span>

* <span data-ttu-id="f166e-135">具有 `personal`（OneDrive 个人版）**driveType** 的 [驱动器](../resources/drive.md) 无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="f166e-135">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "Sharing/Remove permissions",
  "suppressions": [
    "Error: /api-reference/v1.0/api/permission-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/permission-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/permission-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
