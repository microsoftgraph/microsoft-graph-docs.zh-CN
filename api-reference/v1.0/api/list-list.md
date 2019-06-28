---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 列出网站中的 SharePoint 列表
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 98d3d893c5aa02bd7df6d997244e940ce7049f08
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272042"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="452c7-102">枚举网站中的列表</span><span class="sxs-lookup"><span data-stu-id="452c7-102">Enumerate lists in a site</span></span>

<span data-ttu-id="452c7-103">获取 [site][] 的 [lists][] 的集合。</span><span class="sxs-lookup"><span data-stu-id="452c7-103">Get the collection of [lists][] for a [site][].</span></span>

[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="452c7-106">权限</span><span class="sxs-lookup"><span data-stu-id="452c7-106">Permissions</span></span>

<span data-ttu-id="452c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="452c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="452c7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="452c7-109">Permission type</span></span>      | <span data-ttu-id="452c7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="452c7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="452c7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="452c7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="452c7-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="452c7-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="452c7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="452c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="452c7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="452c7-114">Not supported.</span></span>    |
|<span data-ttu-id="452c7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="452c7-115">Application</span></span> | <span data-ttu-id="452c7-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="452c7-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="452c7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="452c7-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="452c7-118">示例</span><span class="sxs-lookup"><span data-stu-id="452c7-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="452c7-119">请求</span><span class="sxs-lookup"><span data-stu-id="452c7-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="452c7-120">响应</span><span class="sxs-lookup"><span data-stu-id="452c7-120">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="452c7-121">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="452c7-121">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="452c7-122">C#</span><span class="sxs-lookup"><span data-stu-id="452c7-122">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/enum-lists-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="452c7-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="452c7-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/enum-lists-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="452c7-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="452c7-124">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/enum-lists-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="452c7-125">说明</span><span class="sxs-lookup"><span data-stu-id="452c7-125">Remarks</span></span>

<span data-ttu-id="452c7-126">默认情况下，将隐藏包含 [system][] Facet 的列表。</span><span class="sxs-lookup"><span data-stu-id="452c7-126">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="452c7-127">若要列出它们，请在 `$select` 语句中添加 `system`。</span><span class="sxs-lookup"><span data-stu-id="452c7-127">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
    "Error: /api-reference/v1.0/api/list-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/list-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
