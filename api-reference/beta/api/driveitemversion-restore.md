---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 还原以前的版本
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ede7eb6275a4d23c715a3c981686355fc20aa369
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259946"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="b3bac-102">还原 DriveItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="b3bac-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3bac-103">将 DriveItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="b3bac-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="b3bac-104">这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="b3bac-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3bac-105">权限</span><span class="sxs-lookup"><span data-stu-id="b3bac-105">Permissions</span></span>

<span data-ttu-id="b3bac-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3bac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3bac-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3bac-108">Permission type</span></span>      | <span data-ttu-id="b3bac-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3bac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3bac-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3bac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b3bac-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3bac-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3bac-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3bac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3bac-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3bac-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3bac-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3bac-114">Application</span></span> | <span data-ttu-id="b3bac-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3bac-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3bac-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3bac-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="b3bac-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3bac-117">Request body</span></span>

<span data-ttu-id="b3bac-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3bac-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="b3bac-119">示例</span><span class="sxs-lookup"><span data-stu-id="b3bac-119">Example</span></span>

<span data-ttu-id="b3bac-120">本示例还原由 `{item-id}` 和 `{version-id}` 标识的文件的一个版本。</span><span class="sxs-lookup"><span data-stu-id="b3bac-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="b3bac-121">响应</span><span class="sxs-lookup"><span data-stu-id="b3bac-121">Response</span></span>

<span data-ttu-id="b3bac-122">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="b3bac-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b3bac-123">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b3bac-123">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b3bac-124">C#</span><span class="sxs-lookup"><span data-stu-id="b3bac-124">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/restore-item-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3bac-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="b3bac-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/restore-item-version-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b3bac-126">目标-C</span><span class="sxs-lookup"><span data-stu-id="b3bac-126">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/restore-item-version-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
