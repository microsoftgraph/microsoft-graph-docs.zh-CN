---
title: 获取 ListItemVersion 资源
description: 检索 ListItem 的某个特定版本的元数据。
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: 474ce406f39eb1b43324677d9e48ed844e2d78df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057249"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="82bf8-103">获取 ListItemVersion 资源</span><span class="sxs-lookup"><span data-stu-id="82bf8-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="82bf8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82bf8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82bf8-105">检索 [ListItem](../resources/listitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="82bf8-105">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="82bf8-106">权限</span><span class="sxs-lookup"><span data-stu-id="82bf8-106">Permissions</span></span>

<span data-ttu-id="82bf8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82bf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="82bf8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="82bf8-109">Permission type</span></span>             | <span data-ttu-id="82bf8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82bf8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="82bf8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82bf8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="82bf8-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82bf8-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="82bf8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82bf8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82bf8-114">无</span><span class="sxs-lookup"><span data-stu-id="82bf8-114">n/a</span></span>                                         |
| <span data-ttu-id="82bf8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="82bf8-115">Application</span></span>                            | <span data-ttu-id="82bf8-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82bf8-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="82bf8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82bf8-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="82bf8-118">响应</span><span class="sxs-lookup"><span data-stu-id="82bf8-118">Response</span></span>

<span data-ttu-id="82bf8-119">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ListItemVersion](../resources/listitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="82bf8-119">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="82bf8-120">示例</span><span class="sxs-lookup"><span data-stu-id="82bf8-120">Example</span></span>

<span data-ttu-id="82bf8-121">本示例检索 listItem 的版本，并扩展字段集合以请求 listItem 中的字段值。</span><span class="sxs-lookup"><span data-stu-id="82bf8-121">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="82bf8-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82bf8-122">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="82bf8-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="82bf8-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="82bf8-124">C#</span><span class="sxs-lookup"><span data-stu-id="82bf8-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82bf8-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82bf8-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82bf8-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82bf8-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82bf8-127">Java</span><span class="sxs-lookup"><span data-stu-id="82bf8-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-single-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="82bf8-128">响应</span><span class="sxs-lookup"><span data-stu-id="82bf8-128">Response</span></span>

<span data-ttu-id="82bf8-129">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="82bf8-129">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->

