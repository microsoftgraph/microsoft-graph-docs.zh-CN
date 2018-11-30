---
title: 获取 DriveItemVersion 资源（预览）
description: 检索 DriveItem 的某个特定版本的元数据。
ms.openlocfilehash: c78a81d1a5428bbb969f8761b238655ab7919e5a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043278"
---
# <a name="get-a-driveitemversion-resource-preview"></a><span data-ttu-id="3b8c4-103">获取 DriveItemVersion 资源（预览）</span><span class="sxs-lookup"><span data-stu-id="3b8c4-103">Get a DriveItemVersion resource (preview)</span></span>

> <span data-ttu-id="3b8c4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3b8c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b8c4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3b8c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b8c4-106">检索 [DriveItem](../resources/driveitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="3b8c4-106">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b8c4-107">权限</span><span class="sxs-lookup"><span data-stu-id="3b8c4-107">Permissions</span></span>

<span data-ttu-id="3b8c4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b8c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b8c4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b8c4-110">Permission type</span></span>      | <span data-ttu-id="3b8c4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b8c4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b8c4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b8c4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b8c4-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b8c4-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b8c4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b8c4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b8c4-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b8c4-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b8c4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b8c4-116">Application</span></span> | <span data-ttu-id="3b8c4-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b8c4-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="3b8c4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b8c4-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="3b8c4-119">响应</span><span class="sxs-lookup"><span data-stu-id="3b8c4-119">Response</span></span>

<span data-ttu-id="3b8c4-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItemVersion](../resources/driveitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b8c4-120">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="3b8c4-121">示例</span><span class="sxs-lookup"><span data-stu-id="3b8c4-121">Example</span></span>

<span data-ttu-id="3b8c4-122">本示例检索当前用户驱动器中的文件的版本。</span><span class="sxs-lookup"><span data-stu-id="3b8c4-122">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="3b8c4-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b8c4-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="3b8c4-124">响应</span><span class="sxs-lookup"><span data-stu-id="3b8c4-124">Response</span></span>

<span data-ttu-id="3b8c4-125">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="3b8c4-125">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "D4990684-58CE-4FAB-9B87-D6C49E74F298",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "size": 123
}
```

## <a name="remarks"></a><span data-ttu-id="3b8c4-126">注解</span><span class="sxs-lookup"><span data-stu-id="3b8c4-126">Remarks</span></span>

<span data-ttu-id="3b8c4-127">OneDrive 不保留文件以前版本的完整元数据。</span><span class="sxs-lookup"><span data-stu-id="3b8c4-127">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="3b8c4-128">当应用检索文件的可用版本列表时，将返回 [DriveItemVersion](../resources/driveitemversion.md) 资源，它提供有关特定版本的可用信息。</span><span class="sxs-lookup"><span data-stu-id="3b8c4-128">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
