---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 搜索文件
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ce18912b0fd116f13e2bd32d999dd852d6cc5182
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528219"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="213f7-102">搜索驱动器内的 DriveItems</span><span class="sxs-lookup"><span data-stu-id="213f7-102">Search for a DriveItems within a drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="213f7-103">在项目层次结构中搜索与查询匹配的项目。</span><span class="sxs-lookup"><span data-stu-id="213f7-103">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="213f7-104">可以在文件夹层次结构、整个驱动器或与当前用户共享的文件内执行搜索。</span><span class="sxs-lookup"><span data-stu-id="213f7-104">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="213f7-105">权限</span><span class="sxs-lookup"><span data-stu-id="213f7-105">Permissions</span></span>

<span data-ttu-id="213f7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="213f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="213f7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="213f7-108">Permission type</span></span>      | <span data-ttu-id="213f7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="213f7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="213f7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="213f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="213f7-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="213f7-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="213f7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="213f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="213f7-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="213f7-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="213f7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="213f7-114">Application</span></span> | <span data-ttu-id="213f7-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="213f7-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="213f7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="213f7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="213f7-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="213f7-117">Optional query parameters</span></span>

<span data-ttu-id="213f7-118">此方法支持使用 `$expand`、`$select`、`$skipToken`、`$top` 和 `$orderby` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="213f7-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="213f7-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="213f7-119">Function parameters</span></span>

| <span data-ttu-id="213f7-120">参数</span><span class="sxs-lookup"><span data-stu-id="213f7-120">Parameter</span></span> | <span data-ttu-id="213f7-121">类型</span><span class="sxs-lookup"><span data-stu-id="213f7-121">Type</span></span>  | <span data-ttu-id="213f7-122">说明</span><span class="sxs-lookup"><span data-stu-id="213f7-122">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="213f7-123">q</span><span class="sxs-lookup"><span data-stu-id="213f7-123">q</span></span>  | <span data-ttu-id="213f7-124">string</span><span class="sxs-lookup"><span data-stu-id="213f7-124">string</span></span> | <span data-ttu-id="213f7-p103">用来搜索项目的查询文本。可以跨多个字段（包括文件名、元数据和文件内容）与值相匹配。</span><span class="sxs-lookup"><span data-stu-id="213f7-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="213f7-127">示例</span><span class="sxs-lookup"><span data-stu-id="213f7-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="213f7-128">请求</span><span class="sxs-lookup"><span data-stu-id="213f7-128">Request</span></span>

<span data-ttu-id="213f7-129">下面是一个请求搜索当前用户的 OneDrive 示例</span><span class="sxs-lookup"><span data-stu-id="213f7-129">Here is an example of the request searching the current user's OneDrive</span></span>

<!-- { "blockType": "request", "name": "item_search" }-->

```http
GET /me/drive/root/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="213f7-130">响应</span><span class="sxs-lookup"><span data-stu-id="213f7-130">Response</span></span>

<span data-ttu-id="213f7-p104">此方法返回一个对象，该对象包含与搜索条件相匹配的 [DriveItem](../resources/driveitem.md) 集合。如果未找到任何项目，则返回一个空集合。</span><span class="sxs-lookup"><span data-stu-id="213f7-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="213f7-p105">如果匹配项太多，将对响应分页，并且 **@odata.nextLink** 属性将包含指向下一页结果的 URL。可以使用 `$top` 查询参数来指定页中的项目数。</span><span class="sxs-lookup"><span data-stu-id="213f7-p105">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

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

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="213f7-135">搜索用户可以访问的项目</span><span class="sxs-lookup"><span data-stu-id="213f7-135">Searching for items a user can access</span></span>

<span data-ttu-id="213f7-p106">除了在驱动器中搜索项目外，你的应用程序还可以进行更广泛的搜索，以便包含与当前用户共享的项目。若要扩大搜索范围，请使用 [驱动器](../resources/drive.md) 资源中的**搜索**方法。</span><span class="sxs-lookup"><span data-stu-id="213f7-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="213f7-138">示例</span><span class="sxs-lookup"><span data-stu-id="213f7-138">Example</span></span>

<!-- { "blockType": "request", "name": "item_search_all" }-->

```http
GET /me/drive/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="213f7-139">响应</span><span class="sxs-lookup"><span data-stu-id="213f7-139">Response</span></span>

<span data-ttu-id="213f7-p107">从**驱动器**资源中搜索时的响应可能包括驱动器外部的项目（与当前用户共享的项目）。这些项目将包括 [**remoteItem**](../resources/remoteitem.md) 方面，以指示它们存储在目标驱动器外部。</span><span class="sxs-lookup"><span data-stu-id="213f7-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

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

## <a name="error-responses"></a><span data-ttu-id="213f7-142">错误响应</span><span class="sxs-lookup"><span data-stu-id="213f7-142">Error responses</span></span>

<span data-ttu-id="213f7-143">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="213f7-143">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
    "Error: /api-reference/beta/api/driveitem-search.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
