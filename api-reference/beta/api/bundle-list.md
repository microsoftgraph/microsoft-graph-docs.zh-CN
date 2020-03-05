---
author: JeremyKelley
ms.author: jeremyke
title: 列出捆绑包
description: 列出用户驱动器中的捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 52d03febbb44448081c1a9f69066254e639d361b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441044"
---
# <a name="list-bundles"></a><span data-ttu-id="b93d1-103">列出捆绑包</span><span class="sxs-lookup"><span data-stu-id="b93d1-103">List bundles</span></span>

<span data-ttu-id="b93d1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b93d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b93d1-105">获取用户驱动器中[所有捆绑][包]的列表。</span><span class="sxs-lookup"><span data-stu-id="b93d1-105">Get a list of all the [bundles][bundle] in a user's drive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b93d1-106">权限</span><span class="sxs-lookup"><span data-stu-id="b93d1-106">Permissions</span></span>

<span data-ttu-id="b93d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b93d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b93d1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b93d1-109">Permission type</span></span>      | <span data-ttu-id="b93d1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b93d1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b93d1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b93d1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b93d1-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b93d1-112">Not supported.</span></span>                             |
|<span data-ttu-id="b93d1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b93d1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b93d1-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b93d1-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b93d1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b93d1-115">Application</span></span>          | <span data-ttu-id="b93d1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b93d1-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="b93d1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b93d1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/bundles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b93d1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b93d1-118">Optional query parameters</span></span>

<span data-ttu-id="b93d1-119">此方法支持使用 [OData 查询参数][]筛选响应和生成响应形状。</span><span class="sxs-lookup"><span data-stu-id="b93d1-119">This method supports the [OData Query Parameters][] to filter and shape the response.</span></span>

<span data-ttu-id="b93d1-120">枚举绑定时不`expand=children`能使用查询参数。</span><span class="sxs-lookup"><span data-stu-id="b93d1-120">You can't use the `expand=children` query parameter when enumerating bundles.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b93d1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b93d1-121">Request headers</span></span>

| <span data-ttu-id="b93d1-122">名称</span><span class="sxs-lookup"><span data-stu-id="b93d1-122">Name</span></span>          | <span data-ttu-id="b93d1-123">说明</span><span class="sxs-lookup"><span data-stu-id="b93d1-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="b93d1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b93d1-124">Authorization</span></span> | <span data-ttu-id="b93d1-125">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="b93d1-125">Bearer \{token\}.</span></span> <span data-ttu-id="b93d1-126">必填。</span><span class="sxs-lookup"><span data-stu-id="b93d1-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b93d1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b93d1-127">Request body</span></span>

<span data-ttu-id="b93d1-128">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="b93d1-128">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="b93d1-129">响应</span><span class="sxs-lookup"><span data-stu-id="b93d1-129">Response</span></span>

<span data-ttu-id="b93d1-130">如果成功，此请求将返回为驱动器定义的捆绑包项的列表。</span><span class="sxs-lookup"><span data-stu-id="b93d1-130">If successful, this request returns the list of bundle items defined for the drive.</span></span>

<span data-ttu-id="b93d1-131">阅读 "[错误响应][error-response]" 主题，了解有关如何返回错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b93d1-131">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="b93d1-132">示例</span><span class="sxs-lookup"><span data-stu-id="b93d1-132">Examples</span></span>

### <a name="example-1-list-all-bundles-in-a-drive"></a><span data-ttu-id="b93d1-133">示例1：列出驱动器中的所有捆绑包</span><span class="sxs-lookup"><span data-stu-id="b93d1-133">Example 1: List all bundles in a drive</span></span>

<span data-ttu-id="b93d1-134">若要请求对驱动器中定义的所有绑定的枚举，可以向不带任何参数的**束**集合发出请求。</span><span class="sxs-lookup"><span data-stu-id="b93d1-134">To request an enumeration of all bundles defined in the drive, you can make a request to the **bundles** collection without any parameters.</span></span>

#### <a name="request"></a><span data-ttu-id="b93d1-135">请求</span><span class="sxs-lookup"><span data-stu-id="b93d1-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b93d1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b93d1-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-all-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles
```
# <a name="c"></a>[<span data-ttu-id="b93d1-137">C#</span><span class="sxs-lookup"><span data-stu-id="b93d1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-all-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b93d1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b93d1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-all-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b93d1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b93d1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-all-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b93d1-140">响应</span><span class="sxs-lookup"><span data-stu-id="b93d1-140">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "0120310201abd",
      "name": "Family shared files",
      "bundle": {
        "childCount": 1
      }
    }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="b93d1-141">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b93d1-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b93d1-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b93d1-142">All the properties will be returned from an actual call.</span></span>


### <a name="example-2-list-all-photo-albums-in-a-drive"></a><span data-ttu-id="b93d1-143">示例2：列出驱动器中的所有相册</span><span class="sxs-lookup"><span data-stu-id="b93d1-143">Example 2: List all photo albums in a drive</span></span>

<span data-ttu-id="b93d1-144">若要筛选从请求返回到捆绑包集合的捆绑包列表，可以使用`filter`查询字符串参数指定要返回的捆绑包的类型，方法是检查捆绑包中是否存在某一 facet：</span><span class="sxs-lookup"><span data-stu-id="b93d1-144">To filter the list of bundles returned from a request to the bundles collection, you can use the `filter` query string parameter to specify the type of bundle to return by checking for the existence of a facet on the bundle:</span></span>

#### <a name="request"></a><span data-ttu-id="b93d1-145">请求</span><span class="sxs-lookup"><span data-stu-id="b93d1-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b93d1-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="b93d1-146">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "list-album-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles?filter=bundle/album%20ne%20null
```
# <a name="c"></a>[<span data-ttu-id="b93d1-147">C#</span><span class="sxs-lookup"><span data-stu-id="b93d1-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-album-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b93d1-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b93d1-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-album-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b93d1-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b93d1-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-album-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b93d1-150">响应</span><span class="sxs-lookup"><span data-stu-id="b93d1-150">Response</span></span>

<span data-ttu-id="b93d1-151">对绑定终结点的 GET 响应是具有[捆绑包][]的[driveItem][]资源的数组。</span><span class="sxs-lookup"><span data-stu-id="b93d1-151">The response to a GET to the bundles endpoint is an array of [driveItem][] resources with the [bundle][].</span></span>
<span data-ttu-id="b93d1-152">由于所有捆绑包都是项目，因此可以对其使用所有的标准项操作。</span><span class="sxs-lookup"><span data-stu-id="b93d1-152">Because all bundles are items, you can use use all the standard item operations on them.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "120301010abcd",
      "name": "Seattle Center event",
      "bundle": {
        "childCount": 4,
        "album": { }
      },
      "tags": [
        {
          "name": "outside",
          "autoTagged": { }
        }
      ]
    }
  ]
}
```

<span data-ttu-id="b93d1-153">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b93d1-153">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b93d1-154">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b93d1-154">All the properties will be returned from an actual call.</span></span>


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[OData 查询参数]: /graph/query-parameters
[OData Query Parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "List the bundles in a drive.",
  "keywords": "list,bundle,collection",
  "section": "documentation",
  "tocPath": "Bundles/List"
} -->
