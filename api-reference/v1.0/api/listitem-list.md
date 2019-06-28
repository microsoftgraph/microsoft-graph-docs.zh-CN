---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 检索 SharePoint 列表中的项
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: b3b41aceaad0251eeaf8c6339ef7f691abe1261c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271965"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="d0ebc-102">枚举列表中的项</span><span class="sxs-lookup"><span data-stu-id="d0ebc-102">Enumerate items in a list</span></span>

<span data-ttu-id="d0ebc-103">获取[列表][]中[项][item]的集合。</span><span class="sxs-lookup"><span data-stu-id="d0ebc-103">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="d0ebc-105">权限</span><span class="sxs-lookup"><span data-stu-id="d0ebc-105">Permissions</span></span>

<span data-ttu-id="d0ebc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0ebc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0ebc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0ebc-108">Permission type</span></span>      | <span data-ttu-id="d0ebc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0ebc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0ebc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0ebc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d0ebc-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ebc-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0ebc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0ebc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0ebc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0ebc-113">Not supported.</span></span>    |
|<span data-ttu-id="d0ebc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0ebc-114">Application</span></span> | <span data-ttu-id="d0ebc-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ebc-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0ebc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0ebc-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="d0ebc-117">示例</span><span class="sxs-lookup"><span data-stu-id="d0ebc-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d0ebc-118">请求</span><span class="sxs-lookup"><span data-stu-id="d0ebc-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="d0ebc-119">响应</span><span class="sxs-lookup"><span data-stu-id="d0ebc-119">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Color": "Red",
        "Quantity": 503
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Color": "Blue",
        "Quantity": 2357
       }
    },
    {
      "id": "7",
      "fields": {
        "Name": "Gizmo",
        "Color": "Green",
        "Quantity": 92
       }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d0ebc-120">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d0ebc-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d0ebc-121">C#</span><span class="sxs-lookup"><span data-stu-id="d0ebc-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-items-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0ebc-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="d0ebc-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-items-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d0ebc-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0ebc-123">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-items-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitem-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
