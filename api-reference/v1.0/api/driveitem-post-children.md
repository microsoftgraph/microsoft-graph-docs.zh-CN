---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 新建文件夹
localization_priority: Priority
ms.prod: sharepoint
description: 使用指定的父项或路径在驱动器中新建文件夹或 DriveItem。
doc_type: apiPageType
ms.openlocfilehash: a522ee90a09dabeba2cb5bf94a3393b8392e1c1d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015381"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="cb9ae-103">在驱动器中新建文件夹</span><span class="sxs-lookup"><span data-stu-id="cb9ae-103">Create a new folder in a drive</span></span>

<span data-ttu-id="cb9ae-104">使用指定的父项或路径在[驱动器](../resources/drive.md)中新建文件夹或 [DriveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="cb9ae-104">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb9ae-105">权限</span><span class="sxs-lookup"><span data-stu-id="cb9ae-105">Permissions</span></span>

<span data-ttu-id="cb9ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb9ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb9ae-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb9ae-108">Permission type</span></span>      | <span data-ttu-id="cb9ae-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb9ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb9ae-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb9ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb9ae-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb9ae-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb9ae-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb9ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb9ae-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb9ae-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb9ae-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb9ae-114">Application</span></span> | <span data-ttu-id="cb9ae-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb9ae-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb9ae-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb9ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="cb9ae-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb9ae-117">Request body</span></span>

<span data-ttu-id="cb9ae-118">在请求正文中，提供要创建的 [DriveItem](../resources/driveitem.md) 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb9ae-118">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="cb9ae-119">响应</span><span class="sxs-lookup"><span data-stu-id="cb9ae-119">Response</span></span>

<span data-ttu-id="cb9ae-120">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="cb9ae-120">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb9ae-121">示例</span><span class="sxs-lookup"><span data-stu-id="cb9ae-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb9ae-122">请求</span><span class="sxs-lookup"><span data-stu-id="cb9ae-122">Request</span></span>

<span data-ttu-id="cb9ae-123">下面是请求在登录用户的 OneDrive 根文件夹下新建文件夹的示例。</span><span class="sxs-lookup"><span data-stu-id="cb9ae-123">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="cb9ae-124">`@microsoft.graph.conflictBehavior` 属性用于指示是否已存在具有相同名称的项，服务是否应在创建文件夹时选择新名称。</span><span class="sxs-lookup"><span data-stu-id="cb9ae-124">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cb9ae-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb9ae-125">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="cb9ae-126">C#</span><span class="sxs-lookup"><span data-stu-id="cb9ae-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb9ae-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="cb9ae-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cb9ae-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb9ae-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cb9ae-129">Java</span><span class="sxs-lookup"><span data-stu-id="cb9ae-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-folder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cb9ae-130">响应</span><span class="sxs-lookup"><span data-stu-id="cb9ae-130">Response</span></span>

<span data-ttu-id="cb9ae-131">如果成功，此方法将新创建的文件夹返回为 [[DriveItem]][item-resource] 资源。</span><span class="sxs-lookup"><span data-stu-id="cb9ae-131">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

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

## <a name="error-response"></a><span data-ttu-id="cb9ae-132">错误响应</span><span class="sxs-lookup"><span data-stu-id="cb9ae-132">Error response</span></span>

<span data-ttu-id="cb9ae-133">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="cb9ae-133">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[folder-facet]: ../resources/folder.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a folder item in a drive.",
  "keywords": "create,folder,new item",
  "section": "documentation",
  "tocPath": "Items/Create folder",
  "suppressions": [
  ]
} -->
