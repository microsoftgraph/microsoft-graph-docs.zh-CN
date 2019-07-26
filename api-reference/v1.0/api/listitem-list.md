---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 检索 SharePoint 列表中的项
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 0eda28675e4b785b6745ea15f167a9236ac8f8c0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884541"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="89047-102">枚举列表中的项</span><span class="sxs-lookup"><span data-stu-id="89047-102">Enumerate items in a list</span></span>

<span data-ttu-id="89047-103">获取[列表][]中[项][item]的集合。</span><span class="sxs-lookup"><span data-stu-id="89047-103">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="89047-105">权限</span><span class="sxs-lookup"><span data-stu-id="89047-105">Permissions</span></span>

<span data-ttu-id="89047-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89047-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89047-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="89047-108">Permission type</span></span>      | <span data-ttu-id="89047-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89047-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89047-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89047-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89047-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89047-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="89047-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89047-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89047-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="89047-113">Not supported.</span></span>    |
|<span data-ttu-id="89047-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="89047-114">Application</span></span> | <span data-ttu-id="89047-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89047-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89047-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89047-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="89047-117">示例</span><span class="sxs-lookup"><span data-stu-id="89047-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="89047-118">请求</span><span class="sxs-lookup"><span data-stu-id="89047-118">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="89047-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="89047-119">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="89047-120">C#</span><span class="sxs-lookup"><span data-stu-id="89047-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89047-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="89047-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89047-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89047-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="89047-123">Java</span><span class="sxs-lookup"><span data-stu-id="89047-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89047-124">响应</span><span class="sxs-lookup"><span data-stu-id="89047-124">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
  ]
} -->
