---
author: JeremyKelley
description: 获取列表中项的集合。
ms.date: 09/11/2017
title: 检索 SharePoint 列表中的项
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: dd188f69ea39acf98117231ad6c153852cb4f5b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993051"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="4a08c-103">枚举列表中的项</span><span class="sxs-lookup"><span data-stu-id="4a08c-103">Enumerate items in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a08c-104">获取[列表][]中[项][item]的集合。</span><span class="sxs-lookup"><span data-stu-id="4a08c-104">Get the collection of [items][item] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="4a08c-106">权限</span><span class="sxs-lookup"><span data-stu-id="4a08c-106">Permissions</span></span>

<span data-ttu-id="4a08c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a08c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a08c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a08c-109">Permission type</span></span>      | <span data-ttu-id="4a08c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a08c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a08c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a08c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4a08c-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a08c-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a08c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a08c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a08c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a08c-114">Not supported.</span></span>    |
|<span data-ttu-id="4a08c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a08c-115">Application</span></span> | <span data-ttu-id="4a08c-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a08c-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a08c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a08c-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="4a08c-118">示例</span><span class="sxs-lookup"><span data-stu-id="4a08c-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4a08c-119">请求</span><span class="sxs-lookup"><span data-stu-id="4a08c-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4a08c-120">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4a08c-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a08c-121">C#</span><span class="sxs-lookup"><span data-stu-id="4a08c-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a08c-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a08c-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a08c-123">目标-C</span><span class="sxs-lookup"><span data-stu-id="4a08c-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4a08c-124">Java</span><span class="sxs-lookup"><span data-stu-id="4a08c-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4a08c-125">响应</span><span class="sxs-lookup"><span data-stu-id="4a08c-125">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
  ]
}
-->
