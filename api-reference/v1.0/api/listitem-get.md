---
author: JeremyKelley
ms.author: JeremyKelley
title: 获取 listItem
description: 返回 SharePoint 列表中某个项的元数据。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a498947002247541bebf4fc7cd24147a0ca0df7a
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968784"
---
# <a name="get-listitem"></a><span data-ttu-id="77dd7-103">获取 listItem</span><span class="sxs-lookup"><span data-stu-id="77dd7-103">Get listItem</span></span>

<span data-ttu-id="77dd7-104">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="77dd7-104">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="77dd7-107">权限</span><span class="sxs-lookup"><span data-stu-id="77dd7-107">Permissions</span></span>

<span data-ttu-id="77dd7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77dd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77dd7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="77dd7-110">Permission type</span></span>      | <span data-ttu-id="77dd7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77dd7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77dd7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77dd7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="77dd7-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77dd7-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="77dd7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77dd7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77dd7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="77dd7-115">Not supported.</span></span>    |
|<span data-ttu-id="77dd7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="77dd7-116">Application</span></span> | <span data-ttu-id="77dd7-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77dd7-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77dd7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77dd7-118">HTTP request</span></span>

<span data-ttu-id="77dd7-119">获取 listItem</span><span class="sxs-lookup"><span data-stu-id="77dd7-119">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="77dd7-120">获取 listItem 上的列值</span><span class="sxs-lookup"><span data-stu-id="77dd7-120">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="77dd7-121">获取 listItem 上的特定列值</span><span class="sxs-lookup"><span data-stu-id="77dd7-121">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="77dd7-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="77dd7-122">Optional query parameters</span></span>
<span data-ttu-id="77dd7-123">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="77dd7-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77dd7-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="77dd7-124">Request headers</span></span>

| <span data-ttu-id="77dd7-125">名称</span><span class="sxs-lookup"><span data-stu-id="77dd7-125">Name</span></span>      |<span data-ttu-id="77dd7-126">说明</span><span class="sxs-lookup"><span data-stu-id="77dd7-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77dd7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="77dd7-127">Authorization</span></span>  | <span data-ttu-id="77dd7-128">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="77dd7-128">Bearer {code}.</span></span> <span data-ttu-id="77dd7-129">必需。</span><span class="sxs-lookup"><span data-stu-id="77dd7-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77dd7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="77dd7-130">Request body</span></span>

<span data-ttu-id="77dd7-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77dd7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77dd7-132">响应</span><span class="sxs-lookup"><span data-stu-id="77dd7-132">Response</span></span> 

<span data-ttu-id="77dd7-133">如果成功，此方法在响应正文中返回`200 OK`响应代码和[项目][]。</span><span class="sxs-lookup"><span data-stu-id="77dd7-133">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77dd7-134">示例</span><span class="sxs-lookup"><span data-stu-id="77dd7-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="77dd7-135">请求</span><span class="sxs-lookup"><span data-stu-id="77dd7-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="77dd7-136">响应</span><span class="sxs-lookup"><span data-stu-id="77dd7-136">Response</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="77dd7-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="77dd7-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="77dd7-138">C#</span><span class="sxs-lookup"><span data-stu-id="77dd7-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77dd7-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="77dd7-139">Javascript</span></span>](#tab/javascript)
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
