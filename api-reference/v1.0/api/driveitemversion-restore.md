---
title: 还原 DriveItem 的以前版本
description: 将 DriveItem 的以前版本还原为当前版本。 这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。
ms.openlocfilehash: e8272678e048391279d5b2147985d4f1e83f0456
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011021"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="f3230-104">还原 DriveItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="f3230-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="f3230-105">将 DriveItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="f3230-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="f3230-106">这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="f3230-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3230-107">权限</span><span class="sxs-lookup"><span data-stu-id="f3230-107">Permissions</span></span>

<span data-ttu-id="f3230-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3230-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3230-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3230-110">Permission type</span></span>      | <span data-ttu-id="f3230-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3230-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3230-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3230-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f3230-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3230-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3230-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3230-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3230-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3230-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3230-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3230-116">Application</span></span> | <span data-ttu-id="f3230-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3230-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3230-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3230-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="f3230-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3230-119">Request body</span></span>

<span data-ttu-id="f3230-120">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="f3230-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="f3230-121">示例</span><span class="sxs-lookup"><span data-stu-id="f3230-121">Example</span></span>

<span data-ttu-id="f3230-122">本示例还原由 `{item-id}` 和 `{version-id}` 标识的文件的一个版本。</span><span class="sxs-lookup"><span data-stu-id="f3230-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="f3230-123">响应</span><span class="sxs-lookup"><span data-stu-id="f3230-123">Response</span></span>

<span data-ttu-id="f3230-124">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="f3230-124">If successful, the API call returns a `204 No Content`.</span></span>

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
  "tocPath": "Items/Copy"
} -->
