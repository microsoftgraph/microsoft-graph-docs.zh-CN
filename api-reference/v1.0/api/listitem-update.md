---
author: JeremyKelley
ms.author: JeremyKelley
title: 更新 listItem
description: 更新 **[listItem][]** 上的属性。
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5584ab4bde08ad0386c545f9041b2a8500c72cb1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057239"
---
# <a name="update-listitem"></a><span data-ttu-id="aaeda-103">更新 listItem</span><span class="sxs-lookup"><span data-stu-id="aaeda-103">Update listItem</span></span>

<span data-ttu-id="aaeda-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaeda-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aaeda-105">更新 **[listItem][]** 上的属性。</span><span class="sxs-lookup"><span data-stu-id="aaeda-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaeda-106">权限</span><span class="sxs-lookup"><span data-stu-id="aaeda-106">Permissions</span></span>

<span data-ttu-id="aaeda-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aaeda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaeda-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aaeda-109">Permission type</span></span>      | <span data-ttu-id="aaeda-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aaeda-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaeda-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aaeda-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aaeda-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaeda-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="aaeda-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aaeda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaeda-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aaeda-114">Not supported.</span></span>    |
|<span data-ttu-id="aaeda-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aaeda-115">Application</span></span> | <span data-ttu-id="aaeda-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaeda-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaeda-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aaeda-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="aaeda-118">更新 listItem 上的属性。</span><span class="sxs-lookup"><span data-stu-id="aaeda-118">Update the properties on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

<span data-ttu-id="aaeda-119">更新 listItem 上的列值。</span><span class="sxs-lookup"><span data-stu-id="aaeda-119">Update column values on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="aaeda-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="aaeda-120">Optional request headers</span></span>

| <span data-ttu-id="aaeda-121">名称</span><span class="sxs-lookup"><span data-stu-id="aaeda-121">Name</span></span>       | <span data-ttu-id="aaeda-122">值</span><span class="sxs-lookup"><span data-stu-id="aaeda-122">Value</span></span> | <span data-ttu-id="aaeda-123">说明</span><span class="sxs-lookup"><span data-stu-id="aaeda-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="aaeda-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="aaeda-124">_if-match_</span></span> | <span data-ttu-id="aaeda-125">etag</span><span class="sxs-lookup"><span data-stu-id="aaeda-125">etag</span></span>  | <span data-ttu-id="aaeda-126">如果包含此请求标头，且提供的 eTag 与项中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应，并且不会更新该项。</span><span class="sxs-lookup"><span data-stu-id="aaeda-126">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>

## <a name="request-body"></a><span data-ttu-id="aaeda-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aaeda-127">Request body</span></span> 
<span data-ttu-id="aaeda-128">在请求正文中，提供指定要更新的字段的 [fieldValueSet][] 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aaeda-128">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="response"></a><span data-ttu-id="aaeda-129">响应</span><span class="sxs-lookup"><span data-stu-id="aaeda-129">Response</span></span> 

<span data-ttu-id="aaeda-130">如果成功，此方法在已更新列表项的响应正文中返回`201 Created`响应代码和 [fieldValueSet][]。</span><span class="sxs-lookup"><span data-stu-id="aaeda-130">If successful, this method returns a `201 Created` response code and a [fieldValueSet][] in the response body for the updated list item.</span></span>

## <a name="example"></a><span data-ttu-id="aaeda-131">示例</span><span class="sxs-lookup"><span data-stu-id="aaeda-131">Example</span></span>

<span data-ttu-id="aaeda-132">下面是一个示例，使用新值更新列表项的**颜色**和**数量**字段。</span><span class="sxs-lookup"><span data-stu-id="aaeda-132">The following example updates the **Color** and **Quantity** fields of the list item with new values.</span></span> <span data-ttu-id="aaeda-133">**listItem** 上的所有其他值都保持独立。</span><span class="sxs-lookup"><span data-stu-id="aaeda-133">All other values on the **listItem** are left alone.</span></span> 

### <a name="request"></a><span data-ttu-id="aaeda-134">请求</span><span class="sxs-lookup"><span data-stu-id="aaeda-134">Request</span></span> 


# <a name="http"></a>[<span data-ttu-id="aaeda-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="aaeda-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="c"></a>[<span data-ttu-id="aaeda-136">C#</span><span class="sxs-lookup"><span data-stu-id="aaeda-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aaeda-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aaeda-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aaeda-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aaeda-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aaeda-139">Java</span><span class="sxs-lookup"><span data-stu-id="aaeda-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aaeda-140">响应</span><span class="sxs-lookup"><span data-stu-id="aaeda-140">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
  ]
} -->

