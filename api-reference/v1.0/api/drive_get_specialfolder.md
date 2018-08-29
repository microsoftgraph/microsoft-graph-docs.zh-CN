---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 获取特殊文件夹
ms.openlocfilehash: 42deedff6dc5a0925412e95af806fee99d8be242
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265034"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="74179-102">按名称获取特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="74179-102">Get a special folder by name</span></span>

<span data-ttu-id="74179-103">使用特殊集合可以按名称访问特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="74179-103">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="74179-p101">特殊文件夹可以提供简单别名来访问 OneDrive 中的已知文件夹，无需按路径查找（需要本地化）或通过 ID 引用文件夹。如果特殊文件夹被重命名或移到驱动器中的其他位置，此语法将继续查找该文件夹。</span><span class="sxs-lookup"><span data-stu-id="74179-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="74179-p102">应用程序第一次尝试向特殊文件夹中写入内容时，如果特殊文件夹不存在，系统会自动创建特殊文件夹。如果用户删除某个特殊文件夹，再次向其写入内容时会重新创建特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="74179-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="74179-108">**注意：** 如果你拥有只读权限并且请求不存在的特殊文件夹，将收到 `403 Forbidden` 错误。</span><span class="sxs-lookup"><span data-stu-id="74179-108">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="74179-109">权限</span><span class="sxs-lookup"><span data-stu-id="74179-109">Permissions</span></span>

<span data-ttu-id="74179-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="74179-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="74179-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="74179-112">Permission type</span></span>             |                                           <span data-ttu-id="74179-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74179-113">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="74179-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74179-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="74179-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74179-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="74179-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74179-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74179-117">Files.ReadWrite.AppFolder、Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74179-117">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="74179-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="74179-118">Application</span></span>                            | <span data-ttu-id="74179-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74179-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="74179-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74179-120">HTTP Request</span></span>

<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a><span data-ttu-id="74179-121">特殊文件夹名称</span><span class="sxs-lookup"><span data-stu-id="74179-121">Special folder names</span></span>

<span data-ttu-id="74179-122">以下是 OneDrive 和 OneDrive for Business 中可用的特殊文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="74179-122">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="74179-123">名称</span><span class="sxs-lookup"><span data-stu-id="74179-123">Name</span></span>        | <span data-ttu-id="74179-124">文件夹 ID</span><span class="sxs-lookup"><span data-stu-id="74179-124">Folder id</span></span>    | <span data-ttu-id="74179-125">说明</span><span class="sxs-lookup"><span data-stu-id="74179-125">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="74179-126">Documents</span><span class="sxs-lookup"><span data-stu-id="74179-126">Documents</span></span>   | `documents`  | <span data-ttu-id="74179-127">“文档”文件夹。</span><span class="sxs-lookup"><span data-stu-id="74179-127">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="74179-128">Photos</span><span class="sxs-lookup"><span data-stu-id="74179-128">Photos</span></span>      | `photos`     | <span data-ttu-id="74179-129">“照片”文件夹。</span><span class="sxs-lookup"><span data-stu-id="74179-129">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="74179-130">Camera Roll</span><span class="sxs-lookup"><span data-stu-id="74179-130">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="74179-131">“本机照片备份”文件夹。</span><span class="sxs-lookup"><span data-stu-id="74179-131">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="74179-132">App Root</span><span class="sxs-lookup"><span data-stu-id="74179-132">App Root</span></span>    | `approot`    | <span data-ttu-id="74179-p104">应用程序的个人文件夹。通常位于 `/Apps/{Application Name}` 中</span><span class="sxs-lookup"><span data-stu-id="74179-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="74179-135">Music</span><span class="sxs-lookup"><span data-stu-id="74179-135">Music</span></span>       | `music`      | <span data-ttu-id="74179-136">“音乐”文件夹。</span><span class="sxs-lookup"><span data-stu-id="74179-136">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="74179-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="74179-137">Optional query parameters</span></span>

<span data-ttu-id="74179-138">此方法支持使用 `$expand` 和 `$select` [OData 查询参数](../../../concepts/query_parameters.md)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="74179-138">This method supports the `$expand` and `$select` [OData query parameters](../../../concepts/query_parameters.md) to customize the response.</span></span>

## <a name="http-response"></a><span data-ttu-id="74179-139">HTTP 响应</span><span class="sxs-lookup"><span data-stu-id="74179-139">HTTP Response</span></span>

<span data-ttu-id="74179-140">此方法在响应正文中返回 `200 OK` 响应代码和 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74179-140">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="74179-141">你可以将此处理特殊文件夹内联的方法与对 driveItem 上的属性和关系的其他调用结合使用。</span><span class="sxs-lookup"><span data-stu-id="74179-141">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "Documents",
  "eTag": "012345819293.1",
  "specialFolder": {
    "name": "documents"
  }
}
```

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="74179-142">获取特殊文件夹的子文件夹</span><span class="sxs-lookup"><span data-stu-id="74179-142">Get children of a special folder</span></span>

<span data-ttu-id="74179-143">若要请求特殊文件夹的子文件夹，则可以请求 `children` 集合，或使用 [expand](../../../concepts/query_parameters.md) 选项展开子集合。</span><span class="sxs-lookup"><span data-stu-id="74179-143">To request the children of a special folder, you can request the `children` collection or use the [expand](../../../concepts/query_parameters.md) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="74179-144">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74179-144">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/special/{special-folder-name}/children
```

### <a name="http-response"></a><span data-ttu-id="74179-145">HTTP 响应</span><span class="sxs-lookup"><span data-stu-id="74179-145">HTTP response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048 },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="74179-146">备注</span><span class="sxs-lookup"><span data-stu-id="74179-146">Remarks</span></span>

> <span data-ttu-id="74179-147">**注意：** 带有 `specialFolder` facet 的 DriveItem 指示项目是特殊文件夹，且可以通过 `special` 集合访问。</span><span class="sxs-lookup"><span data-stu-id="74179-147">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="74179-148">如果应用拥有只读权限，且特殊文件夹尚不存在，那么可能无法请求获取特殊文件夹或其子项，响应为 `404 Not Found` 或 `403 Forbidden` 错误。</span><span class="sxs-lookup"><span data-stu-id="74179-148">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders"
} -->
