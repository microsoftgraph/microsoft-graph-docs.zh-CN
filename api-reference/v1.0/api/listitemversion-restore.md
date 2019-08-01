---
title: 还原 ListItem 的以前版本
description: 将 ListItem 的以前版本还原为当前版本。 这将使用以前版本的内容创建一个新版本，但保留项的所有现有版本。
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 91671a0e974cedfeaae491771054fe040348fa43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023102"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="ab143-104">还原 ListItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="ab143-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="ab143-105">将 ListItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="ab143-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="ab143-106">这将使用以前版本的内容创建一个新版本，但保留项的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="ab143-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab143-107">权限</span><span class="sxs-lookup"><span data-stu-id="ab143-107">Permissions</span></span>

<span data-ttu-id="ab143-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab143-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="ab143-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab143-110">Permission type</span></span>             |         <span data-ttu-id="ab143-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab143-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="ab143-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab143-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab143-113">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ab143-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="ab143-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab143-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab143-115">无</span><span class="sxs-lookup"><span data-stu-id="ab143-115">n/a</span></span>                                                          |
| <span data-ttu-id="ab143-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab143-116">Application</span></span>                            | <span data-ttu-id="ab143-117">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ab143-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab143-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab143-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="ab143-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab143-119">Request body</span></span>

<span data-ttu-id="ab143-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab143-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="ab143-121">示例</span><span class="sxs-lookup"><span data-stu-id="ab143-121">Example</span></span>

<span data-ttu-id="ab143-122">本示例还原由 `{item-id}` 和 `{version-id}` 标识的 listItem 的一个版本。</span><span class="sxs-lookup"><span data-stu-id="ab143-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ab143-123">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ab143-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ab143-124">C#</span><span class="sxs-lookup"><span data-stu-id="ab143-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ab143-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="ab143-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ab143-126">目标-C</span><span class="sxs-lookup"><span data-stu-id="ab143-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ab143-127">Java</span><span class="sxs-lookup"><span data-stu-id="ab143-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="ab143-128">响应</span><span class="sxs-lookup"><span data-stu-id="ab143-128">Response</span></span>

<span data-ttu-id="ab143-129">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="ab143-129">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->
