---
author: JeremyKelley
ms.author: jeremyke
title: 获取捆绑包
description: 获取 Driveitem 的捆绑包
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0be042c6f1ce3915db93faa135ba054a3cc6a34f
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932661"
---
# <a name="get-bundle"></a><span data-ttu-id="c772c-103">获取捆绑包</span><span class="sxs-lookup"><span data-stu-id="c772c-103">Get bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c772c-104">根据捆绑包的唯一 ID 检索[捆绑][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="c772c-104">Retrieve the metadata for a [bundle][] based on the bundle's unique ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="c772c-105">权限</span><span class="sxs-lookup"><span data-stu-id="c772c-105">Permissions</span></span>

<span data-ttu-id="c772c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c772c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c772c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c772c-108">Permission type</span></span>      | <span data-ttu-id="c772c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c772c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c772c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c772c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c772c-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="c772c-111">Not supported.</span></span>                             |
|<span data-ttu-id="c772c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c772c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c772c-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c772c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c772c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c772c-114">Application</span></span>          | <span data-ttu-id="c772c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c772c-115">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="c772c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c772c-116">HTTP request</span></span>

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

<span data-ttu-id="c772c-117">由于捆绑包是项, 因此可以使用**items**集合返回有关捆绑包的元数据。</span><span class="sxs-lookup"><span data-stu-id="c772c-117">Because bundles are items, you can use the **items** collection to return metadata about a bundle.</span></span>
<span data-ttu-id="c772c-118">你也可以使用**捆绑包**集合来确保你在响应时获得捆绑包。</span><span class="sxs-lookup"><span data-stu-id="c772c-118">You can also use the **bundles** collection as a convenience to ensure you're getting a bundle in response.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c772c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c772c-119">Optional query parameters</span></span>

<span data-ttu-id="c772c-120">可以使用 [OData查询参数][odata-parameters]限制通过此调用返回的对象的形状。</span><span class="sxs-lookup"><span data-stu-id="c772c-120">You can use the [OData query parameters][odata-parameters] to restrict the shape of the objects returned from this call.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c772c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c772c-121">Request headers</span></span>
| <span data-ttu-id="c772c-122">名称</span><span class="sxs-lookup"><span data-stu-id="c772c-122">Name</span></span>          | <span data-ttu-id="c772c-123">说明</span><span class="sxs-lookup"><span data-stu-id="c772c-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="c772c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c772c-124">Authorization</span></span> | <span data-ttu-id="c772c-125">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="c772c-125">Bearer \{token\}.</span></span> <span data-ttu-id="c772c-126">必需。</span><span class="sxs-lookup"><span data-stu-id="c772c-126">Required.</span></span> |
| <span data-ttu-id="c772c-127">if-none-match</span><span class="sxs-lookup"><span data-stu-id="c772c-127">if-none-match</span></span> | <span data-ttu-id="c772c-128">eTag.</span><span class="sxs-lookup"><span data-stu-id="c772c-128">eTag.</span></span> <span data-ttu-id="c772c-129">可选。</span><span class="sxs-lookup"><span data-stu-id="c772c-129">Optional.</span></span> <span data-ttu-id="c772c-130">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="c772c-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="c772c-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c772c-131">Request body</span></span>

<span data-ttu-id="c772c-132">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="c772c-132">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="c772c-133">响应</span><span class="sxs-lookup"><span data-stu-id="c772c-133">Response</span></span>

<span data-ttu-id="c772c-134">如果成功, 此方法在响应正文中返回[driveItem][driveItem] resource with the [bundle][bundle] 。</span><span class="sxs-lookup"><span data-stu-id="c772c-134">If successful, this method returns a [driveItem][driveItem] resource with the [bundle][bundle] in the response body.</span></span>

<span data-ttu-id="c772c-135">阅读 "[错误响应][error-response]" 主题, 了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c772c-135">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="c772c-136">示例</span><span class="sxs-lookup"><span data-stu-id="c772c-136">Examples</span></span>

### <a name="example-1-get-a-bundle"></a><span data-ttu-id="c772c-137">示例 1: 获取捆绑包</span><span class="sxs-lookup"><span data-stu-id="c772c-137">Example 1: Get a bundle</span></span>

#### <a name="request"></a><span data-ttu-id="c772c-138">请求</span><span class="sxs-lookup"><span data-stu-id="c772c-138">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c772c-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c772c-139">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```http
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c772c-140">C#</span><span class="sxs-lookup"><span data-stu-id="c772c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c772c-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="c772c-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c772c-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="c772c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c772c-143">Java</span><span class="sxs-lookup"><span data-stu-id="c772c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-metadata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c772c-144">响应</span><span class="sxs-lookup"><span data-stu-id="c772c-144">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "My Photo Album Bundle",
  "eTag": "etag",
  "cTag": "etag",
  "createdBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "createdDateTime": "datetime",
  "lastModifiedBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "lastModifiedDateTime": "datetime",
  "size": 1234,
  "webUrl": "http://onedrive.com/...",
  "bundle": {
    "childCount": 4,
     "album": { }
  }
}
```

<span data-ttu-id="c772c-145">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c772c-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c772c-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c772c-146">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a><span data-ttu-id="c772c-147">示例 2: 在单个调用中获取捆绑包及其子项</span><span class="sxs-lookup"><span data-stu-id="c772c-147">Example 2: Get a bundle and its children in a single call</span></span>

<span data-ttu-id="c772c-148">您可以使用[`expand`](/graph/query-parameters)查询字符串参数在与检索捆绑的元数据的相同调用中添加捆绑包的子项。</span><span class="sxs-lookup"><span data-stu-id="c772c-148">You can use the [`expand`](/graph/query-parameters) query string parameter to include the children of a bundle in the same call as retrieving the metadata of a bundle.</span></span>

#### <a name="request"></a><span data-ttu-id="c772c-149">请求</span><span class="sxs-lookup"><span data-stu-id="c772c-149">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c772c-150">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c772c-150">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```http
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c772c-151">C#</span><span class="sxs-lookup"><span data-stu-id="c772c-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-and-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c772c-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="c772c-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-and-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c772c-153">目标-C</span><span class="sxs-lookup"><span data-stu-id="c772c-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-and-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c772c-154">Java</span><span class="sxs-lookup"><span data-stu-id="c772c-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-and-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c772c-155">响应</span><span class="sxs-lookup"><span data-stu-id="c772c-155">Response</span></span>

<span data-ttu-id="c772c-156">此调用将返回捆绑包元数据和捆绑的子项列表。</span><span class="sxs-lookup"><span data-stu-id="c772c-156">This call will return the bundle metadata and a list of children of the bundle.</span></span>
<span data-ttu-id="c772c-157">如果捆绑包没有任何子级, 则将返回一个空集合。</span><span class="sxs-lookup"><span data-stu-id="c772c-157">If the bundle has no children, it will return an empty collection.</span></span>

<span data-ttu-id="c772c-158">如果捆绑包中的子项数量大于默认页面大小, 则将使用可用于请求捆绑中的下一页子页面的 URL 返回**子级 @ nextLink**属性。</span><span class="sxs-lookup"><span data-stu-id="c772c-158">If the number of children in the bundle is greater than the default page size, the **children@odata.nextLink** property will be returned with a URL that can be used to request the next page of children in the bundle.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "101230100alkc",
  "name": "My Cool Day at the Beach",
  "children": [
    { "id": "120100abab", "name": "image1.jpg", "file": {} },
    { "id": "120100abo1", "name": "image2.jpg", "file": {} }
  ],
  "children@odata.nextLink": "https://api.onedrive.com/v1.0/..."
}
```

<span data-ttu-id="c772c-159">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c772c-159">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c772c-160">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c772c-160">All the properties will be returned from an actual call.</span></span>


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters


<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about a bundle and its children in OneDrive",
  "keywords": "retrieve,item,bundle,metadata",
  "section": "documentation",
  "tocPath": "Bundles/Get Bundle Metadata"
} -->
