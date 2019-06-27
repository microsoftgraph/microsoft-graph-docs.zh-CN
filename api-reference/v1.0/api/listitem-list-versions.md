---
title: 列出列表的版本
description: SharePoint 可以配置为保留列表项的历史记录。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5d242fa9d152b62f4dfbc617277623ee0b6d542d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271972"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="a16d8-103">列出列表的版本</span><span class="sxs-lookup"><span data-stu-id="a16d8-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="a16d8-104">SharePoint 可以配置为保留列表项的历史记录。</span><span class="sxs-lookup"><span data-stu-id="a16d8-104">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="a16d8-105">以前版本可能会保留有限的一段时间，具体取决于管理员设置，这对于每个用户或位置可能是唯一的。</span><span class="sxs-lookup"><span data-stu-id="a16d8-105">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="a16d8-106">权限</span><span class="sxs-lookup"><span data-stu-id="a16d8-106">Permissions</span></span>

<span data-ttu-id="a16d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a16d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="a16d8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a16d8-109">Permission type</span></span>             | <span data-ttu-id="a16d8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a16d8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a16d8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a16d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a16d8-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a16d8-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="a16d8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a16d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a16d8-114">无</span><span class="sxs-lookup"><span data-stu-id="a16d8-114">n/a</span></span>                                         |
| <span data-ttu-id="a16d8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a16d8-115">Application</span></span>                            | <span data-ttu-id="a16d8-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a16d8-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="a16d8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a16d8-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="a16d8-118">响应</span><span class="sxs-lookup"><span data-stu-id="a16d8-118">Response</span></span>

<span data-ttu-id="a16d8-119">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ListItemVersion](../resources/listitemversion.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a16d8-119">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="a16d8-120">示例</span><span class="sxs-lookup"><span data-stu-id="a16d8-120">Example</span></span>

<span data-ttu-id="a16d8-121">本示例检索 SharePoint 列表中的 listItem 的版本：</span><span class="sxs-lookup"><span data-stu-id="a16d8-121">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="a16d8-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a16d8-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="a16d8-123">响应</span><span class="sxs-lookup"><span data-stu-id="a16d8-123">Response</span></span>

<span data-ttu-id="a16d8-124">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="a16d8-124">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a16d8-125">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a16d8-125">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a16d8-126">C#</span><span class="sxs-lookup"><span data-stu-id="a16d8-126">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-previous-versions-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a16d8-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="a16d8-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-previous-versions-listitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a16d8-128">目标-C</span><span class="sxs-lookup"><span data-stu-id="a16d8-128">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-previous-versions-listitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-list-versions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
