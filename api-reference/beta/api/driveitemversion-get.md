---
title: 获取 DriveItemVersion 资源（预览）
description: 检索 DriveItem 的某个特定版本的元数据。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b9b5fae9013fcb2e6014f322d950aa831bafdb71
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325204"
---
# <a name="get-a-driveitemversion-resource-preview"></a><span data-ttu-id="ad1bc-103">获取 DriveItemVersion 资源（预览）</span><span class="sxs-lookup"><span data-stu-id="ad1bc-103">Get a DriveItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad1bc-104">检索 [DriveItem](../resources/driveitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="ad1bc-104">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad1bc-105">权限</span><span class="sxs-lookup"><span data-stu-id="ad1bc-105">Permissions</span></span>

<span data-ttu-id="ad1bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad1bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad1bc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad1bc-108">Permission type</span></span>      | <span data-ttu-id="ad1bc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad1bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad1bc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad1bc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad1bc-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad1bc-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad1bc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad1bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad1bc-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad1bc-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad1bc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad1bc-114">Application</span></span> | <span data-ttu-id="ad1bc-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad1bc-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="ad1bc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad1bc-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="ad1bc-117">响应</span><span class="sxs-lookup"><span data-stu-id="ad1bc-117">Response</span></span>

<span data-ttu-id="ad1bc-118">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItemVersion](../resources/driveitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ad1bc-118">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="ad1bc-119">示例</span><span class="sxs-lookup"><span data-stu-id="ad1bc-119">Example</span></span>

<span data-ttu-id="ad1bc-120">本示例检索当前用户驱动器中的文件版本。</span><span class="sxs-lookup"><span data-stu-id="ad1bc-120">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="ad1bc-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad1bc-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="ad1bc-122">响应</span><span class="sxs-lookup"><span data-stu-id="ad1bc-122">Response</span></span>

<span data-ttu-id="ad1bc-123">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="ad1bc-123">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="ad1bc-124">注解</span><span class="sxs-lookup"><span data-stu-id="ad1bc-124">Remarks</span></span>

<span data-ttu-id="ad1bc-125">OneDrive 不保留文件以前版本的完整元数据。</span><span class="sxs-lookup"><span data-stu-id="ad1bc-125">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="ad1bc-126">当应用程序检索文件的可用版本列表时，将返回 [DriveItemVersion](../resources/driveitemversion.md) 资源，它提供有关特定版本的可用信息。</span><span class="sxs-lookup"><span data-stu-id="ad1bc-126">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": []
}
-->
