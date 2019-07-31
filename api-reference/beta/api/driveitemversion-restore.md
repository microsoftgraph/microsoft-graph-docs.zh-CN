---
author: JeremyKelley
description: 将 DriveItem 的以前版本还原为当前版本。 这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。
ms.date: 09/10/2017
title: 还原以前的版本
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 73c5f590976dc8b6f2e529421449895bb1863f8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956903"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="80eb5-104">还原 DriveItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="80eb5-104">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80eb5-105">将 DriveItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="80eb5-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="80eb5-106">这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="80eb5-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="80eb5-107">权限</span><span class="sxs-lookup"><span data-stu-id="80eb5-107">Permissions</span></span>

<span data-ttu-id="80eb5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80eb5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80eb5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="80eb5-110">Permission type</span></span>      | <span data-ttu-id="80eb5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80eb5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80eb5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80eb5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="80eb5-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80eb5-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="80eb5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80eb5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80eb5-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80eb5-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="80eb5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="80eb5-116">Application</span></span> | <span data-ttu-id="80eb5-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80eb5-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80eb5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80eb5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="80eb5-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="80eb5-119">Request body</span></span>

<span data-ttu-id="80eb5-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="80eb5-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="80eb5-121">示例</span><span class="sxs-lookup"><span data-stu-id="80eb5-121">Example</span></span>

<span data-ttu-id="80eb5-122">本示例还原由 `{item-id}` 和 `{version-id}` 标识的文件的一个版本。</span><span class="sxs-lookup"><span data-stu-id="80eb5-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="80eb5-123">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="80eb5-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="80eb5-124">C#</span><span class="sxs-lookup"><span data-stu-id="80eb5-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80eb5-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="80eb5-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80eb5-126">目标-C</span><span class="sxs-lookup"><span data-stu-id="80eb5-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="80eb5-127">Java</span><span class="sxs-lookup"><span data-stu-id="80eb5-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="80eb5-128">响应</span><span class="sxs-lookup"><span data-stu-id="80eb5-128">Response</span></span>

<span data-ttu-id="80eb5-129">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="80eb5-129">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
