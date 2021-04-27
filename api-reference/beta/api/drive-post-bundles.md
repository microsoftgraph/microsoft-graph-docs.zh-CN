---
author: JeremyKelley
title: 创建捆绑包
description: 创建 driveItems 捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 21312f78257fbd3c7c371e3c22e1ee03905402c1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046270"
---
# <a name="create-bundle"></a><span data-ttu-id="49fc4-103">创建捆绑包</span><span class="sxs-lookup"><span data-stu-id="49fc4-103">Create bundle</span></span>

<span data-ttu-id="49fc4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49fc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49fc4-105">将新 [捆绑包][] 添加到用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="49fc4-105">Add a new [bundle][] to the user's drive.</span></span>

[bundle]: ../resources/bundle.md

## <a name="permissions"></a><span data-ttu-id="49fc4-107">权限</span><span class="sxs-lookup"><span data-stu-id="49fc4-107">Permissions</span></span>

<span data-ttu-id="49fc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49fc4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="49fc4-110">Permission type</span></span>      | <span data-ttu-id="49fc4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49fc4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49fc4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49fc4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="49fc4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="49fc4-113">Not supported.</span></span>                             |
|<span data-ttu-id="49fc4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49fc4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49fc4-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49fc4-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="49fc4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="49fc4-116">Application</span></span>          | <span data-ttu-id="49fc4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="49fc4-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="49fc4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49fc4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a><span data-ttu-id="49fc4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="49fc4-119">Request headers</span></span>

| <span data-ttu-id="49fc4-120">名称</span><span class="sxs-lookup"><span data-stu-id="49fc4-120">Name</span></span>          | <span data-ttu-id="49fc4-121">说明</span><span class="sxs-lookup"><span data-stu-id="49fc4-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="49fc4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49fc4-122">Authorization</span></span> | <span data-ttu-id="49fc4-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="49fc4-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49fc4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="49fc4-125">Request body</span></span>

<span data-ttu-id="49fc4-126">在请求正文中，提供要创建的捆绑包的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49fc4-126">In the request body, supply a JSON representation of the bundle to be created.</span></span>

## <a name="response"></a><span data-ttu-id="49fc4-127">响应</span><span class="sxs-lookup"><span data-stu-id="49fc4-127">Response</span></span>

<span data-ttu-id="49fc4-128">如果请求成功，将返回表示新创建的捆绑包的[driveItem。](../resources/driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="49fc4-128">If the request is successful, the [driveItem](../resources/driveitem.md) representing the newly created bundle will be returned.</span></span>

<span data-ttu-id="49fc4-129">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="49fc4-129">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="49fc4-130">示例</span><span class="sxs-lookup"><span data-stu-id="49fc4-130">Examples</span></span>

### <a name="example-1-create-a-bundle"></a><span data-ttu-id="49fc4-131">示例 1：创建捆绑包</span><span class="sxs-lookup"><span data-stu-id="49fc4-131">Example 1: Create a bundle</span></span>

<span data-ttu-id="49fc4-132">以下示例演示如何创建基本的新捆绑包。</span><span class="sxs-lookup"><span data-stu-id="49fc4-132">The following example shows how to create a basic new bundle.</span></span>
<span data-ttu-id="49fc4-133">此请求将创建一个名为 的新捆绑包 `Just some files` ，并添加两个现有项到该捆绑包。</span><span class="sxs-lookup"><span data-stu-id="49fc4-133">This request will create a new bundle named `Just some files` and add two existing items to the bundle.</span></span>
<span data-ttu-id="49fc4-134">此捆绑包可用于与其他用户共享文件集合，而无需共享存储这些项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="49fc4-134">This bundle can be used to share a collection of files with other users without sharing the folder those items are stored in.</span></span>

#### <a name="request"></a><span data-ttu-id="49fc4-135">请求</span><span class="sxs-lookup"><span data-stu-id="49fc4-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="49fc4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="49fc4-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="49fc4-137">C#</span><span class="sxs-lookup"><span data-stu-id="49fc4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49fc4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49fc4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49fc4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49fc4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49fc4-140">Java</span><span class="sxs-lookup"><span data-stu-id="49fc4-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49fc4-141">响应</span><span class="sxs-lookup"><span data-stu-id="49fc4-141">Response</span></span>

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

<span data-ttu-id="49fc4-142">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="49fc4-142">The response object shown here might be shortened for readability.</span></span>

### <a name="example-2-create-an-album"></a><span data-ttu-id="49fc4-143">示例 2：创建相册</span><span class="sxs-lookup"><span data-stu-id="49fc4-143">Example 2: Create an album</span></span>

<span data-ttu-id="49fc4-144">创建新相册的请求相似，尽管在 bundle Facet 中，相册属性设置为非 null 值。</span><span class="sxs-lookup"><span data-stu-id="49fc4-144">The request to create a new photo album is similar, although inside the bundle facet, the album property is set to a non-null value.</span></span>

#### <a name="request"></a><span data-ttu-id="49fc4-145">请求</span><span class="sxs-lookup"><span data-stu-id="49fc4-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="49fc4-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="49fc4-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="49fc4-147">C#</span><span class="sxs-lookup"><span data-stu-id="49fc4-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-album-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49fc4-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49fc4-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-album-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49fc4-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49fc4-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-album-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49fc4-150">Java</span><span class="sxs-lookup"><span data-stu-id="49fc4-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-album-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49fc4-151">响应</span><span class="sxs-lookup"><span data-stu-id="49fc4-151">Response</span></span>

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

<span data-ttu-id="49fc4-152">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="49fc4-152">The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="49fc4-153">如果将 _@microsoft.graph.conflictBehavior_ 设置为 **rename，** 并且已存在同名的捆绑包，则新的捆绑包名称将更新为唯一。</span><span class="sxs-lookup"><span data-stu-id="49fc4-153">If _@microsoft.graph.conflictBehavior_ is set to **rename** and a bundle with the same name already exists, the new bundle name will be updated to be unique.</span></span>
<span data-ttu-id="49fc4-154">OneDrive将在捆绑包名称的末尾附加一个数字。</span><span class="sxs-lookup"><span data-stu-id="49fc4-154">OneDrive will append a number to the end of the bundle name.</span></span>

<span data-ttu-id="49fc4-155">例如，将把 `My Day at the Beach` 重命名为 `My Day at the Beach 1`。</span><span class="sxs-lookup"><span data-stu-id="49fc4-155">For example, `My Day at the Beach` would be renamed `My Day at the Beach 1`.</span></span>
<span data-ttu-id="49fc4-156">如果 `My Day at the Beach 1` 已取值，则数字将再次递增，直到发现唯一的捆绑包名称。</span><span class="sxs-lookup"><span data-stu-id="49fc4-156">If `My Day at the Beach 1` is taken, then the number would be incremented again until a unique bundle name is discovered.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Create"
} -->


