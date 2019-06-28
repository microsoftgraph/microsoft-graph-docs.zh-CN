---
author: JeremyKelley
ms.author: JeremyKelley
title: 获取 listItem
description: 返回 SharePoint 列表中某个项的元数据。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 57d95b67ff27ff58e26310db69f97c027d5e3639
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271993"
---
# <a name="get-listitem"></a><span data-ttu-id="4a662-103">获取 listItem</span><span class="sxs-lookup"><span data-stu-id="4a662-103">Get listItem</span></span>

<span data-ttu-id="4a662-104">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="4a662-104">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="4a662-107">权限</span><span class="sxs-lookup"><span data-stu-id="4a662-107">Permissions</span></span>

<span data-ttu-id="4a662-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a662-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a662-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a662-110">Permission type</span></span>      | <span data-ttu-id="4a662-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a662-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a662-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a662-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4a662-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a662-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a662-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a662-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a662-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a662-115">Not supported.</span></span>    |
|<span data-ttu-id="4a662-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a662-116">Application</span></span> | <span data-ttu-id="4a662-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a662-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a662-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a662-118">HTTP request</span></span>

<span data-ttu-id="4a662-119">获取 listItem</span><span class="sxs-lookup"><span data-stu-id="4a662-119">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="4a662-120">获取 listItem 上的列值</span><span class="sxs-lookup"><span data-stu-id="4a662-120">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="4a662-121">获取 listItem 上的特定列值</span><span class="sxs-lookup"><span data-stu-id="4a662-121">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4a662-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4a662-122">Optional query parameters</span></span>
<span data-ttu-id="4a662-123">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4a662-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a662-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a662-124">Request headers</span></span>

| <span data-ttu-id="4a662-125">名称</span><span class="sxs-lookup"><span data-stu-id="4a662-125">Name</span></span>      |<span data-ttu-id="4a662-126">说明</span><span class="sxs-lookup"><span data-stu-id="4a662-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a662-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a662-127">Authorization</span></span>  | <span data-ttu-id="4a662-128">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="4a662-128">Bearer {code}.</span></span> <span data-ttu-id="4a662-129">必需。</span><span class="sxs-lookup"><span data-stu-id="4a662-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a662-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a662-130">Request body</span></span>

<span data-ttu-id="4a662-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4a662-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a662-132">响应</span><span class="sxs-lookup"><span data-stu-id="4a662-132">Response</span></span> 

<span data-ttu-id="4a662-133">如果成功，此方法在响应正文中返回`200 OK`响应代码和[项目][]。</span><span class="sxs-lookup"><span data-stu-id="4a662-133">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a662-134">示例</span><span class="sxs-lookup"><span data-stu-id="4a662-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a662-135">请求</span><span class="sxs-lookup"><span data-stu-id="4a662-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="4a662-136">响应</span><span class="sxs-lookup"><span data-stu-id="4a662-136">Response</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="4a662-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4a662-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4a662-138">C#</span><span class="sxs-lookup"><span data-stu-id="4a662-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a662-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a662-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4a662-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a662-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
