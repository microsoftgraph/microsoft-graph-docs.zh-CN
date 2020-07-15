---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 07/07/2020
title: 搜索文件
localization_priority: Priority
ms.prod: sharepoint
description: 在项目层次结构中搜索与查询匹配的项目。
doc_type: apiPageType
ms.openlocfilehash: 0abdd3f1f509a7c1692356888fddf805ff9833c5
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091380"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="61362-103">搜索驱动器内的 DriveItems</span><span class="sxs-lookup"><span data-stu-id="61362-103">Search for a DriveItems within a drive</span></span>

<span data-ttu-id="61362-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61362-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61362-105">在项目层次结构中搜索与查询匹配的项目。</span><span class="sxs-lookup"><span data-stu-id="61362-105">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="61362-106">可以在文件夹层次结构、整个驱动器或与当前用户共享的文件内执行搜索。</span><span class="sxs-lookup"><span data-stu-id="61362-106">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="61362-107">权限</span><span class="sxs-lookup"><span data-stu-id="61362-107">Permissions</span></span>

<span data-ttu-id="61362-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="61362-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="61362-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61362-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61362-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="61362-110">Permission type</span></span>      | <span data-ttu-id="61362-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61362-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61362-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61362-112">Delegated (work or school account)</span></span> | <span data-ttu-id="61362-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61362-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="61362-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61362-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61362-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61362-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="61362-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="61362-116">Application</span></span> | <span data-ttu-id="61362-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61362-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61362-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61362-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61362-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="61362-119">Optional query parameters</span></span>

<span data-ttu-id="61362-120">此方法支持使用 `$expand`、`$select`、`$skipToken`、`$top` 和 `$orderby` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="61362-120">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="61362-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="61362-121">Function parameters</span></span>

| <span data-ttu-id="61362-122">参数</span><span class="sxs-lookup"><span data-stu-id="61362-122">Parameter</span></span> | <span data-ttu-id="61362-123">类型</span><span class="sxs-lookup"><span data-stu-id="61362-123">Type</span></span>  | <span data-ttu-id="61362-124">说明</span><span class="sxs-lookup"><span data-stu-id="61362-124">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="61362-125">q</span><span class="sxs-lookup"><span data-stu-id="61362-125">q</span></span>  | <span data-ttu-id="61362-126">字符串</span><span class="sxs-lookup"><span data-stu-id="61362-126">string</span></span> | <span data-ttu-id="61362-127">The query text used to search for items.</span><span class="sxs-lookup"><span data-stu-id="61362-127">The query text used to search for items.</span></span> <span data-ttu-id="61362-128">Values may be matched across several fields including filename, metadata, and file content.</span><span class="sxs-lookup"><span data-stu-id="61362-128">Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="61362-129">示例</span><span class="sxs-lookup"><span data-stu-id="61362-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="61362-130">请求</span><span class="sxs-lookup"><span data-stu-id="61362-130">Request</span></span>

<span data-ttu-id="61362-131">下面的示例在登录用户的驱动器项的多个字段中搜索“Contoso Project”的匹配项。</span><span class="sxs-lookup"><span data-stu-id="61362-131">The following example searches for a match for "Contoso Project" across several fields in the signed-in user's drive items.</span></span>


# <a name="http"></a>[<span data-ttu-id="61362-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="61362-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search", "tags": "service.graph" }-->

```msgraph-interactive
GET /me/drive/root/search(q='Contoso Project')
```
# <a name="c"></a>[<span data-ttu-id="61362-133">C#</span><span class="sxs-lookup"><span data-stu-id="61362-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61362-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61362-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61362-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61362-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61362-136">Java</span><span class="sxs-lookup"><span data-stu-id="61362-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/item-search-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="61362-137">响应</span><span class="sxs-lookup"><span data-stu-id="61362-137">Response</span></span>

<span data-ttu-id="61362-138">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria.</span><span class="sxs-lookup"><span data-stu-id="61362-138">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria.</span></span>
<span data-ttu-id="61362-139">If no items were found, an empty collection is returned.</span><span class="sxs-lookup"><span data-stu-id="61362-139">If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="61362-140">If there are too many matches the response will be paged and an **\@odata.nextLink** property will contain a URL to the next page of results.</span><span class="sxs-lookup"><span data-stu-id="61362-140">If there are too many matches the response will be paged and an **\@odata.nextLink** property will contain a URL to the next page of results.</span></span>
<span data-ttu-id="61362-141">You can use the `$top` query parameter to specify the number of items in the page.</span><span class="sxs-lookup"><span data-stu-id="61362-141">You can use the `$top` query parameter to specify the number of items in the page.</span></span>

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

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="61362-142">搜索用户可以访问的项目</span><span class="sxs-lookup"><span data-stu-id="61362-142">Searching for items a user can access</span></span>

<span data-ttu-id="61362-143">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user.</span><span class="sxs-lookup"><span data-stu-id="61362-143">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user.</span></span>
<span data-ttu-id="61362-144">To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span><span class="sxs-lookup"><span data-stu-id="61362-144">To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="61362-145">示例</span><span class="sxs-lookup"><span data-stu-id="61362-145">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="61362-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="61362-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search_all", "tags": "service.graph" }-->

```msgraph-interactive
GET /me/drive/search(q='Contoso Project')
```
# <a name="c"></a>[<span data-ttu-id="61362-147">C#</span><span class="sxs-lookup"><span data-stu-id="61362-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-all-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61362-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61362-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-all-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61362-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61362-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-all-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61362-150">Java</span><span class="sxs-lookup"><span data-stu-id="61362-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/item-search-all-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="61362-151">响应</span><span class="sxs-lookup"><span data-stu-id="61362-151">Response</span></span>

<span data-ttu-id="61362-152">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user).</span><span class="sxs-lookup"><span data-stu-id="61362-152">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user).</span></span>
<span data-ttu-id="61362-153">These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span><span class="sxs-lookup"><span data-stu-id="61362-153">These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

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
        "remoteItem": { "id": "!23141901", "parentReference": { "driveId": "s!1020101jlkjl12lx" } }
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

## <a name="error-responses"></a><span data-ttu-id="61362-154">错误响应</span><span class="sxs-lookup"><span data-stu-id="61362-154">Error responses</span></span>

<span data-ttu-id="61362-155">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="61362-155">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search",
  "suppressions": [
  ]
} -->
