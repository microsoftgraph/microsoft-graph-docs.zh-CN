---
author: JeremyKelley
ms.date: 09/11/2017
title: 列出网站中的 SharePoint 列表
localization_priority: Priority
ms.prod: sharepoint
description: 获取网站列表的集合。
doc_type: apiPageType
ms.openlocfilehash: ffafff7ed35f8e88d32ccd5f0e6daf3f9861e1a7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238797"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="16e43-103">枚举网站中的列表</span><span class="sxs-lookup"><span data-stu-id="16e43-103">Enumerate lists in a site</span></span>

<span data-ttu-id="16e43-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16e43-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16e43-105">获取 [site][] 的 [lists][] 的集合。</span><span class="sxs-lookup"><span data-stu-id="16e43-105">Get the collection of [lists][] for a [site][].</span></span>

[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="16e43-108">权限</span><span class="sxs-lookup"><span data-stu-id="16e43-108">Permissions</span></span>

<span data-ttu-id="16e43-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16e43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16e43-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="16e43-111">Permission type</span></span>      | <span data-ttu-id="16e43-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16e43-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16e43-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16e43-113">Delegated (work or school account)</span></span> | <span data-ttu-id="16e43-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e43-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="16e43-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16e43-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16e43-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="16e43-116">Not supported.</span></span>    |
|<span data-ttu-id="16e43-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="16e43-117">Application</span></span> | <span data-ttu-id="16e43-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e43-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16e43-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16e43-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="16e43-120">示例</span><span class="sxs-lookup"><span data-stu-id="16e43-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="16e43-121">请求</span><span class="sxs-lookup"><span data-stu-id="16e43-121">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="16e43-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="16e43-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```
# <a name="c"></a>[<span data-ttu-id="16e43-123">C#</span><span class="sxs-lookup"><span data-stu-id="16e43-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16e43-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16e43-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16e43-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16e43-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16e43-126">Java</span><span class="sxs-lookup"><span data-stu-id="16e43-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="16e43-127">响应</span><span class="sxs-lookup"><span data-stu-id="16e43-127">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="16e43-128">注解</span><span class="sxs-lookup"><span data-stu-id="16e43-128">Remarks</span></span>

<span data-ttu-id="16e43-129">默认情况下，将隐藏包含 [system][] Facet 的列表。</span><span class="sxs-lookup"><span data-stu-id="16e43-129">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="16e43-130">若要列出它们，请在 `$select` 语句中添加 `system`。</span><span class="sxs-lookup"><span data-stu-id="16e43-130">To list them, include `system` in your `$select` statement.</span></span>

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

