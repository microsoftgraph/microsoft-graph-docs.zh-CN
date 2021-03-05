---
author: JeremyKelley
title: 列出捆绑包
description: 列出用户驱动器中的捆绑包
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: fafafbdef4f2fa8b6c2ba01f8544fa5f814f7672
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472718"
---
# <a name="list-bundles"></a><span data-ttu-id="e1120-103">列出捆绑包</span><span class="sxs-lookup"><span data-stu-id="e1120-103">List bundles</span></span>

<span data-ttu-id="e1120-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1120-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1120-105">获取用户驱动器 [中][所有] 捆绑包的列表。</span><span class="sxs-lookup"><span data-stu-id="e1120-105">Get a list of all the [bundles][bundle] in a user's drive.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1120-106">权限</span><span class="sxs-lookup"><span data-stu-id="e1120-106">Permissions</span></span>

<span data-ttu-id="e1120-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1120-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1120-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1120-109">Permission type</span></span>      | <span data-ttu-id="e1120-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1120-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1120-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1120-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e1120-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1120-112">Not supported.</span></span>                             |
|<span data-ttu-id="e1120-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1120-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1120-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1120-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1120-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1120-115">Application</span></span>          | <span data-ttu-id="e1120-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1120-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="e1120-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1120-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/bundles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1120-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e1120-118">Optional query parameters</span></span>

<span data-ttu-id="e1120-119">此方法支持使用 [OData 查询参数][]筛选响应和生成响应形状。</span><span class="sxs-lookup"><span data-stu-id="e1120-119">This method supports the [OData Query Parameters][] to filter and shape the response.</span></span>

<span data-ttu-id="e1120-120">枚举捆绑包 `expand=children` 时，不能使用查询参数。</span><span class="sxs-lookup"><span data-stu-id="e1120-120">You can't use the `expand=children` query parameter when enumerating bundles.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1120-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1120-121">Request headers</span></span>

| <span data-ttu-id="e1120-122">名称</span><span class="sxs-lookup"><span data-stu-id="e1120-122">Name</span></span>          | <span data-ttu-id="e1120-123">说明</span><span class="sxs-lookup"><span data-stu-id="e1120-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="e1120-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1120-124">Authorization</span></span> | <span data-ttu-id="e1120-125">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="e1120-125">Bearer \{token\}.</span></span> <span data-ttu-id="e1120-126">必填。</span><span class="sxs-lookup"><span data-stu-id="e1120-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1120-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1120-127">Request body</span></span>

<span data-ttu-id="e1120-128">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="e1120-128">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1120-129">响应</span><span class="sxs-lookup"><span data-stu-id="e1120-129">Response</span></span>

<span data-ttu-id="e1120-130">如果成功，此请求将返回为驱动器定义的捆绑包项列表。</span><span class="sxs-lookup"><span data-stu-id="e1120-130">If successful, this request returns the list of bundle items defined for the drive.</span></span>

<span data-ttu-id="e1120-131">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="e1120-131">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="e1120-132">示例</span><span class="sxs-lookup"><span data-stu-id="e1120-132">Examples</span></span>

### <a name="example-1-list-all-bundles-in-a-drive"></a><span data-ttu-id="e1120-133">示例 1：列出驱动器中所有捆绑包</span><span class="sxs-lookup"><span data-stu-id="e1120-133">Example 1: List all bundles in a drive</span></span>

<span data-ttu-id="e1120-134">若要请求枚举在驱动器中定义的所有捆绑包，你可以向不带任何参数的 **捆绑** 包集合提出请求。</span><span class="sxs-lookup"><span data-stu-id="e1120-134">To request an enumeration of all bundles defined in the drive, you can make a request to the **bundles** collection without any parameters.</span></span>

#### <a name="request"></a><span data-ttu-id="e1120-135">请求</span><span class="sxs-lookup"><span data-stu-id="e1120-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e1120-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1120-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-all-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles
```
# <a name="c"></a>[<span data-ttu-id="e1120-137">C#</span><span class="sxs-lookup"><span data-stu-id="e1120-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-all-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1120-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1120-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-all-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1120-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1120-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-all-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1120-140">Java</span><span class="sxs-lookup"><span data-stu-id="e1120-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-all-bundles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e1120-141">响应</span><span class="sxs-lookup"><span data-stu-id="e1120-141">Response</span></span>

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

<span data-ttu-id="e1120-142">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e1120-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e1120-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e1120-143">All the properties will be returned from an actual call.</span></span>


### <a name="example-2-list-all-photo-albums-in-a-drive"></a><span data-ttu-id="e1120-144">示例 2：列出驱动器中所有相册</span><span class="sxs-lookup"><span data-stu-id="e1120-144">Example 2: List all photo albums in a drive</span></span>

<span data-ttu-id="e1120-145">若要筛选从对捆绑包集合的请求返回的捆绑包列表，可以使用查询字符串参数通过检查捆绑包上是否存在 Facet 来指定要返回的捆绑 `filter` 包的类型：</span><span class="sxs-lookup"><span data-stu-id="e1120-145">To filter the list of bundles returned from a request to the bundles collection, you can use the `filter` query string parameter to specify the type of bundle to return by checking for the existence of a facet on the bundle:</span></span>

#### <a name="request"></a><span data-ttu-id="e1120-146">请求</span><span class="sxs-lookup"><span data-stu-id="e1120-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e1120-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1120-147">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "list-album-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles?filter=bundle/album%20ne%20null
```
# <a name="c"></a>[<span data-ttu-id="e1120-148">C#</span><span class="sxs-lookup"><span data-stu-id="e1120-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-album-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1120-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1120-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-album-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1120-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1120-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-album-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1120-151">Java</span><span class="sxs-lookup"><span data-stu-id="e1120-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-album-bundles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e1120-152">响应</span><span class="sxs-lookup"><span data-stu-id="e1120-152">Response</span></span>

<span data-ttu-id="e1120-153">对捆绑包终结点的 GET 响应是包含捆绑包的 [driveItem][] 资源的 [数组][]。</span><span class="sxs-lookup"><span data-stu-id="e1120-153">The response to a GET to the bundles endpoint is an array of [driveItem][] resources with the [bundle][].</span></span>
<span data-ttu-id="e1120-154">由于所有捆绑包都是项目，因此可以使用所有标准项操作。</span><span class="sxs-lookup"><span data-stu-id="e1120-154">Because all bundles are items, you can use use all the standard item operations on them.</span></span>

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

<span data-ttu-id="e1120-155">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e1120-155">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e1120-156">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e1120-156">All the properties will be returned from an actual call.</span></span>


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


