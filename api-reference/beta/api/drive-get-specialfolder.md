---
author: JeremyKelley
description: 使用特殊集合可以按名称访问特殊文件夹。
title: 获取特殊文件夹
localization_priority: Normal
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 48a20da153eaf1e74d34b2ecfa3b7c30f8a794aa
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236177"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="1b547-103">按名称获取特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="1b547-103">Get a special folder by name</span></span>

<span data-ttu-id="1b547-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b547-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b547-105">使用特殊集合可以按名称访问特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="1b547-105">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="1b547-p101">特殊文件夹可以提供简单别名来访问 OneDrive 中的已知文件夹，无需按路径查找（需要本地化）或通过 ID 引用文件夹。如果特殊文件夹被重命名或移到驱动器中的其他位置，此语法将继续查找该文件夹。</span><span class="sxs-lookup"><span data-stu-id="1b547-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="1b547-p102">应用程序第一次尝试向特殊文件夹中写入内容时，如果特殊文件夹不存在，系统会自动创建特殊文件夹。如果用户删除某个特殊文件夹，再次向其写入内容时会重新创建特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="1b547-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="1b547-110">**注意：** 如果你拥有只读权限并且请求不存在的特殊文件夹，将收到 `403 Forbidden` 错误。</span><span class="sxs-lookup"><span data-stu-id="1b547-110">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b547-111">权限</span><span class="sxs-lookup"><span data-stu-id="1b547-111">Permissions</span></span>

<span data-ttu-id="1b547-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b547-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="1b547-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b547-114">Permission type</span></span>             |                                           <span data-ttu-id="1b547-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b547-115">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1b547-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b547-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b547-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b547-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="1b547-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b547-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b547-119">Files.ReadWrite.AppFolder、Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b547-119">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="1b547-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b547-120">Application</span></span>                            | <span data-ttu-id="1b547-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b547-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="1b547-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b547-122">HTTP Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1b547-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b547-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/special/{name}
```
# <a name="c"></a>[<span data-ttu-id="1b547-124">C#</span><span class="sxs-lookup"><span data-stu-id="1b547-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b547-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b547-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b547-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b547-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b547-127">Java</span><span class="sxs-lookup"><span data-stu-id="1b547-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-special-folder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="special-folder-names"></a><span data-ttu-id="1b547-128">特殊文件夹名称</span><span class="sxs-lookup"><span data-stu-id="1b547-128">Special folder names</span></span>
[!INCLUDE [files-special-folder-list](../includes/files-special-folder-list.md)]


### <a name="optional-query-parameters"></a><span data-ttu-id="1b547-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1b547-129">Optional query parameters</span></span>

<span data-ttu-id="1b547-130">此方法支持使用 `$expand` 和 `$select` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1b547-130">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="1b547-131">响应</span><span class="sxs-lookup"><span data-stu-id="1b547-131">Response</span></span>

<span data-ttu-id="1b547-132">此方法在响应正文中返回 `200 OK` 响应代码和 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1b547-132">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="1b547-133">可以将此处理特殊文件夹内联的方法与对 driveItem 上的属性或关系的其他调用结合使用。</span><span class="sxs-lookup"><span data-stu-id="1b547-133">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

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

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="1b547-134">获取特殊文件夹的子文件夹</span><span class="sxs-lookup"><span data-stu-id="1b547-134">Get children of a special folder</span></span>

<span data-ttu-id="1b547-135">若要请求特殊文件夹的子文件夹，则可以请求 `children` 集合，或使用 [expand](/graph/query-parameters) 选项展开子集合。</span><span class="sxs-lookup"><span data-stu-id="1b547-135">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="1b547-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b547-136">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="1b547-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b547-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/special/{name}/children
```
# <a name="c"></a>[<span data-ttu-id="1b547-138">C#</span><span class="sxs-lookup"><span data-stu-id="1b547-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b547-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b547-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b547-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b547-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b547-141">Java</span><span class="sxs-lookup"><span data-stu-id="1b547-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-special-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1b547-142">响应</span><span class="sxs-lookup"><span data-stu-id="1b547-142">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="1b547-143">说明</span><span class="sxs-lookup"><span data-stu-id="1b547-143">Remarks</span></span>

> <span data-ttu-id="1b547-144">**注意：** 带有 `specialFolder` facet 的 DriveItem 指示项目是特殊文件夹，且可以通过 `special` 集合访问。</span><span class="sxs-lookup"><span data-stu-id="1b547-144">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="1b547-145">如果应用拥有只读权限，且特殊文件夹尚不存在，那么可能无法请求获取特殊文件夹或其子项，响应为 `404 Not Found` 或 `403 Forbidden` 错误。</span><span class="sxs-lookup"><span data-stu-id="1b547-145">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
  ]
}
-->


