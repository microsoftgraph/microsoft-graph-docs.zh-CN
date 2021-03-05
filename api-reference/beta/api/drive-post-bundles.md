---
author: JeremyKelley
title: 创建捆绑包
description: 创建 driveItems 捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8883006a6aa1daf86e4d3b8a6efac31e0ae25376
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471381"
---
# <a name="create-bundle"></a><span data-ttu-id="a478f-103">创建捆绑包</span><span class="sxs-lookup"><span data-stu-id="a478f-103">Create bundle</span></span>

<span data-ttu-id="a478f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a478f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a478f-105">向用户 [驱动器][] 添加新捆绑包。</span><span class="sxs-lookup"><span data-stu-id="a478f-105">Add a new [bundle][] to the user's drive.</span></span>

[bundle]: ../resources/bundle.md

## <a name="permissions"></a><span data-ttu-id="a478f-107">权限</span><span class="sxs-lookup"><span data-stu-id="a478f-107">Permissions</span></span>

<span data-ttu-id="a478f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a478f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a478f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a478f-110">Permission type</span></span>      | <span data-ttu-id="a478f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a478f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a478f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a478f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a478f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a478f-113">Not supported.</span></span>                             |
|<span data-ttu-id="a478f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a478f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a478f-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a478f-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="a478f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a478f-116">Application</span></span>          | <span data-ttu-id="a478f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a478f-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="a478f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a478f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a><span data-ttu-id="a478f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a478f-119">Request headers</span></span>

| <span data-ttu-id="a478f-120">名称</span><span class="sxs-lookup"><span data-stu-id="a478f-120">Name</span></span>          | <span data-ttu-id="a478f-121">说明</span><span class="sxs-lookup"><span data-stu-id="a478f-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="a478f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a478f-122">Authorization</span></span> | <span data-ttu-id="a478f-123">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="a478f-123">Bearer \{token\}.</span></span> <span data-ttu-id="a478f-124">必填。</span><span class="sxs-lookup"><span data-stu-id="a478f-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a478f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a478f-125">Request body</span></span>

<span data-ttu-id="a478f-126">在请求正文中，提供要创建的捆绑包的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a478f-126">In the request body, supply a JSON representation of the bundle to be created.</span></span>

## <a name="response"></a><span data-ttu-id="a478f-127">响应</span><span class="sxs-lookup"><span data-stu-id="a478f-127">Response</span></span>

<span data-ttu-id="a478f-128">如果请求成功，将返回表示新创建的捆绑包的[driveItem。](../resources/driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="a478f-128">If the request is successful, the [driveItem](../resources/driveitem.md) representing the newly created bundle will be returned.</span></span>

<span data-ttu-id="a478f-129">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="a478f-129">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="a478f-130">示例</span><span class="sxs-lookup"><span data-stu-id="a478f-130">Examples</span></span>

### <a name="example-1-create-a-bundle"></a><span data-ttu-id="a478f-131">示例 1：创建捆绑包</span><span class="sxs-lookup"><span data-stu-id="a478f-131">Example 1: Create a bundle</span></span>

<span data-ttu-id="a478f-132">以下示例演示如何创建基本的新捆绑包。</span><span class="sxs-lookup"><span data-stu-id="a478f-132">The following example shows how to create a basic new bundle.</span></span>
<span data-ttu-id="a478f-133">此请求将创建一个名为的新捆绑包 `Just some files` ，并添加两个现有项到捆绑包。</span><span class="sxs-lookup"><span data-stu-id="a478f-133">This request will create a new bundle named `Just some files` and add two existing items to the bundle.</span></span>
<span data-ttu-id="a478f-134">此捆绑包可用于与其他用户共享文件集合，而无需共享存储这些项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="a478f-134">This bundle can be used to share a collection of files with other users without sharing the folder those items are stored in.</span></span>

#### <a name="request"></a><span data-ttu-id="a478f-135">请求</span><span class="sxs-lookup"><span data-stu-id="a478f-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a478f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a478f-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-bundle" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "Just some files",
  "@microsoft.graph.conflictBehavior" : "rename",
  "bundle": { },
  "children": [
    { "id": "1234asdf" },
    { "id": "1234qwerty" }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="a478f-137">C#</span><span class="sxs-lookup"><span data-stu-id="a478f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a478f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a478f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a478f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a478f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a478f-140">Java</span><span class="sxs-lookup"><span data-stu-id="a478f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a478f-141">响应</span><span class="sxs-lookup"><span data-stu-id="a478f-141">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2
  }
}
```

<span data-ttu-id="a478f-142">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a478f-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a478f-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a478f-143">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-create-an-album"></a><span data-ttu-id="a478f-144">示例 2：创建相册</span><span class="sxs-lookup"><span data-stu-id="a478f-144">Example 2: Create an album</span></span>

<span data-ttu-id="a478f-145">创建新相册的请求相似，尽管该相册属性在捆绑包 Facet 中设置为非 null 值。</span><span class="sxs-lookup"><span data-stu-id="a478f-145">The request to create a new photo album is similar, although inside the bundle facet, the album property is set to a non-null value.</span></span>

#### <a name="request"></a><span data-ttu-id="a478f-146">请求</span><span class="sxs-lookup"><span data-stu-id="a478f-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a478f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="a478f-147">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-album" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "My Day at the Beach",
  "@microsoft.graph.conflictBehavior" : "rename",
  "bundle": { "album": {} },
  "children": [
    { "id": "1234asdf" }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="a478f-148">C#</span><span class="sxs-lookup"><span data-stu-id="a478f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-album-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a478f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a478f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-album-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a478f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a478f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-album-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a478f-151">Java</span><span class="sxs-lookup"><span data-stu-id="a478f-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-album-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a478f-152">响应</span><span class="sxs-lookup"><span data-stu-id="a478f-152">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2,
    "album": { }
 }
}
```

<span data-ttu-id="a478f-153">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a478f-153">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a478f-154">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a478f-154">All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="a478f-155">如果 _@microsoft.graph.conflictBehavior_ 设置为重命名，并且已存在同名的捆绑包，则新的捆绑包名称将更新为唯一。</span><span class="sxs-lookup"><span data-stu-id="a478f-155">If _@microsoft.graph.conflictBehavior_ is set to **rename** and a bundle with the same name already exists, the new bundle name will be updated to be unique.</span></span>
<span data-ttu-id="a478f-156">OneDrive 将在捆绑包名称的末尾追加一个数字。</span><span class="sxs-lookup"><span data-stu-id="a478f-156">OneDrive will append a number to the end of the bundle name.</span></span>

<span data-ttu-id="a478f-157">例如，将把 `My Day at the Beach` 重命名为 `My Day at the Beach 1`。</span><span class="sxs-lookup"><span data-stu-id="a478f-157">For example, `My Day at the Beach` would be renamed `My Day at the Beach 1`.</span></span>
<span data-ttu-id="a478f-158">如果使用 `My Day at the Beach 1` ，则数字将再次递增，直到发现唯一的捆绑包名称。</span><span class="sxs-lookup"><span data-stu-id="a478f-158">If `My Day at the Beach 1` is taken, then the number would be incremented again until a unique bundle name is discovered.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath": "Bundles/Create"
} -->


