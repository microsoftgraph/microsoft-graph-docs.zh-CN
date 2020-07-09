---
author: JeremyKelley
description: 在项目层次结构中搜索与查询匹配的项目。
ms.date: 09/10/2017
title: 搜索文件
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 08774f68c9b5ec17ff3e0c5f4f6ba42e058245e1
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091401"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="368fc-103">搜索驱动器内的 DriveItems</span><span class="sxs-lookup"><span data-stu-id="368fc-103">Search for a DriveItems within a drive</span></span>

<span data-ttu-id="368fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="368fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="368fc-105">在项目层次结构中搜索与查询匹配的项目。</span><span class="sxs-lookup"><span data-stu-id="368fc-105">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="368fc-106">可以在文件夹层次结构、整个驱动器或与当前用户共享的文件内执行搜索。</span><span class="sxs-lookup"><span data-stu-id="368fc-106">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="368fc-107">权限</span><span class="sxs-lookup"><span data-stu-id="368fc-107">Permissions</span></span>

<span data-ttu-id="368fc-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="368fc-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="368fc-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="368fc-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="368fc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="368fc-110">Permission type</span></span>      | <span data-ttu-id="368fc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="368fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="368fc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="368fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="368fc-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="368fc-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="368fc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="368fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="368fc-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="368fc-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="368fc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="368fc-116">Application</span></span> | <span data-ttu-id="368fc-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="368fc-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="368fc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="368fc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="368fc-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="368fc-119">Optional query parameters</span></span>

<span data-ttu-id="368fc-120">此方法支持使用 `$expand`、`$select`、`$skipToken`、`$top` 和 `$orderby` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="368fc-120">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="368fc-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="368fc-121">Function parameters</span></span>

| <span data-ttu-id="368fc-122">参数</span><span class="sxs-lookup"><span data-stu-id="368fc-122">Parameter</span></span> | <span data-ttu-id="368fc-123">类型</span><span class="sxs-lookup"><span data-stu-id="368fc-123">Type</span></span>  | <span data-ttu-id="368fc-124">说明</span><span class="sxs-lookup"><span data-stu-id="368fc-124">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="368fc-125">q</span><span class="sxs-lookup"><span data-stu-id="368fc-125">q</span></span>  | <span data-ttu-id="368fc-126">字符串</span><span class="sxs-lookup"><span data-stu-id="368fc-126">string</span></span> | <span data-ttu-id="368fc-127">The query text used to search for items.</span><span class="sxs-lookup"><span data-stu-id="368fc-127">The query text used to search for items.</span></span> <span data-ttu-id="368fc-128">Values may be matched across several fields including filename, metadata, and file content.</span><span class="sxs-lookup"><span data-stu-id="368fc-128">Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="368fc-129">示例</span><span class="sxs-lookup"><span data-stu-id="368fc-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="368fc-130">请求</span><span class="sxs-lookup"><span data-stu-id="368fc-130">Request</span></span>

<span data-ttu-id="368fc-131">下面的示例在登录用户的驱动器项的多个字段中搜索 "Contoso Project" 的匹配项。</span><span class="sxs-lookup"><span data-stu-id="368fc-131">The following example searches for a match for "Contoso Project" across several fields in the signed-in user's drive items.</span></span>

# <a name="http"></a>[<span data-ttu-id="368fc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="368fc-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search" }-->

```msgraph-interactive
GET /me/drive/root/search(q='Contoso Projec}')
```
# <a name="c"></a>[<span data-ttu-id="368fc-133">C#</span><span class="sxs-lookup"><span data-stu-id="368fc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="368fc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="368fc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="368fc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="368fc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="368fc-136">响应</span><span class="sxs-lookup"><span data-stu-id="368fc-136">Response</span></span>

<span data-ttu-id="368fc-137">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria.</span><span class="sxs-lookup"><span data-stu-id="368fc-137">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria.</span></span>
<span data-ttu-id="368fc-138">If no items were found, an empty collection is returned.</span><span class="sxs-lookup"><span data-stu-id="368fc-138">If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="368fc-139">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results.</span><span class="sxs-lookup"><span data-stu-id="368fc-139">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results.</span></span>
<span data-ttu-id="368fc-140">You can use the `$top` query parameter to specify the number of items in the page.</span><span class="sxs-lookup"><span data-stu-id="368fc-140">You can use the `$top` query parameter to specify the number of items in the page.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="368fc-141">搜索用户可以访问的项目</span><span class="sxs-lookup"><span data-stu-id="368fc-141">Searching for items a user can access</span></span>

<span data-ttu-id="368fc-142">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user.</span><span class="sxs-lookup"><span data-stu-id="368fc-142">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user.</span></span>
<span data-ttu-id="368fc-143">To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span><span class="sxs-lookup"><span data-stu-id="368fc-143">To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="368fc-144">示例</span><span class="sxs-lookup"><span data-stu-id="368fc-144">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="368fc-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="368fc-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search_all" }-->

```msgraph-interactive
GET /me/drive/search(q='Contoso Project')
```
# <a name="c"></a>[<span data-ttu-id="368fc-146">C#</span><span class="sxs-lookup"><span data-stu-id="368fc-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-all-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="368fc-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="368fc-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-all-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="368fc-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="368fc-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-all-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="368fc-149">响应</span><span class="sxs-lookup"><span data-stu-id="368fc-149">Response</span></span>

<span data-ttu-id="368fc-150">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user).</span><span class="sxs-lookup"><span data-stu-id="368fc-150">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user).</span></span>
<span data-ttu-id="368fc-151">These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span><span class="sxs-lookup"><span data-stu-id="368fc-151">These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "driveId": "s!1020101jlkjl12lx" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="error-responses"></a><span data-ttu-id="368fc-152">错误响应</span><span class="sxs-lookup"><span data-stu-id="368fc-152">Error responses</span></span>

<span data-ttu-id="368fc-153">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="368fc-153">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search",
  "suppressions": [
  ]
}
-->
