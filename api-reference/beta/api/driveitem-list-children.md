---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出文件夹的内容
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 83a3394c8c7f5b77dbedeece6c38045bab0fd9a6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589751"
---
# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="fc73f-102">列出 DriveItem 的子项</span><span class="sxs-lookup"><span data-stu-id="fc73f-102">List children of a driveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc73f-103">在 DriveItem 的 **children** 关系中返回 [DriveItems](../resources/driveitem.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="fc73f-103">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="fc73f-104">具有非 null **folder** 或 **package** facet 的 DriveItem 可以拥有一个或多个子 DriveItem。</span><span class="sxs-lookup"><span data-stu-id="fc73f-104">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="fc73f-105">权限</span><span class="sxs-lookup"><span data-stu-id="fc73f-105">Permissions</span></span>

<span data-ttu-id="fc73f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc73f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc73f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc73f-108">Permission type</span></span>      | <span data-ttu-id="fc73f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc73f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc73f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc73f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fc73f-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc73f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fc73f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc73f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc73f-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc73f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="fc73f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc73f-114">Application</span></span> | <span data-ttu-id="fc73f-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc73f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc73f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc73f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc73f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fc73f-117">Optional query parameters</span></span>

<span data-ttu-id="fc73f-118">此方法支持使用 `$expand`、`$select`、`$skipToken`、`$top` 和 `$orderby` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fc73f-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top` and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

### <a name="optional-request-headers"></a><span data-ttu-id="fc73f-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="fc73f-119">Optional request headers</span></span>

| <span data-ttu-id="fc73f-120">头名称</span><span class="sxs-lookup"><span data-stu-id="fc73f-120">Header name</span></span>     | <span data-ttu-id="fc73f-121">值</span><span class="sxs-lookup"><span data-stu-id="fc73f-121">Value</span></span> | <span data-ttu-id="fc73f-122">说明</span><span class="sxs-lookup"><span data-stu-id="fc73f-122">Description</span></span>                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fc73f-123">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="fc73f-123">_if-none-match_</span></span> | <span data-ttu-id="fc73f-124">etag</span><span class="sxs-lookup"><span data-stu-id="fc73f-124">etag</span></span>  | <span data-ttu-id="fc73f-125">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="fc73f-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="examples"></a><span data-ttu-id="fc73f-126">示例</span><span class="sxs-lookup"><span data-stu-id="fc73f-126">Examples</span></span>

### <a name="list-children-in-the-root-of-the-current-users-drive"></a><span data-ttu-id="fc73f-127">列出当前用户的驱动器根目录中的子项</span><span class="sxs-lookup"><span data-stu-id="fc73f-127">List children in the root of the current user's drive</span></span>

<span data-ttu-id="fc73f-128">若要检索驱动器根目录中的文件，请使用驱动器上的 `root` 关系，然后访问子项关系。</span><span class="sxs-lookup"><span data-stu-id="fc73f-128">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read" } -->

```http
GET /me/drive/root/children
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fc73f-129">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="fc73f-129">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fc73f-130">语言</span><span class="sxs-lookup"><span data-stu-id="fc73f-130">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-children-root-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc73f-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc73f-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-children-root-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


### <a name="list-children-of-a-driveitem-with-a-known-id"></a><span data-ttu-id="fc73f-132">列出带已知 ID 的 DriveItem 子项</span><span class="sxs-lookup"><span data-stu-id="fc73f-132">List children of a DriveItem with a known ID</span></span>

<span data-ttu-id="fc73f-133">若要检索驱动器根目录中的文件，请使用驱动器上的 `root` 关系，然后访问子项关系。</span><span class="sxs-lookup"><span data-stu-id="fc73f-133">To retrieve files in the root of the drive, use the `root` relationship on the drive, then access the children relationship.</span></span>

<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fc73f-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="fc73f-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fc73f-135">语言</span><span class="sxs-lookup"><span data-stu-id="fc73f-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-children-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc73f-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc73f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-children-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="list-children-of-a-driveitem-with-a-known-path"></a><span data-ttu-id="fc73f-137">列出带已知路径的 DriveItem 子项</span><span class="sxs-lookup"><span data-stu-id="fc73f-137">List children of a DriveItem with a known path</span></span>

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a><span data-ttu-id="fc73f-138">响应</span><span class="sxs-lookup"><span data-stu-id="fc73f-138">Response</span></span>

<span data-ttu-id="fc73f-p102">如果成功，此方法将返回目标项的子项集合列表。 子项集合由 [driveItem][item-resource] 资源组成。</span><span class="sxs-lookup"><span data-stu-id="fc73f-p102">If successful, this method returns the list of items in the children collection of the target item. The children collection will be composed of [driveItem][item-resource] resources.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.driveItem)", 
       "truncated": true,
       "name": [ "list-children-root", "list-children", "list-children-from-path" ] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="fc73f-141">**注意：** 如果集合超出默认页面大小（200 项），则在响应中返回 **@odata.nextLink** 属性以指示有更多项可用，并提供下一页项目的请求 URL。</span><span class="sxs-lookup"><span data-stu-id="fc73f-141">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="fc73f-142">可以通过[可选的查询字符串参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)控制页面大小</span><span class="sxs-lookup"><span data-stu-id="fc73f-142">You can control the page size through [optional query string parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters)</span></span>

### <a name="error-responses"></a><span data-ttu-id="fc73f-143">错误响应</span><span class="sxs-lookup"><span data-stu-id="fc73f-143">Error responses</span></span>

<span data-ttu-id="fc73f-144">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="fc73f-144">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-list-children.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-children.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-children.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-children.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
