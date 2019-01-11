---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 还原以前版本
localization_priority: Normal
ms.openlocfilehash: 6b325edc637779327390f34d6ebaab7dee2666cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813879"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="f3e30-102">还原 DriveItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="f3e30-102">Restore a previous version of a DriveItem</span></span>

> <span data-ttu-id="f3e30-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f3e30-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3e30-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f3e30-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3e30-105">将 DriveItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="f3e30-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="f3e30-106">这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="f3e30-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3e30-107">权限</span><span class="sxs-lookup"><span data-stu-id="f3e30-107">Permissions</span></span>

<span data-ttu-id="f3e30-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3e30-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3e30-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3e30-110">Permission type</span></span>      | <span data-ttu-id="f3e30-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3e30-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3e30-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3e30-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f3e30-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3e30-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3e30-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3e30-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3e30-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3e30-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3e30-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3e30-116">Application</span></span> | <span data-ttu-id="f3e30-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3e30-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3e30-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3e30-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="f3e30-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3e30-119">Request body</span></span>

<span data-ttu-id="f3e30-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="f3e30-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="f3e30-121">示例</span><span class="sxs-lookup"><span data-stu-id="f3e30-121">Example</span></span>

<span data-ttu-id="f3e30-122">本示例还原由 `{item-id}` 和 `{version-id}` 标识的文件的一个版本。</span><span class="sxs-lookup"><span data-stu-id="f3e30-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="f3e30-123">响应</span><span class="sxs-lookup"><span data-stu-id="f3e30-123">Response</span></span>

<span data-ttu-id="f3e30-124">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="f3e30-124">If successful, the API call returns a `204 No content`.</span></span>

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
