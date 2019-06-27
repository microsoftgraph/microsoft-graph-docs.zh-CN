---
title: 列出 DriveItem 的版本
description: OneDrive 和 SharePoint 可以配置为保留文件的历史记录。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 268e832fc40c7505dbfe072e46fb7f9e62c82b4d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260079"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="a03ef-103">列出 DriveItem 的版本</span><span class="sxs-lookup"><span data-stu-id="a03ef-103">Listing versions of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a03ef-104">OneDrive 和 SharePoint 可以配置为保留文件的历史记录。</span><span class="sxs-lookup"><span data-stu-id="a03ef-104">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="a03ef-105">根据服务和配置，每次编辑都可以创建一个新版本，每次手动保存文件或永不保存。</span><span class="sxs-lookup"><span data-stu-id="a03ef-105">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="a03ef-106">文档之前的版本可能会保留有限的一段时间，具体取决于管理员设置，这对于每个用户或位置可能是唯一的。</span><span class="sxs-lookup"><span data-stu-id="a03ef-106">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="a03ef-107">权限</span><span class="sxs-lookup"><span data-stu-id="a03ef-107">Permissions</span></span>

<span data-ttu-id="a03ef-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a03ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a03ef-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a03ef-110">Permission type</span></span>      | <span data-ttu-id="a03ef-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a03ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a03ef-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a03ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a03ef-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a03ef-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a03ef-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a03ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a03ef-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a03ef-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a03ef-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a03ef-116">Application</span></span> | <span data-ttu-id="a03ef-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a03ef-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="a03ef-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a03ef-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="a03ef-119">响应</span><span class="sxs-lookup"><span data-stu-id="a03ef-119">Response</span></span>

<span data-ttu-id="a03ef-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItemVersion](../resources/driveitemversion.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a03ef-120">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="a03ef-121">示例</span><span class="sxs-lookup"><span data-stu-id="a03ef-121">Example</span></span>

<span data-ttu-id="a03ef-122">本示例检索当前用户驱动器中的文件的版本。</span><span class="sxs-lookup"><span data-stu-id="a03ef-122">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="a03ef-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a03ef-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="a03ef-124">响应</span><span class="sxs-lookup"><span data-stu-id="a03ef-124">Response</span></span>

<span data-ttu-id="a03ef-125">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="a03ef-125">This returns a collection of versions:</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a03ef-126">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a03ef-126">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a03ef-127">C#</span><span class="sxs-lookup"><span data-stu-id="a03ef-127">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-previous-versions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a03ef-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="a03ef-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-previous-versions-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a03ef-129">目标-C</span><span class="sxs-lookup"><span data-stu-id="a03ef-129">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-previous-versions-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="a03ef-130">注解</span><span class="sxs-lookup"><span data-stu-id="a03ef-130">Remarks</span></span>

<span data-ttu-id="a03ef-131">OneDrive 不保留文件以前版本的完整元数据。</span><span class="sxs-lookup"><span data-stu-id="a03ef-131">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="a03ef-132">当应用程序检索文件的可用版本列表时，将返回 [DriveItemVersion](../resources/driveitemversion.md) 资源，它提供有关特定版本的可用信息。</span><span class="sxs-lookup"><span data-stu-id="a03ef-132">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
