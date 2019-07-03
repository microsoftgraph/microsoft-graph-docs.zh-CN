---
author: JeremyKelley
ms.author: JeremyKelley
title: 更新 listItem
description: 更新 **[listItem][]** 上的属性。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 3b13f48c514a753e68e6b556130bb5e9147f0f75
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460712"
---
# <a name="update-listitem"></a><span data-ttu-id="21237-103">更新 listItem</span><span class="sxs-lookup"><span data-stu-id="21237-103">Update listItem</span></span>

<span data-ttu-id="21237-104">更新 **[listItem][]** 上的属性。</span><span class="sxs-lookup"><span data-stu-id="21237-104">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="21237-105">权限</span><span class="sxs-lookup"><span data-stu-id="21237-105">Permissions</span></span>

<span data-ttu-id="21237-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21237-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21237-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="21237-108">Permission type</span></span>      | <span data-ttu-id="21237-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21237-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21237-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21237-110">Delegated (work or school account)</span></span> | <span data-ttu-id="21237-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21237-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="21237-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21237-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21237-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="21237-113">Not supported.</span></span>    |
|<span data-ttu-id="21237-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="21237-114">Application</span></span> | <span data-ttu-id="21237-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21237-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21237-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21237-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="21237-117">更新 listItem 上的属性。</span><span class="sxs-lookup"><span data-stu-id="21237-117">Update the properties on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

<span data-ttu-id="21237-118">更新 listItem 上的列值。</span><span class="sxs-lookup"><span data-stu-id="21237-118">Update column values on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="21237-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="21237-119">Optional request headers</span></span>

| <span data-ttu-id="21237-120">名称</span><span class="sxs-lookup"><span data-stu-id="21237-120">Name</span></span>       | <span data-ttu-id="21237-121">值</span><span class="sxs-lookup"><span data-stu-id="21237-121">Value</span></span> | <span data-ttu-id="21237-122">说明</span><span class="sxs-lookup"><span data-stu-id="21237-122">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="21237-123">_if-match_</span><span class="sxs-lookup"><span data-stu-id="21237-123">_if-match_</span></span> | <span data-ttu-id="21237-124">etag</span><span class="sxs-lookup"><span data-stu-id="21237-124">etag</span></span>  | <span data-ttu-id="21237-125">如果包含此请求标头，且提供的 eTag 与项中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应，并且不会更新该项。</span><span class="sxs-lookup"><span data-stu-id="21237-125">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>

## <a name="request-body"></a><span data-ttu-id="21237-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="21237-126">Request body</span></span> 
<span data-ttu-id="21237-127">在请求正文中，提供指定要更新的字段的 [fieldValueSet][] 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21237-127">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="response"></a><span data-ttu-id="21237-128">响应</span><span class="sxs-lookup"><span data-stu-id="21237-128">Response</span></span> 

<span data-ttu-id="21237-129">如果成功，此方法在已更新列表项的响应正文中返回`201 Created`响应代码和 [fieldValueSet][]。</span><span class="sxs-lookup"><span data-stu-id="21237-129">If successful, this method returns a `201 Created` response code and a [fieldValueSet][] in the response body for the updated list item.</span></span>

## <a name="example"></a><span data-ttu-id="21237-130">示例</span><span class="sxs-lookup"><span data-stu-id="21237-130">Example</span></span>

<span data-ttu-id="21237-131">下面是一个示例，使用新值更新列表项的**颜色**和**数量**字段。</span><span class="sxs-lookup"><span data-stu-id="21237-131">The following example updates the **Color** and **Quantity** fields of the list item with new values.</span></span> <span data-ttu-id="21237-132">**listItem** 上的所有其他值都保持独立。</span><span class="sxs-lookup"><span data-stu-id="21237-132">All other values on the **listItem** are left alone.</span></span> 

### <a name="request"></a><span data-ttu-id="21237-133">请求</span><span class="sxs-lookup"><span data-stu-id="21237-133">Request</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="21237-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="21237-134">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="21237-135">C#</span><span class="sxs-lookup"><span data-stu-id="21237-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21237-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="21237-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21237-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21237-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="21237-138">响应</span><span class="sxs-lookup"><span data-stu-id="21237-138">Response</span></span>

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
