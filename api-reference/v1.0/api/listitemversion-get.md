---
title: 获取 ListItemVersion 资源
description: 检索 ListItem 的某个特定版本的元数据。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d36c09c62cd802c8514781df26f5cac076f107df
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613463"
---
# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="79d8c-103">获取 ListItemVersion 资源</span><span class="sxs-lookup"><span data-stu-id="79d8c-103">Get a ListItemVersion resource</span></span>

<span data-ttu-id="79d8c-104">检索 [ListItem](../resources/listitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="79d8c-104">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79d8c-105">权限</span><span class="sxs-lookup"><span data-stu-id="79d8c-105">Permissions</span></span>

<span data-ttu-id="79d8c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79d8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="79d8c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="79d8c-108">Permission type</span></span>             | <span data-ttu-id="79d8c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79d8c-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="79d8c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79d8c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="79d8c-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79d8c-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="79d8c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79d8c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79d8c-113">无</span><span class="sxs-lookup"><span data-stu-id="79d8c-113">n/a</span></span>                                         |
| <span data-ttu-id="79d8c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="79d8c-114">Application</span></span>                            | <span data-ttu-id="79d8c-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79d8c-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="79d8c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79d8c-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="79d8c-117">响应</span><span class="sxs-lookup"><span data-stu-id="79d8c-117">Response</span></span>

<span data-ttu-id="79d8c-118">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ListItemVersion](../resources/listitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79d8c-118">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="79d8c-119">示例</span><span class="sxs-lookup"><span data-stu-id="79d8c-119">Example</span></span>

<span data-ttu-id="79d8c-120">本示例检索 listItem 的版本，并扩展字段集合以请求 listItem 中的字段值。</span><span class="sxs-lookup"><span data-stu-id="79d8c-120">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="79d8c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79d8c-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="79d8c-122">响应</span><span class="sxs-lookup"><span data-stu-id="79d8c-122">Response</span></span>

<span data-ttu-id="79d8c-123">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="79d8c-123">This returns a collection of versions:</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="79d8c-124">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="79d8c-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="79d8c-125">语言</span><span class="sxs-lookup"><span data-stu-id="79d8c-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-single-version-listItem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79d8c-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="79d8c-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-single-version-listItem-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitemversion-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitemversion-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
