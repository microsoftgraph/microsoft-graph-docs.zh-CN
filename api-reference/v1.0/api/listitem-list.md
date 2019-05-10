---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 检索 SharePoint 列表中的项
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 6038b5d82ed91b94a9388689ba39c890f1dc4f6c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613520"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="a5334-102">枚举列表中的项</span><span class="sxs-lookup"><span data-stu-id="a5334-102">Enumerate items in a list</span></span>

<span data-ttu-id="a5334-103">获取[列表][]中[项][item]的集合。</span><span class="sxs-lookup"><span data-stu-id="a5334-103">Get the collection of [items][item] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="a5334-105">权限</span><span class="sxs-lookup"><span data-stu-id="a5334-105">Permissions</span></span>

<span data-ttu-id="a5334-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5334-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5334-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5334-108">Permission type</span></span>      | <span data-ttu-id="a5334-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5334-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5334-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5334-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5334-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5334-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5334-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5334-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5334-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5334-113">Not supported.</span></span>    |
|<span data-ttu-id="a5334-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5334-114">Application</span></span> | <span data-ttu-id="a5334-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5334-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5334-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5334-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="a5334-117">示例</span><span class="sxs-lookup"><span data-stu-id="a5334-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a5334-118">请求</span><span class="sxs-lookup"><span data-stu-id="a5334-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="a5334-119">响应</span><span class="sxs-lookup"><span data-stu-id="a5334-119">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a5334-120">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a5334-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a5334-121">C#</span><span class="sxs-lookup"><span data-stu-id="a5334-121">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-items-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5334-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="a5334-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-items-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
