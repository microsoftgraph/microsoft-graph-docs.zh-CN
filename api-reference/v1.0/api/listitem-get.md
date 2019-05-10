---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: c46fed1c2da3ac246212dbbcdfeb35479699efe6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613063"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="35895-102">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="35895-102">Get an item in a list</span></span>

<span data-ttu-id="35895-103">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="35895-103">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="35895-106">权限</span><span class="sxs-lookup"><span data-stu-id="35895-106">Permissions</span></span>

<span data-ttu-id="35895-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35895-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="35895-109">Permission type</span></span>      | <span data-ttu-id="35895-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="35895-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35895-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35895-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35895-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35895-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="35895-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35895-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35895-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="35895-114">Not supported.</span></span>    |
|<span data-ttu-id="35895-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="35895-115">Application</span></span> | <span data-ttu-id="35895-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35895-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35895-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35895-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="35895-118">示例</span><span class="sxs-lookup"><span data-stu-id="35895-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="35895-119">请求</span><span class="sxs-lookup"><span data-stu-id="35895-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="35895-120">响应</span><span class="sxs-lookup"><span data-stu-id="35895-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="35895-121">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="35895-121">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="35895-122">C#</span><span class="sxs-lookup"><span data-stu-id="35895-122">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35895-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="35895-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
