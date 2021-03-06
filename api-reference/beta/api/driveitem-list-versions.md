---
title: 列出 DriveItem 的版本
description: OneDrive 和 SharePoint 可以配置为保留文件的历史记录。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: 3f3c2135f84d5c4b5a71a7a2e003528a72edb8b0
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515533"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="8c34d-103">列出 DriveItem 的版本</span><span class="sxs-lookup"><span data-stu-id="8c34d-103">Listing versions of a DriveItem</span></span>

<span data-ttu-id="8c34d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c34d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c34d-105">OneDrive 和 SharePoint 可以配置为保留文件的历史记录。</span><span class="sxs-lookup"><span data-stu-id="8c34d-105">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="8c34d-106">根据服务和配置，每次编辑都可以创建一个新版本，每次手动保存文件或永不保存。</span><span class="sxs-lookup"><span data-stu-id="8c34d-106">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="8c34d-107">文档之前的版本可能会保留有限的一段时间，具体取决于管理员设置，这对于每个用户或位置可能是唯一的。</span><span class="sxs-lookup"><span data-stu-id="8c34d-107">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c34d-108">权限</span><span class="sxs-lookup"><span data-stu-id="8c34d-108">Permissions</span></span>

<span data-ttu-id="8c34d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c34d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c34d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c34d-111">Permission type</span></span>      | <span data-ttu-id="8c34d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c34d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c34d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c34d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8c34d-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c34d-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8c34d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c34d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c34d-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c34d-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8c34d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c34d-117">Application</span></span> | <span data-ttu-id="8c34d-118">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c34d-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="8c34d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c34d-119">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/items/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="8c34d-120">响应</span><span class="sxs-lookup"><span data-stu-id="8c34d-120">Response</span></span>

<span data-ttu-id="8c34d-121">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItemVersion](../resources/driveitemversion.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c34d-121">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="8c34d-122">示例</span><span class="sxs-lookup"><span data-stu-id="8c34d-122">Example</span></span>

<span data-ttu-id="8c34d-123">本示例检索当前用户驱动器中的文件的版本。</span><span class="sxs-lookup"><span data-stu-id="8c34d-123">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="8c34d-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c34d-124">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="8c34d-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c34d-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions
```
# <a name="c"></a>[<span data-ttu-id="8c34d-126">C#</span><span class="sxs-lookup"><span data-stu-id="8c34d-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c34d-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c34d-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c34d-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c34d-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c34d-129">Java</span><span class="sxs-lookup"><span data-stu-id="8c34d-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c34d-130">响应</span><span class="sxs-lookup"><span data-stu-id="8c34d-130">Response</span></span>

<span data-ttu-id="8c34d-131">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="8c34d-131">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="8c34d-132">注解</span><span class="sxs-lookup"><span data-stu-id="8c34d-132">Remarks</span></span>

<span data-ttu-id="8c34d-133">OneDrive 不保留文件以前版本的完整元数据。</span><span class="sxs-lookup"><span data-stu-id="8c34d-133">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="8c34d-134">当应用程序检索文件的可用版本列表时，将返回 [DriveItemVersion](../resources/driveitemversion.md) 资源，它提供有关特定版本的可用信息。</span><span class="sxs-lookup"><span data-stu-id="8c34d-134">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


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


