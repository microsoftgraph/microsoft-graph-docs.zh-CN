---
author: JeremyKelley
ms.author: JeremyKelley
title: 获取 listItem
description: 返回 SharePoint 列表中某个项的元数据。
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e2d441bb306a6614cdc27f5dff79bd55377b0459
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057283"
---
# <a name="get-listitem"></a><span data-ttu-id="ae7ad-103">获取 listItem</span><span class="sxs-lookup"><span data-stu-id="ae7ad-103">Get listItem</span></span>

<span data-ttu-id="ae7ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae7ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae7ad-105">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="ae7ad-105">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="ae7ad-108">权限</span><span class="sxs-lookup"><span data-stu-id="ae7ad-108">Permissions</span></span>

<span data-ttu-id="ae7ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae7ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae7ad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae7ad-111">Permission type</span></span>      | <span data-ttu-id="ae7ad-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae7ad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae7ad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae7ad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ae7ad-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae7ad-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ae7ad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae7ad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae7ad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae7ad-116">Not supported.</span></span>    |
|<span data-ttu-id="ae7ad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae7ad-117">Application</span></span> | <span data-ttu-id="ae7ad-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae7ad-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae7ad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae7ad-119">HTTP request</span></span>

<span data-ttu-id="ae7ad-120">获取 listItem</span><span class="sxs-lookup"><span data-stu-id="ae7ad-120">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="ae7ad-121">获取 listItem 上的列值</span><span class="sxs-lookup"><span data-stu-id="ae7ad-121">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="ae7ad-122">获取 listItem 上的特定列值</span><span class="sxs-lookup"><span data-stu-id="ae7ad-122">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae7ad-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae7ad-123">Optional query parameters</span></span>
<span data-ttu-id="ae7ad-124">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ae7ad-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae7ad-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae7ad-125">Request headers</span></span>

| <span data-ttu-id="ae7ad-126">名称</span><span class="sxs-lookup"><span data-stu-id="ae7ad-126">Name</span></span>      |<span data-ttu-id="ae7ad-127">说明</span><span class="sxs-lookup"><span data-stu-id="ae7ad-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae7ad-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae7ad-128">Authorization</span></span>  | <span data-ttu-id="ae7ad-129">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="ae7ad-129">Bearer {code}.</span></span> <span data-ttu-id="ae7ad-130">必需。</span><span class="sxs-lookup"><span data-stu-id="ae7ad-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae7ad-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae7ad-131">Request body</span></span>

<span data-ttu-id="ae7ad-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae7ad-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae7ad-133">响应</span><span class="sxs-lookup"><span data-stu-id="ae7ad-133">Response</span></span> 

<span data-ttu-id="ae7ad-134">如果成功，此方法在响应正文中返回`200 OK`响应代码和[项目][]。</span><span class="sxs-lookup"><span data-stu-id="ae7ad-134">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae7ad-135">示例</span><span class="sxs-lookup"><span data-stu-id="ae7ad-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae7ad-136">请求</span><span class="sxs-lookup"><span data-stu-id="ae7ad-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ae7ad-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae7ad-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="ae7ad-138">C#</span><span class="sxs-lookup"><span data-stu-id="ae7ad-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae7ad-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae7ad-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae7ad-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae7ad-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae7ad-141">Java</span><span class="sxs-lookup"><span data-stu-id="ae7ad-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ae7ad-142">响应</span><span class="sxs-lookup"><span data-stu-id="ae7ad-142">Response</span></span>

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

