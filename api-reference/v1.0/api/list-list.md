---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 列出网站中的 SharePoint 列表
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: d5ead524312fe1beffc561d8e936c8742c0e723a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888321"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="97976-102">枚举网站中的列表</span><span class="sxs-lookup"><span data-stu-id="97976-102">Enumerate lists in a site</span></span>

<span data-ttu-id="97976-103">获取 [site][] 的 [lists][] 的集合。</span><span class="sxs-lookup"><span data-stu-id="97976-103">Get the collection of [lists][] for a [site][].</span></span>

[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="97976-106">权限</span><span class="sxs-lookup"><span data-stu-id="97976-106">Permissions</span></span>

<span data-ttu-id="97976-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97976-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97976-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="97976-109">Permission type</span></span>      | <span data-ttu-id="97976-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97976-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97976-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97976-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97976-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97976-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="97976-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97976-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97976-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="97976-114">Not supported.</span></span>    |
|<span data-ttu-id="97976-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="97976-115">Application</span></span> | <span data-ttu-id="97976-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97976-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97976-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97976-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="97976-118">示例</span><span class="sxs-lookup"><span data-stu-id="97976-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="97976-119">请求</span><span class="sxs-lookup"><span data-stu-id="97976-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="97976-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="97976-120">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97976-121">C#</span><span class="sxs-lookup"><span data-stu-id="97976-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97976-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="97976-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97976-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97976-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="97976-124">Java</span><span class="sxs-lookup"><span data-stu-id="97976-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="97976-125">响应</span><span class="sxs-lookup"><span data-stu-id="97976-125">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="97976-126">注解</span><span class="sxs-lookup"><span data-stu-id="97976-126">Remarks</span></span>

<span data-ttu-id="97976-127">默认情况下，将隐藏包含 [system][] Facet 的列表。</span><span class="sxs-lookup"><span data-stu-id="97976-127">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="97976-128">若要列出它们，请在 `$select` 语句中添加 `system`。</span><span class="sxs-lookup"><span data-stu-id="97976-128">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
  ]
} -->
