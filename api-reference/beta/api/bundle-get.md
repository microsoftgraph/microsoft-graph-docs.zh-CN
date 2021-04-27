---
author: JeremyKelley
title: 获取捆绑包
description: 获取 driveItems 捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b6f1619bbb169a92841d3999c43603860c0038fd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047789"
---
# <a name="get-bundle"></a><span data-ttu-id="c9058-103">获取捆绑包</span><span class="sxs-lookup"><span data-stu-id="c9058-103">Get bundle</span></span>

<span data-ttu-id="c9058-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9058-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9058-105">根据捆绑 [包的唯一][] ID 检索捆绑包的元数据。</span><span class="sxs-lookup"><span data-stu-id="c9058-105">Retrieve the metadata for a [bundle][] based on the bundle's unique ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9058-106">权限</span><span class="sxs-lookup"><span data-stu-id="c9058-106">Permissions</span></span>

<span data-ttu-id="c9058-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9058-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9058-109">Permission type</span></span>      | <span data-ttu-id="c9058-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c9058-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9058-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9058-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c9058-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9058-112">Not supported.</span></span>                             |
|<span data-ttu-id="c9058-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9058-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9058-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9058-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9058-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9058-115">Application</span></span>          | <span data-ttu-id="c9058-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9058-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="c9058-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9058-117">HTTP request</span></span>

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

<span data-ttu-id="c9058-118">由于捆绑包是项，因此可以使用 **items** 集合返回有关捆绑包的元数据。</span><span class="sxs-lookup"><span data-stu-id="c9058-118">Because bundles are items, you can use the **items** collection to return metadata about a bundle.</span></span>
<span data-ttu-id="c9058-119">您还可以使用 **bundles 集合** 作为方便，以确保收到响应中的捆绑包。</span><span class="sxs-lookup"><span data-stu-id="c9058-119">You can also use the **bundles** collection as a convenience to ensure you're getting a bundle in response.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c9058-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c9058-120">Optional query parameters</span></span>

<span data-ttu-id="c9058-121">可以使用 [OData查询参数][odata-parameters]限制通过此调用返回的对象的形状。</span><span class="sxs-lookup"><span data-stu-id="c9058-121">You can use the [OData query parameters][odata-parameters] to restrict the shape of the objects returned from this call.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9058-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9058-122">Request headers</span></span>
| <span data-ttu-id="c9058-123">名称</span><span class="sxs-lookup"><span data-stu-id="c9058-123">Name</span></span>          | <span data-ttu-id="c9058-124">说明</span><span class="sxs-lookup"><span data-stu-id="c9058-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="c9058-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9058-125">Authorization</span></span> | <span data-ttu-id="c9058-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="c9058-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="c9058-128">if-none-match</span><span class="sxs-lookup"><span data-stu-id="c9058-128">if-none-match</span></span> | <span data-ttu-id="c9058-129">eTag。</span><span class="sxs-lookup"><span data-stu-id="c9058-129">eTag.</span></span> <span data-ttu-id="c9058-130">可选。</span><span class="sxs-lookup"><span data-stu-id="c9058-130">Optional.</span></span> <span data-ttu-id="c9058-131">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="c9058-131">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="c9058-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9058-132">Request body</span></span>

<span data-ttu-id="c9058-133">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="c9058-133">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9058-134">响应</span><span class="sxs-lookup"><span data-stu-id="c9058-134">Response</span></span>

<span data-ttu-id="c9058-135">如果成功，此方法在响应正文中返回[driveItem。][driveItem] resource with the [bundle][bundle]</span><span class="sxs-lookup"><span data-stu-id="c9058-135">If successful, this method returns a [driveItem][driveItem] resource with the [bundle][bundle] in the response body.</span></span>

<span data-ttu-id="c9058-136">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="c9058-136">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="c9058-137">示例</span><span class="sxs-lookup"><span data-stu-id="c9058-137">Examples</span></span>

### <a name="example-1-get-a-bundle"></a><span data-ttu-id="c9058-138">示例 1：获取捆绑包</span><span class="sxs-lookup"><span data-stu-id="c9058-138">Example 1: Get a bundle</span></span>

#### <a name="request"></a><span data-ttu-id="c9058-139">请求</span><span class="sxs-lookup"><span data-stu-id="c9058-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c9058-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9058-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```
# <a name="c"></a>[<span data-ttu-id="c9058-141">C#</span><span class="sxs-lookup"><span data-stu-id="c9058-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9058-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9058-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9058-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9058-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9058-144">Java</span><span class="sxs-lookup"><span data-stu-id="c9058-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-metadata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c9058-145">响应</span><span class="sxs-lookup"><span data-stu-id="c9058-145">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
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

<span data-ttu-id="c9058-146">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c9058-146">The response object shown here might be shortened for readability.</span></span>

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a><span data-ttu-id="c9058-147">示例 2：在单个调用中获取捆绑包及其子项</span><span class="sxs-lookup"><span data-stu-id="c9058-147">Example 2: Get a bundle and its children in a single call</span></span>

<span data-ttu-id="c9058-148">可以使用查询字符串参数在检索捆绑包元数据的同一调用中包括捆绑 [`expand`](/graph/query-parameters) 包的子项。</span><span class="sxs-lookup"><span data-stu-id="c9058-148">You can use the [`expand`](/graph/query-parameters) query string parameter to include the children of a bundle in the same call as retrieving the metadata of a bundle.</span></span>

#### <a name="request"></a><span data-ttu-id="c9058-149">请求</span><span class="sxs-lookup"><span data-stu-id="c9058-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c9058-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9058-150">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```
# <a name="c"></a>[<span data-ttu-id="c9058-151">C#</span><span class="sxs-lookup"><span data-stu-id="c9058-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-and-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9058-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9058-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-and-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9058-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9058-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-and-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9058-154">Java</span><span class="sxs-lookup"><span data-stu-id="c9058-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-and-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c9058-155">响应</span><span class="sxs-lookup"><span data-stu-id="c9058-155">Response</span></span>

<span data-ttu-id="c9058-156">此调用将返回捆绑包元数据和捆绑包的子项列表。</span><span class="sxs-lookup"><span data-stu-id="c9058-156">This call will return the bundle metadata and a list of children of the bundle.</span></span>
<span data-ttu-id="c9058-157">如果捆绑包没有子项，它将返回空集合。</span><span class="sxs-lookup"><span data-stu-id="c9058-157">If the bundle has no children, it will return an empty collection.</span></span>

<span data-ttu-id="c9058-158">如果捆绑包中的子项数量大于默认页面大小 **，children@odata.nextLink** 属性将返回一个 URL，该 URL 可用于请求捆绑包中的下一页子页面。</span><span class="sxs-lookup"><span data-stu-id="c9058-158">If the number of children in the bundle is greater than the default page size, the **children@odata.nextLink** property will be returned with a URL that can be used to request the next page of children in the bundle.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
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

<span data-ttu-id="c9058-159">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c9058-159">The response object shown here might be shortened for readability.</span></span>


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters


<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about a bundle and its children in OneDrive",
  "keywords": "retrieve,item,bundle,metadata",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Get Bundle Metadata"
} -->


