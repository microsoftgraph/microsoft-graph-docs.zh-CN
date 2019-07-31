---
author: JeremyKelley
ms.author: jeremyke
title: 创建捆绑包
description: 创建 Driveitem 的捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 342a03f7fad3b8919774296d8e7fa5562c49b30a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957302"
---
# <a name="create-bundle"></a><span data-ttu-id="4736f-103">创建捆绑包</span><span class="sxs-lookup"><span data-stu-id="4736f-103">Create bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4736f-104">将新的[捆绑包][]添加到用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="4736f-104">Add a new [bundle][] to the user's drive.</span></span>

[bundle]: ../resources/bundle.md

## <a name="permissions"></a><span data-ttu-id="4736f-106">权限</span><span class="sxs-lookup"><span data-stu-id="4736f-106">Permissions</span></span>

<span data-ttu-id="4736f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4736f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4736f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4736f-109">Permission type</span></span>      | <span data-ttu-id="4736f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4736f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4736f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4736f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4736f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="4736f-112">Not supported.</span></span>                             |
|<span data-ttu-id="4736f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4736f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4736f-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4736f-114">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="4736f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4736f-115">Application</span></span>          | <span data-ttu-id="4736f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4736f-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="4736f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4736f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a><span data-ttu-id="4736f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4736f-118">Request headers</span></span>

| <span data-ttu-id="4736f-119">名称</span><span class="sxs-lookup"><span data-stu-id="4736f-119">Name</span></span>          | <span data-ttu-id="4736f-120">说明</span><span class="sxs-lookup"><span data-stu-id="4736f-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="4736f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4736f-121">Authorization</span></span> | <span data-ttu-id="4736f-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="4736f-122">Bearer \{token\}.</span></span> <span data-ttu-id="4736f-123">必需。</span><span class="sxs-lookup"><span data-stu-id="4736f-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4736f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4736f-124">Request body</span></span>

<span data-ttu-id="4736f-125">在请求正文中, 提供要创建的捆绑包的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4736f-125">In the request body, supply a JSON representation of the bundle to be created.</span></span>

## <a name="response"></a><span data-ttu-id="4736f-126">响应</span><span class="sxs-lookup"><span data-stu-id="4736f-126">Response</span></span>

<span data-ttu-id="4736f-127">如果请求成功, 则返回表示新创建的捆绑包的[driveItem](../resources/driveitem.md) 。</span><span class="sxs-lookup"><span data-stu-id="4736f-127">If the request is successful, the [driveItem](../resources/driveitem.md) representing the newly created bundle will be returned.</span></span>

<span data-ttu-id="4736f-128">阅读 "[错误响应][error-response]" 主题, 了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4736f-128">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="4736f-129">示例</span><span class="sxs-lookup"><span data-stu-id="4736f-129">Examples</span></span>

### <a name="example-1-create-a-bundle"></a><span data-ttu-id="4736f-130">示例 1: 创建捆绑包</span><span class="sxs-lookup"><span data-stu-id="4736f-130">Example 1: Create a bundle</span></span>

<span data-ttu-id="4736f-131">下面的示例展示了如何创建基本的新包。</span><span class="sxs-lookup"><span data-stu-id="4736f-131">The following example shows how to create a basic new bundle.</span></span>
<span data-ttu-id="4736f-132">此请求将创建一个名为`Just some files`的新包, 并向捆绑包中添加两个现有项。</span><span class="sxs-lookup"><span data-stu-id="4736f-132">This request will create a new bundle named `Just some files` and add two existing items to the bundle.</span></span>
<span data-ttu-id="4736f-133">此捆绑包可用于与其他用户共享文件集合, 而不共享存储这些项目的文件夹。</span><span class="sxs-lookup"><span data-stu-id="4736f-133">This bundle can be used to share a collection of files with other users without sharing the folder those items are stored in.</span></span>

#### <a name="request"></a><span data-ttu-id="4736f-134">请求</span><span class="sxs-lookup"><span data-stu-id="4736f-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4736f-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4736f-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-bundle" } -->

```json
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "Just some files",
  "@name.conflictBehavior" : "rename",
  "bundle": { },
  "children": [
    { "id": "1234asdf" },
    { "id": "1234qwerty" }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4736f-136">C#</span><span class="sxs-lookup"><span data-stu-id="4736f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4736f-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="4736f-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4736f-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="4736f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4736f-139">Java</span><span class="sxs-lookup"><span data-stu-id="4736f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4736f-140">响应</span><span class="sxs-lookup"><span data-stu-id="4736f-140">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
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

<span data-ttu-id="4736f-141">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4736f-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4736f-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4736f-142">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-create-an-album"></a><span data-ttu-id="4736f-143">示例 2: 创建相册</span><span class="sxs-lookup"><span data-stu-id="4736f-143">Example 2: Create an album</span></span>

<span data-ttu-id="4736f-144">创建新相册的请求与此类似, 尽管在捆绑包 facet 中, 唱集属性设置为非 null 值。</span><span class="sxs-lookup"><span data-stu-id="4736f-144">The request to create a new photo album is similar, although inside the bundle facet, the album property is set to a non-null value.</span></span>

#### <a name="request"></a><span data-ttu-id="4736f-145">请求</span><span class="sxs-lookup"><span data-stu-id="4736f-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4736f-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4736f-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-album" } -->

```json
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "My Day at the Beach",
  "@name.conflictBehavior" : "rename",
  "bundle": { "album": {} },
  "children": [
    { "id": "1234asdf" }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4736f-147">C#</span><span class="sxs-lookup"><span data-stu-id="4736f-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-album-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4736f-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="4736f-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-album-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4736f-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="4736f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-album-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4736f-150">Java</span><span class="sxs-lookup"><span data-stu-id="4736f-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-album-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4736f-151">响应</span><span class="sxs-lookup"><span data-stu-id="4736f-151">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
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

<span data-ttu-id="4736f-152">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4736f-152">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4736f-153">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4736f-153">All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="4736f-154">@Microsoft 如果将_conflictBehavior_设置为**rename** , 并且已存在具有相同名称的捆绑, 则新的捆绑名称将更新为唯一。</span><span class="sxs-lookup"><span data-stu-id="4736f-154">If _@microsoft.graph.conflictBehavior_ is set to **rename** and a bundle with the same name already exists, the new bundle name will be updated to be unique.</span></span>
<span data-ttu-id="4736f-155">OneDrive 会将一个号码追加到捆绑包名称的末尾。</span><span class="sxs-lookup"><span data-stu-id="4736f-155">OneDrive will append a number to the end of the bundle name.</span></span>

<span data-ttu-id="4736f-156">例如，将把 `My Day at the Beach` 重命名为 `My Day at the Beach 1`。</span><span class="sxs-lookup"><span data-stu-id="4736f-156">For example, `My Day at the Beach` would be renamed `My Day at the Beach 1`.</span></span>
<span data-ttu-id="4736f-157">如果`My Day at the Beach 1`执行此操作, 则该数字将再次递增, 直到发现唯一的捆绑名称。</span><span class="sxs-lookup"><span data-stu-id="4736f-157">If `My Day at the Beach 1` is taken, then the number would be incremented again until a unique bundle name is discovered.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath": "Bundles/Create"
} -->
