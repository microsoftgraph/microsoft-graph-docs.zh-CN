---
title: 列出列表的版本
description: SharePoint 可以配置为保留列表项的历史记录。
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 55c0ebce4055ea481e0bfeed63cb0b850b4ebad2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023142"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="b530e-103">列出列表的版本</span><span class="sxs-lookup"><span data-stu-id="b530e-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="b530e-104">SharePoint 可以配置为保留列表项的历史记录。</span><span class="sxs-lookup"><span data-stu-id="b530e-104">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="b530e-105">以前版本可能会保留有限的一段时间，具体取决于管理员设置，这对于每个用户或位置可能是唯一的。</span><span class="sxs-lookup"><span data-stu-id="b530e-105">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="b530e-106">权限</span><span class="sxs-lookup"><span data-stu-id="b530e-106">Permissions</span></span>

<span data-ttu-id="b530e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b530e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="b530e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b530e-109">Permission type</span></span>             | <span data-ttu-id="b530e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b530e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="b530e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b530e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b530e-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b530e-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="b530e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b530e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b530e-114">无</span><span class="sxs-lookup"><span data-stu-id="b530e-114">n/a</span></span>                                         |
| <span data-ttu-id="b530e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b530e-115">Application</span></span>                            | <span data-ttu-id="b530e-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b530e-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="b530e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b530e-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="b530e-118">响应</span><span class="sxs-lookup"><span data-stu-id="b530e-118">Response</span></span>

<span data-ttu-id="b530e-119">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ListItemVersion](../resources/listitemversion.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="b530e-119">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="b530e-120">示例</span><span class="sxs-lookup"><span data-stu-id="b530e-120">Example</span></span>

<span data-ttu-id="b530e-121">本示例检索 SharePoint 列表中的 listItem 的版本：</span><span class="sxs-lookup"><span data-stu-id="b530e-121">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="b530e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b530e-122">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b530e-123">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b530e-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b530e-124">C#</span><span class="sxs-lookup"><span data-stu-id="b530e-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-previous-versions-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b530e-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="b530e-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-previous-versions-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b530e-126">目标-C</span><span class="sxs-lookup"><span data-stu-id="b530e-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-previous-versions-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b530e-127">Java</span><span class="sxs-lookup"><span data-stu-id="b530e-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-previous-versions-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b530e-128">响应</span><span class="sxs-lookup"><span data-stu-id="b530e-128">Response</span></span>

<span data-ttu-id="b530e-129">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="b530e-129">This returns a collection of versions:</span></span>

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


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
