---
title: 还原 DriveItem 的以前版本
description: 将 DriveItem 的以前版本还原为当前版本。 这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 53a8f5e40e06ef90662a55c44ca718bc82f4fb4b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616228"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="f3a02-104">还原 DriveItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="f3a02-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="f3a02-105">将 DriveItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="f3a02-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="f3a02-106">这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="f3a02-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3a02-107">权限</span><span class="sxs-lookup"><span data-stu-id="f3a02-107">Permissions</span></span>

<span data-ttu-id="f3a02-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3a02-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3a02-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3a02-110">Permission type</span></span>      | <span data-ttu-id="f3a02-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3a02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3a02-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3a02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f3a02-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3a02-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3a02-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3a02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3a02-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3a02-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3a02-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3a02-116">Application</span></span> | <span data-ttu-id="f3a02-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3a02-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3a02-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3a02-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="f3a02-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3a02-119">Request body</span></span>

<span data-ttu-id="f3a02-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="f3a02-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="f3a02-121">示例</span><span class="sxs-lookup"><span data-stu-id="f3a02-121">Example</span></span>

<span data-ttu-id="f3a02-122">本示例还原由 `{item-id}` 和 `{version-id}` 标识的文件的一个版本。</span><span class="sxs-lookup"><span data-stu-id="f3a02-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="f3a02-123">响应</span><span class="sxs-lookup"><span data-stu-id="f3a02-123">Response</span></span>

<span data-ttu-id="f3a02-124">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="f3a02-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f3a02-125">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f3a02-125">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f3a02-126">语言</span><span class="sxs-lookup"><span data-stu-id="f3a02-126">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/restore-item-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3a02-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="f3a02-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/restore-item-version-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
