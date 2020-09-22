---
author: JeremyKelley
ms.author: jeremyke
title: 获取捆绑包
description: 获取 Driveitem 的捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 810f7c87effc14d2d62ad2039354754331da3ceb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987783"
---
# <a name="get-bundle"></a><span data-ttu-id="0a798-103">获取捆绑包</span><span class="sxs-lookup"><span data-stu-id="0a798-103">Get bundle</span></span>

<span data-ttu-id="0a798-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a798-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a798-105">根据捆绑包的唯一 ID 检索 [捆绑][] 的元数据。</span><span class="sxs-lookup"><span data-stu-id="0a798-105">Retrieve the metadata for a [bundle][] based on the bundle's unique ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a798-106">权限</span><span class="sxs-lookup"><span data-stu-id="0a798-106">Permissions</span></span>

<span data-ttu-id="0a798-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a798-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a798-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a798-109">Permission type</span></span>      | <span data-ttu-id="0a798-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a798-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a798-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a798-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0a798-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a798-112">Not supported.</span></span>                             |
|<span data-ttu-id="0a798-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a798-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a798-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a798-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a798-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a798-115">Application</span></span>          | <span data-ttu-id="0a798-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a798-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="0a798-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a798-117">HTTP request</span></span>

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

<span data-ttu-id="0a798-118">由于捆绑包是项，因此可以使用 **items** 集合返回有关捆绑包的元数据。</span><span class="sxs-lookup"><span data-stu-id="0a798-118">Because bundles are items, you can use the **items** collection to return metadata about a bundle.</span></span>
<span data-ttu-id="0a798-119">你也可以使用 **捆绑包** 集合来确保你在响应时获得捆绑包。</span><span class="sxs-lookup"><span data-stu-id="0a798-119">You can also use the **bundles** collection as a convenience to ensure you're getting a bundle in response.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="0a798-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0a798-120">Optional query parameters</span></span>

<span data-ttu-id="0a798-121">可以使用 [OData查询参数][odata-parameters]限制通过此调用返回的对象的形状。</span><span class="sxs-lookup"><span data-stu-id="0a798-121">You can use the [OData query parameters][odata-parameters] to restrict the shape of the objects returned from this call.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a798-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a798-122">Request headers</span></span>
| <span data-ttu-id="0a798-123">名称</span><span class="sxs-lookup"><span data-stu-id="0a798-123">Name</span></span>          | <span data-ttu-id="0a798-124">说明</span><span class="sxs-lookup"><span data-stu-id="0a798-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="0a798-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a798-125">Authorization</span></span> | <span data-ttu-id="0a798-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="0a798-126">Bearer \{token\}.</span></span> <span data-ttu-id="0a798-127">必需。</span><span class="sxs-lookup"><span data-stu-id="0a798-127">Required.</span></span> |
| <span data-ttu-id="0a798-128">if-none-match</span><span class="sxs-lookup"><span data-stu-id="0a798-128">if-none-match</span></span> | <span data-ttu-id="0a798-129">eTag.</span><span class="sxs-lookup"><span data-stu-id="0a798-129">eTag.</span></span> <span data-ttu-id="0a798-130">可选。</span><span class="sxs-lookup"><span data-stu-id="0a798-130">Optional.</span></span> <span data-ttu-id="0a798-131">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="0a798-131">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="0a798-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a798-132">Request body</span></span>

<span data-ttu-id="0a798-133">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a798-133">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a798-134">响应</span><span class="sxs-lookup"><span data-stu-id="0a798-134">Response</span></span>

<span data-ttu-id="0a798-135">如果成功，此方法[driveItem][driveItem] resource with the [bundle][bundle] 在响应正文中返回 driveItem。</span><span class="sxs-lookup"><span data-stu-id="0a798-135">If successful, this method returns a [driveItem][driveItem] resource with the [bundle][bundle] in the response body.</span></span>

<span data-ttu-id="0a798-136">阅读 " [错误响应][error-response] " 主题，了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0a798-136">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="0a798-137">示例</span><span class="sxs-lookup"><span data-stu-id="0a798-137">Examples</span></span>

### <a name="example-1-get-a-bundle"></a><span data-ttu-id="0a798-138">示例1：获取捆绑包</span><span class="sxs-lookup"><span data-stu-id="0a798-138">Example 1: Get a bundle</span></span>

#### <a name="request"></a><span data-ttu-id="0a798-139">请求</span><span class="sxs-lookup"><span data-stu-id="0a798-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0a798-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a798-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```
# <a name="c"></a>[<span data-ttu-id="0a798-141">C#</span><span class="sxs-lookup"><span data-stu-id="0a798-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a798-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a798-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a798-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a798-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0a798-144">响应</span><span class="sxs-lookup"><span data-stu-id="0a798-144">Response</span></span>

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

<span data-ttu-id="0a798-145">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0a798-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0a798-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0a798-146">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a><span data-ttu-id="0a798-147">示例2：在单个调用中获取捆绑包及其子项</span><span class="sxs-lookup"><span data-stu-id="0a798-147">Example 2: Get a bundle and its children in a single call</span></span>

<span data-ttu-id="0a798-148">您可以使用 [`expand`](/graph/query-parameters) 查询字符串参数在与检索捆绑的元数据的相同调用中添加捆绑包的子项。</span><span class="sxs-lookup"><span data-stu-id="0a798-148">You can use the [`expand`](/graph/query-parameters) query string parameter to include the children of a bundle in the same call as retrieving the metadata of a bundle.</span></span>

#### <a name="request"></a><span data-ttu-id="0a798-149">请求</span><span class="sxs-lookup"><span data-stu-id="0a798-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0a798-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a798-150">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```
# <a name="c"></a>[<span data-ttu-id="0a798-151">C#</span><span class="sxs-lookup"><span data-stu-id="0a798-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-and-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a798-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a798-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-and-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a798-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a798-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-and-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0a798-154">响应</span><span class="sxs-lookup"><span data-stu-id="0a798-154">Response</span></span>

<span data-ttu-id="0a798-155">此调用将返回捆绑包元数据和捆绑的子项列表。</span><span class="sxs-lookup"><span data-stu-id="0a798-155">This call will return the bundle metadata and a list of children of the bundle.</span></span>
<span data-ttu-id="0a798-156">如果捆绑包没有任何子级，则将返回一个空集合。</span><span class="sxs-lookup"><span data-stu-id="0a798-156">If the bundle has no children, it will return an empty collection.</span></span>

<span data-ttu-id="0a798-157">如果捆绑包中的子项数量大于默认页面大小，则将使用可用于请求捆绑中的下一页子页面的 URL 返回 **children@odata 的 nextLink** 属性。</span><span class="sxs-lookup"><span data-stu-id="0a798-157">If the number of children in the bundle is greater than the default page size, the **children@odata.nextLink** property will be returned with a URL that can be used to request the next page of children in the bundle.</span></span>

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

<span data-ttu-id="0a798-158">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0a798-158">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0a798-159">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0a798-159">All the properties will be returned from an actual call.</span></span>


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


