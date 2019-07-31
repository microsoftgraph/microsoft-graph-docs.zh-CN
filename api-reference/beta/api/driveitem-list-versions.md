---
title: 列出 DriveItem 的版本
description: OneDrive 和 SharePoint 可以配置为保留文件的历史记录。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: ''
ms.openlocfilehash: aa9a02994173d508e71b782fa085438074af66de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957043"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="5d42a-103">列出 DriveItem 的版本</span><span class="sxs-lookup"><span data-stu-id="5d42a-103">Listing versions of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d42a-104">OneDrive 和 SharePoint 可以配置为保留文件的历史记录。</span><span class="sxs-lookup"><span data-stu-id="5d42a-104">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="5d42a-105">根据服务和配置，每次编辑都可以创建一个新版本，每次手动保存文件或永不保存。</span><span class="sxs-lookup"><span data-stu-id="5d42a-105">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="5d42a-106">文档之前的版本可能会保留有限的一段时间，具体取决于管理员设置，这对于每个用户或位置可能是唯一的。</span><span class="sxs-lookup"><span data-stu-id="5d42a-106">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d42a-107">权限</span><span class="sxs-lookup"><span data-stu-id="5d42a-107">Permissions</span></span>

<span data-ttu-id="5d42a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d42a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d42a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d42a-110">Permission type</span></span>      | <span data-ttu-id="5d42a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d42a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d42a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d42a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5d42a-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d42a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d42a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d42a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d42a-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d42a-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d42a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d42a-116">Application</span></span> | <span data-ttu-id="5d42a-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d42a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="5d42a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d42a-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="5d42a-119">响应</span><span class="sxs-lookup"><span data-stu-id="5d42a-119">Response</span></span>

<span data-ttu-id="5d42a-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItemVersion](../resources/driveitemversion.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5d42a-120">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="5d42a-121">示例</span><span class="sxs-lookup"><span data-stu-id="5d42a-121">Example</span></span>

<span data-ttu-id="5d42a-122">本示例检索当前用户驱动器中的文件的版本。</span><span class="sxs-lookup"><span data-stu-id="5d42a-122">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="5d42a-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d42a-123">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5d42a-124">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5d42a-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5d42a-125">C#</span><span class="sxs-lookup"><span data-stu-id="5d42a-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d42a-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="5d42a-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5d42a-127">目标-C</span><span class="sxs-lookup"><span data-stu-id="5d42a-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5d42a-128">Java</span><span class="sxs-lookup"><span data-stu-id="5d42a-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d42a-129">响应</span><span class="sxs-lookup"><span data-stu-id="5d42a-129">Response</span></span>

<span data-ttu-id="5d42a-130">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="5d42a-130">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
      "size": 123
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z",
      "size": 62
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z",
      "size": 16
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="5d42a-131">注解</span><span class="sxs-lookup"><span data-stu-id="5d42a-131">Remarks</span></span>

<span data-ttu-id="5d42a-132">OneDrive 不保留文件以前版本的完整元数据。</span><span class="sxs-lookup"><span data-stu-id="5d42a-132">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="5d42a-133">当应用程序检索文件的可用版本列表时，将返回 [DriveItemVersion](../resources/driveitemversion.md) 资源，它提供有关特定版本的可用信息。</span><span class="sxs-lookup"><span data-stu-id="5d42a-133">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
}
-->
