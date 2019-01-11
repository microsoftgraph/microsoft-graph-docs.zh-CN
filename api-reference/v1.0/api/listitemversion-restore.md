---
title: 还原 ListItem 的以前版本
description: 将 ListItem 的以前版本还原为当前版本。 这将使用以前版本的内容创建一个新版本，但保留项的所有现有版本。
localization_priority: Normal
ms.openlocfilehash: 6fb315986a8dc22363e22235f8cf65e0cbc21fed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866960"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="7b74b-104">还原 ListItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="7b74b-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="7b74b-105">将 ListItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="7b74b-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="7b74b-106">这将使用以前版本的内容创建一个新版本，但保留项的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="7b74b-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b74b-107">权限</span><span class="sxs-lookup"><span data-stu-id="7b74b-107">Permissions</span></span>

<span data-ttu-id="7b74b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b74b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="7b74b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b74b-110">Permission type</span></span>             |         <span data-ttu-id="7b74b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b74b-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="7b74b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b74b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b74b-113">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7b74b-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="7b74b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b74b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b74b-115">无</span><span class="sxs-lookup"><span data-stu-id="7b74b-115">n/a</span></span>                                                          |
| <span data-ttu-id="7b74b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b74b-116">Application</span></span>                            | <span data-ttu-id="7b74b-117">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7b74b-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b74b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b74b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="7b74b-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b74b-119">Request body</span></span>

<span data-ttu-id="7b74b-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="7b74b-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="7b74b-121">示例</span><span class="sxs-lookup"><span data-stu-id="7b74b-121">Example</span></span>

<span data-ttu-id="7b74b-122">本示例还原由 `{item-id}` 和 `{version-id}` 标识的 listItem 的一个版本。</span><span class="sxs-lookup"><span data-stu-id="7b74b-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="7b74b-123">响应</span><span class="sxs-lookup"><span data-stu-id="7b74b-123">Response</span></span>

<span data-ttu-id="7b74b-124">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="7b74b-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
