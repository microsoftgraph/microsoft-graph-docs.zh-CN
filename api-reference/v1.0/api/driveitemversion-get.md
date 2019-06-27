---
title: 获取 DriveItemVersion 资源
description: 检索 DriveItem 的某个特定版本的元数据。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3884093837ccc9c213464de7262bad98298b7be8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268850"
---
# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="c542f-103">获取 DriveItemVersion 资源</span><span class="sxs-lookup"><span data-stu-id="c542f-103">Get a DriveItemVersion resource</span></span>

<span data-ttu-id="c542f-104">检索 [DriveItem](../resources/driveitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="c542f-104">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c542f-105">权限</span><span class="sxs-lookup"><span data-stu-id="c542f-105">Permissions</span></span>

<span data-ttu-id="c542f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c542f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c542f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c542f-108">Permission type</span></span>      | <span data-ttu-id="c542f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c542f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c542f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c542f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c542f-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c542f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c542f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c542f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c542f-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c542f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c542f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c542f-114">Application</span></span> | <span data-ttu-id="c542f-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c542f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="c542f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c542f-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="c542f-117">响应</span><span class="sxs-lookup"><span data-stu-id="c542f-117">Response</span></span>

<span data-ttu-id="c542f-118">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItemVersion](../resources/driveitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c542f-118">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="c542f-119">示例</span><span class="sxs-lookup"><span data-stu-id="c542f-119">Example</span></span>

<span data-ttu-id="c542f-120">本示例检索当前用户驱动器中的文件版本。</span><span class="sxs-lookup"><span data-stu-id="c542f-120">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="c542f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c542f-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="c542f-122">响应</span><span class="sxs-lookup"><span data-stu-id="c542f-122">Response</span></span>

<span data-ttu-id="c542f-123">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="c542f-123">This returns a collection of versions:</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c542f-124">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c542f-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c542f-125">C#</span><span class="sxs-lookup"><span data-stu-id="c542f-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-single-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c542f-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="c542f-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-single-version-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c542f-127">目标-C</span><span class="sxs-lookup"><span data-stu-id="c542f-127">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-single-version-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="c542f-128">注解</span><span class="sxs-lookup"><span data-stu-id="c542f-128">Remarks</span></span>

<span data-ttu-id="c542f-129">OneDrive 不保留文件以前版本的完整元数据。</span><span class="sxs-lookup"><span data-stu-id="c542f-129">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="c542f-130">当应用程序检索文件的可用版本列表时，将返回 [DriveItemVersion](../resources/driveitemversion.md) 资源，它提供有关特定版本的可用信息。</span><span class="sxs-lookup"><span data-stu-id="c542f-130">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitemversion-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/driveitemversion-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitemversion-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
