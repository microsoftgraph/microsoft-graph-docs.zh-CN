---
author: JeremyKelley
ms.author: JeremyKelley
title: 更新 listItem
description: 更新 **[listItem][]** 上的属性。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: cbda0492ff0435e23e3bb33ceb75d3461d141a1a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271951"
---
# <a name="update-listitem"></a><span data-ttu-id="c5752-103">更新 listItem</span><span class="sxs-lookup"><span data-stu-id="c5752-103">Update listItem</span></span>

<span data-ttu-id="c5752-104">更新 **[listItem][]** 上的属性。</span><span class="sxs-lookup"><span data-stu-id="c5752-104">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5752-105">权限</span><span class="sxs-lookup"><span data-stu-id="c5752-105">Permissions</span></span>

<span data-ttu-id="c5752-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5752-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5752-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5752-108">Permission type</span></span>      | <span data-ttu-id="c5752-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5752-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5752-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5752-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c5752-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5752-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c5752-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5752-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5752-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5752-113">Not supported.</span></span>    |
|<span data-ttu-id="c5752-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5752-114">Application</span></span> | <span data-ttu-id="c5752-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5752-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5752-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5752-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="c5752-117">更新 listItem 上的属性。</span><span class="sxs-lookup"><span data-stu-id="c5752-117">Update the properties on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

<span data-ttu-id="c5752-118">更新 listItem 上的列值。</span><span class="sxs-lookup"><span data-stu-id="c5752-118">Update column values on a listItem.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="c5752-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="c5752-119">Optional request headers</span></span>

| <span data-ttu-id="c5752-120">名称</span><span class="sxs-lookup"><span data-stu-id="c5752-120">Name</span></span>       | <span data-ttu-id="c5752-121">值</span><span class="sxs-lookup"><span data-stu-id="c5752-121">Value</span></span> | <span data-ttu-id="c5752-122">说明</span><span class="sxs-lookup"><span data-stu-id="c5752-122">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="c5752-123">_if-match_</span><span class="sxs-lookup"><span data-stu-id="c5752-123">_if-match_</span></span> | <span data-ttu-id="c5752-124">etag</span><span class="sxs-lookup"><span data-stu-id="c5752-124">etag</span></span>  | <span data-ttu-id="c5752-125">如果包含此请求标头，且提供的 eTag 与项中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应，并且不会更新该项。</span><span class="sxs-lookup"><span data-stu-id="c5752-125">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>

## <a name="request-body"></a><span data-ttu-id="c5752-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5752-126">Request body</span></span> 
<span data-ttu-id="c5752-127">在请求正文中，提供指定要更新的字段的 [fieldValueSet][] 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5752-127">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="response"></a><span data-ttu-id="c5752-128">响应</span><span class="sxs-lookup"><span data-stu-id="c5752-128">Response</span></span> 

<span data-ttu-id="c5752-129">如果成功，此方法在已更新列表项的响应正文中返回`201 Created`响应代码和 [fieldValueSet][]。</span><span class="sxs-lookup"><span data-stu-id="c5752-129">If successful, this method returns a `201 Created` response code and a [fieldValueSet][] in the response body for the updated list item.</span></span>

## <a name="example"></a><span data-ttu-id="c5752-130">示例</span><span class="sxs-lookup"><span data-stu-id="c5752-130">Example</span></span>

<span data-ttu-id="c5752-131">下面是一个示例，使用新值更新列表项的**颜色**和**数量**字段。</span><span class="sxs-lookup"><span data-stu-id="c5752-131">The following example updates the **Color** and **Quantity** fields of the list item with new values.</span></span> <span data-ttu-id="c5752-132">**listItem** 上的所有其他值都保持独立。</span><span class="sxs-lookup"><span data-stu-id="c5752-132">All other values on the **listItem** are left alone.</span></span> 

### <a name="request"></a><span data-ttu-id="c5752-133">请求</span><span class="sxs-lookup"><span data-stu-id="c5752-133">Request</span></span> 

<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

### <a name="response"></a><span data-ttu-id="c5752-134">响应</span><span class="sxs-lookup"><span data-stu-id="c5752-134">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c5752-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c5752-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c5752-136">C#</span><span class="sxs-lookup"><span data-stu-id="c5752-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5752-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="c5752-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update-listitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c5752-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5752-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update-listitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
