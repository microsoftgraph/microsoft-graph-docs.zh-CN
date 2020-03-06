---
title: 还原 DriveItem 的以前版本
description: 将 DriveItem 的以前版本还原为当前版本。 这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 37f4928e6e3550cb7e022ed4b0ea1ab969a43ec3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517634"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="dad75-104">还原 DriveItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="dad75-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="dad75-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dad75-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dad75-106">将 DriveItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="dad75-106">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="dad75-107">这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="dad75-107">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="dad75-108">权限</span><span class="sxs-lookup"><span data-stu-id="dad75-108">Permissions</span></span>

<span data-ttu-id="dad75-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dad75-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dad75-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dad75-111">Permission type</span></span>      | <span data-ttu-id="dad75-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dad75-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dad75-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dad75-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dad75-114">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad75-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dad75-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dad75-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dad75-116">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad75-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="dad75-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dad75-117">Application</span></span> | <span data-ttu-id="dad75-118">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad75-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dad75-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dad75-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="dad75-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="dad75-120">Request body</span></span>

<span data-ttu-id="dad75-121">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="dad75-121">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="dad75-122">示例</span><span class="sxs-lookup"><span data-stu-id="dad75-122">Example</span></span>

<span data-ttu-id="dad75-123">本示例还原由 `{item-id}` 和 `{version-id}` 标识的文件的一个版本。</span><span class="sxs-lookup"><span data-stu-id="dad75-123">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="dad75-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="dad75-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="c"></a>[<span data-ttu-id="dad75-125">C#</span><span class="sxs-lookup"><span data-stu-id="dad75-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dad75-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dad75-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dad75-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dad75-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dad75-128">Java</span><span class="sxs-lookup"><span data-stu-id="dad75-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="dad75-129">响应</span><span class="sxs-lookup"><span data-stu-id="dad75-129">Response</span></span>

<span data-ttu-id="dad75-130">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="dad75-130">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->
