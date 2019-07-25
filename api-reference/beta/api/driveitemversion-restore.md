---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 还原以前的版本
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 01e423c5bfb96b0f48c34f4615e1b49e1b533a27
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860822"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="7e51d-102">还原 DriveItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="7e51d-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e51d-103">将 DriveItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="7e51d-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="7e51d-104">这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="7e51d-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e51d-105">权限</span><span class="sxs-lookup"><span data-stu-id="7e51d-105">Permissions</span></span>

<span data-ttu-id="7e51d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e51d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e51d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e51d-108">Permission type</span></span>      | <span data-ttu-id="7e51d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e51d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e51d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e51d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e51d-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e51d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e51d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e51d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e51d-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e51d-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e51d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e51d-114">Application</span></span> | <span data-ttu-id="7e51d-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e51d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e51d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e51d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="7e51d-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e51d-117">Request body</span></span>

<span data-ttu-id="7e51d-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="7e51d-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="7e51d-119">示例</span><span class="sxs-lookup"><span data-stu-id="7e51d-119">Example</span></span>

<span data-ttu-id="7e51d-120">本示例还原由 `{item-id}` 和 `{version-id}` 标识的文件的一个版本。</span><span class="sxs-lookup"><span data-stu-id="7e51d-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e51d-121">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7e51d-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e51d-122">C#</span><span class="sxs-lookup"><span data-stu-id="7e51d-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e51d-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="7e51d-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e51d-124">目标-C</span><span class="sxs-lookup"><span data-stu-id="7e51d-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7e51d-125">Java</span><span class="sxs-lookup"><span data-stu-id="7e51d-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="7e51d-126">响应</span><span class="sxs-lookup"><span data-stu-id="7e51d-126">Response</span></span>

<span data-ttu-id="7e51d-127">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="7e51d-127">If successful, the API call returns a `204 No content`.</span></span>

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
