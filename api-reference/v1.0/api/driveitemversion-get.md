---
title: 获取 DriveItemVersion 资源
description: 检索 DriveItem 的某个特定版本的元数据。
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: 74076a044dcab00fc25dfe829eaee582d9a0d6b6
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516778"
---
# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="b19a6-103">获取 DriveItemVersion 资源</span><span class="sxs-lookup"><span data-stu-id="b19a6-103">Get a DriveItemVersion resource</span></span>

<span data-ttu-id="b19a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b19a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b19a6-105">检索 [DriveItem](../resources/driveitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="b19a6-105">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b19a6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b19a6-106">Permissions</span></span>

<span data-ttu-id="b19a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b19a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b19a6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b19a6-109">Permission type</span></span>      | <span data-ttu-id="b19a6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b19a6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b19a6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b19a6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b19a6-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b19a6-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b19a6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b19a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b19a6-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b19a6-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b19a6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b19a6-115">Application</span></span> | <span data-ttu-id="b19a6-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b19a6-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="b19a6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b19a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/items/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="b19a6-118">响应</span><span class="sxs-lookup"><span data-stu-id="b19a6-118">Response</span></span>

<span data-ttu-id="b19a6-119">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItemVersion](../resources/driveitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b19a6-119">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="b19a6-120">示例</span><span class="sxs-lookup"><span data-stu-id="b19a6-120">Example</span></span>

<span data-ttu-id="b19a6-121">本示例检索当前用户驱动器中的文件版本。</span><span class="sxs-lookup"><span data-stu-id="b19a6-121">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="b19a6-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b19a6-122">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="b19a6-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="b19a6-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions/{version-id}
```
# <a name="c"></a>[<span data-ttu-id="b19a6-124">C#</span><span class="sxs-lookup"><span data-stu-id="b19a6-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b19a6-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b19a6-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b19a6-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b19a6-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b19a6-127">Java</span><span class="sxs-lookup"><span data-stu-id="b19a6-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-single-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b19a6-128">响应</span><span class="sxs-lookup"><span data-stu-id="b19a6-128">Response</span></span>

<span data-ttu-id="b19a6-129">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="b19a6-129">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="b19a6-130">注解</span><span class="sxs-lookup"><span data-stu-id="b19a6-130">Remarks</span></span>

<span data-ttu-id="b19a6-131">OneDrive 不保留文件以前版本的完整元数据。</span><span class="sxs-lookup"><span data-stu-id="b19a6-131">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="b19a6-132">当应用程序检索文件的可用版本列表时，将返回 [DriveItemVersion](../resources/driveitemversion.md) 资源，它提供有关特定版本的可用信息。</span><span class="sxs-lookup"><span data-stu-id="b19a6-132">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->

