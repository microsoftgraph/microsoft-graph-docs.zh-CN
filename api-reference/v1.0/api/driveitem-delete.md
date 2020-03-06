---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 删除文件或文件夹
localization_priority: Normal
ms.prod: sharepoint
description: 通过使用其 ID 或路径删除 DriveItem。
doc_type: apiPageType
ms.openlocfilehash: e385c005565819999c3d77066ad636adda92b3d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517767"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="18f43-103">删除 DriveItem</span><span class="sxs-lookup"><span data-stu-id="18f43-103">Delete a DriveItem</span></span>

<span data-ttu-id="18f43-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18f43-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18f43-p101">通过使用其 ID 或路径删除 [DriveItem](../resources/driveitem.md)。注意，使用此方法删除项将把项移动到回收站中，而不是永久删除该项。</span><span class="sxs-lookup"><span data-stu-id="18f43-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="18f43-107">权限</span><span class="sxs-lookup"><span data-stu-id="18f43-107">Permissions</span></span>

<span data-ttu-id="18f43-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18f43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18f43-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="18f43-110">Permission type</span></span>      | <span data-ttu-id="18f43-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18f43-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18f43-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18f43-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18f43-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f43-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="18f43-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18f43-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18f43-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f43-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="18f43-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="18f43-116">Application</span></span> | <span data-ttu-id="18f43-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f43-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18f43-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18f43-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="18f43-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="18f43-119">Optional request headers</span></span>

| <span data-ttu-id="18f43-120">名称</span><span class="sxs-lookup"><span data-stu-id="18f43-120">Name</span></span>          | <span data-ttu-id="18f43-121">类型</span><span class="sxs-lookup"><span data-stu-id="18f43-121">Type</span></span>   | <span data-ttu-id="18f43-122">说明</span><span class="sxs-lookup"><span data-stu-id="18f43-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="18f43-123">if-match</span><span class="sxs-lookup"><span data-stu-id="18f43-123">if-match</span></span>      | <span data-ttu-id="18f43-124">String</span><span class="sxs-lookup"><span data-stu-id="18f43-124">String</span></span> | <span data-ttu-id="18f43-125">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="18f43-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="18f43-126">示例</span><span class="sxs-lookup"><span data-stu-id="18f43-126">Example</span></span>

<span data-ttu-id="18f43-127">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="18f43-127">Here is an example of how to call this API.</span></span>


# <a name="http"></a>[<span data-ttu-id="18f43-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="18f43-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-drive-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
DELETE /me/drive/items/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="18f43-129">C#</span><span class="sxs-lookup"><span data-stu-id="18f43-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-drive-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18f43-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18f43-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-drive-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18f43-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18f43-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-drive-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18f43-132">Java</span><span class="sxs-lookup"><span data-stu-id="18f43-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-drive-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="18f43-133">响应</span><span class="sxs-lookup"><span data-stu-id="18f43-133">Response</span></span>

<span data-ttu-id="18f43-134">如果成功，此调用将返回 `204 No Content` 响应，以指明资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="18f43-134">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="18f43-135">错误响应</span><span class="sxs-lookup"><span data-stu-id="18f43-135">Error responses</span></span>

<span data-ttu-id="18f43-136">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="18f43-136">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete",
  "suppressions": [
  ]
} -->
