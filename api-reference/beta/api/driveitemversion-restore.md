---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 还原以前版本
ms.openlocfilehash: 507f58e79f209e1e65bfb8dcc2ac666f64a8d45d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042905"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="829ed-102">还原 DriveItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="829ed-102">Restore a previous version of a DriveItem</span></span>

> <span data-ttu-id="829ed-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="829ed-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="829ed-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="829ed-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="829ed-105">将 DriveItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="829ed-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="829ed-106">这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="829ed-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="829ed-107">权限</span><span class="sxs-lookup"><span data-stu-id="829ed-107">Permissions</span></span>

<span data-ttu-id="829ed-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="829ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="829ed-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="829ed-110">Permission type</span></span>      | <span data-ttu-id="829ed-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="829ed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="829ed-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="829ed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="829ed-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="829ed-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="829ed-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="829ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="829ed-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="829ed-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="829ed-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="829ed-116">Application</span></span> | <span data-ttu-id="829ed-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="829ed-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="829ed-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="829ed-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="829ed-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="829ed-119">Request body</span></span>

<span data-ttu-id="829ed-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="829ed-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="829ed-121">示例</span><span class="sxs-lookup"><span data-stu-id="829ed-121">Example</span></span>

<span data-ttu-id="829ed-122">本示例还原由 `{item-id}` 和 `{version-id}` 标识的文件的一个版本。</span><span class="sxs-lookup"><span data-stu-id="829ed-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="829ed-123">响应</span><span class="sxs-lookup"><span data-stu-id="829ed-123">Response</span></span>

<span data-ttu-id="829ed-124">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="829ed-124">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
