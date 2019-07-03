---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 新建文件夹
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 06afd98f5928d18ff5b6ff2673e24f19265993a1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436317"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="d3cf2-102">在驱动器中新建文件夹</span><span class="sxs-lookup"><span data-stu-id="d3cf2-102">Create a new folder in a drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3cf2-103">使用指定的父项或路径在[驱动器](../resources/drive.md)中新建文件夹或 [DriveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="d3cf2-103">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3cf2-104">权限</span><span class="sxs-lookup"><span data-stu-id="d3cf2-104">Permissions</span></span>

<span data-ttu-id="d3cf2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3cf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3cf2-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3cf2-107">Permission type</span></span>      | <span data-ttu-id="d3cf2-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3cf2-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3cf2-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3cf2-109">Delegated (work or school account)</span></span> | <span data-ttu-id="d3cf2-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3cf2-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d3cf2-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3cf2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3cf2-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3cf2-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d3cf2-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3cf2-113">Application</span></span> | <span data-ttu-id="d3cf2-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3cf2-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3cf2-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3cf2-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="d3cf2-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3cf2-116">Request body</span></span>

<span data-ttu-id="d3cf2-117">在请求正文中，提供要创建的 [DriveItem](../resources/driveitem.md) 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3cf2-117">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="d3cf2-118">响应</span><span class="sxs-lookup"><span data-stu-id="d3cf2-118">Response</span></span>

<span data-ttu-id="d3cf2-119">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d3cf2-119">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3cf2-120">示例</span><span class="sxs-lookup"><span data-stu-id="d3cf2-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3cf2-121">请求</span><span class="sxs-lookup"><span data-stu-id="d3cf2-121">Request</span></span>

<span data-ttu-id="d3cf2-122">下面是请求在登录用户的 OneDrive 根文件夹下新建文件夹的示例。</span><span class="sxs-lookup"><span data-stu-id="d3cf2-122">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="d3cf2-123">`@microsoft.graph.conflictBehavior` 属性用于指示是否已存在具有相同名称的项，服务是否应在创建文件夹时选择新名称。</span><span class="sxs-lookup"><span data-stu-id="d3cf2-123">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d3cf2-124">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d3cf2-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-folder", "scopes": "files.readwrite" } -->

```http
POST /me/drive/root/children
Content-Type: application/json

{
  "name": "New Folder",
  "folder": { },
  "@microsoft.graph.conflictBehavior": "rename"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d3cf2-125">C#</span><span class="sxs-lookup"><span data-stu-id="d3cf2-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3cf2-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3cf2-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d3cf2-127">目标-C</span><span class="sxs-lookup"><span data-stu-id="d3cf2-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3cf2-128">响应</span><span class="sxs-lookup"><span data-stu-id="d3cf2-128">Response</span></span>

<span data-ttu-id="d3cf2-129">如果成功，此方法将新创建的文件夹返回为 [[DriveItem]][item-resource] 资源。</span><span class="sxs-lookup"><span data-stu-id="d3cf2-129">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "createdDateTime": "2016-09-20T14:34:00Z",
  "eTag": "343F1FBD-E9B3-4DDE-BCA7-D61AEAFF44E5,1",
  "id": "ACEA49D1-1444-45A9-A1CB-68B1B28AE491",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "lastModifiedDateTime": "2016-09-20T14:34:00Z",
  "name": "New Folder",
  "parentReference": {
    "driveId": "5FE38E3C-051C-4D55-9B83-8A437658275B",
    "id": "E67A8F34-B0AA-46E1-8FF7-0750A29553DF",
    "path": "/drive/root:/"
  },
  "size": 0,
  "folder": {
    "childCount": 0
  }
}
```

## <a name="error-response"></a><span data-ttu-id="d3cf2-130">错误响应</span><span class="sxs-lookup"><span data-stu-id="d3cf2-130">Error response</span></span>

<span data-ttu-id="d3cf2-131">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="d3cf2-131">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[folder-facet]: ../resources/folder.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a folder item in a drive.",
  "keywords": "create,folder,new item",
  "section": "documentation",
  "tocPath": "Items/Create folder",
  "suppressions": [
  ]
}
-->
