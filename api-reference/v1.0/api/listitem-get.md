---
author: JeremyKelley
ms.author: JeremyKelley
title: 获取 listItem
description: 返回 SharePoint 列表中某个项的元数据。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 5046cbc44b80f6306c9e948bfbb8fce8427da117
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880698"
---
# <a name="get-listitem"></a><span data-ttu-id="01872-103">获取 listItem</span><span class="sxs-lookup"><span data-stu-id="01872-103">Get listItem</span></span>

<span data-ttu-id="01872-104">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="01872-104">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="01872-107">权限</span><span class="sxs-lookup"><span data-stu-id="01872-107">Permissions</span></span>

<span data-ttu-id="01872-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01872-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01872-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="01872-110">Permission type</span></span>      | <span data-ttu-id="01872-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01872-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01872-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01872-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01872-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01872-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="01872-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01872-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01872-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01872-115">Not supported.</span></span>    |
|<span data-ttu-id="01872-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="01872-116">Application</span></span> | <span data-ttu-id="01872-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01872-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01872-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01872-118">HTTP request</span></span>

<span data-ttu-id="01872-119">获取 listItem</span><span class="sxs-lookup"><span data-stu-id="01872-119">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="01872-120">获取 listItem 上的列值</span><span class="sxs-lookup"><span data-stu-id="01872-120">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="01872-121">获取 listItem 上的特定列值</span><span class="sxs-lookup"><span data-stu-id="01872-121">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01872-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="01872-122">Optional query parameters</span></span>
<span data-ttu-id="01872-123">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="01872-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01872-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="01872-124">Request headers</span></span>

| <span data-ttu-id="01872-125">名称</span><span class="sxs-lookup"><span data-stu-id="01872-125">Name</span></span>      |<span data-ttu-id="01872-126">说明</span><span class="sxs-lookup"><span data-stu-id="01872-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="01872-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="01872-127">Authorization</span></span>  | <span data-ttu-id="01872-128">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="01872-128">Bearer {code}.</span></span> <span data-ttu-id="01872-129">必需。</span><span class="sxs-lookup"><span data-stu-id="01872-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01872-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="01872-130">Request body</span></span>

<span data-ttu-id="01872-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01872-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01872-132">响应</span><span class="sxs-lookup"><span data-stu-id="01872-132">Response</span></span> 

<span data-ttu-id="01872-133">如果成功，此方法在响应正文中返回`200 OK`响应代码和[项目][]。</span><span class="sxs-lookup"><span data-stu-id="01872-133">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01872-134">示例</span><span class="sxs-lookup"><span data-stu-id="01872-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="01872-135">请求</span><span class="sxs-lookup"><span data-stu-id="01872-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="01872-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="01872-136">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="01872-137">C#</span><span class="sxs-lookup"><span data-stu-id="01872-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01872-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="01872-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="01872-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01872-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="01872-140">Java</span><span class="sxs-lookup"><span data-stu-id="01872-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="01872-141">响应</span><span class="sxs-lookup"><span data-stu-id="01872-141">Response</span></span>

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


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
} -->
