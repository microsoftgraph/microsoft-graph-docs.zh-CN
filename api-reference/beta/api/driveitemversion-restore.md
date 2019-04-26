---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 还原以前的版本
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b41e9c266242317151439101809958142124372f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325123"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="bcd1d-102">还原 DriveItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="bcd1d-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcd1d-103">将 DriveItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="bcd1d-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="bcd1d-104">这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="bcd1d-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcd1d-105">权限</span><span class="sxs-lookup"><span data-stu-id="bcd1d-105">Permissions</span></span>

<span data-ttu-id="bcd1d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bcd1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcd1d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bcd1d-108">Permission type</span></span>      | <span data-ttu-id="bcd1d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bcd1d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcd1d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bcd1d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bcd1d-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcd1d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bcd1d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bcd1d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcd1d-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcd1d-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="bcd1d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bcd1d-114">Application</span></span> | <span data-ttu-id="bcd1d-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcd1d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcd1d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bcd1d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="bcd1d-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="bcd1d-117">Request body</span></span>

<span data-ttu-id="bcd1d-118">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="bcd1d-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="bcd1d-119">示例</span><span class="sxs-lookup"><span data-stu-id="bcd1d-119">Example</span></span>

<span data-ttu-id="bcd1d-120">本示例还原由 `{item-id}` 和 `{version-id}` 标识的文件的一个版本。</span><span class="sxs-lookup"><span data-stu-id="bcd1d-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="bcd1d-121">响应</span><span class="sxs-lookup"><span data-stu-id="bcd1d-121">Response</span></span>

<span data-ttu-id="bcd1d-122">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="bcd1d-122">If successful, the API call returns a `204 No content`.</span></span>

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
  "suppressions": []
}
-->
