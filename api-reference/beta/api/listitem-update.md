---
author: JeremyKelley
description: 更新 listItem 上的属性。
ms.date: 09/11/2017
title: 更新 SharePoint 列表中的记录
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4c97e9fbb9957a7d0f652c106d1bf427d16d0898
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475840"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="4b476-103">更新列表中的项</span><span class="sxs-lookup"><span data-stu-id="4b476-103">Update an item in a list</span></span>

<span data-ttu-id="4b476-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b476-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b476-105">更新 **[listItem][]** 上的属性。</span><span class="sxs-lookup"><span data-stu-id="4b476-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b476-106">权限</span><span class="sxs-lookup"><span data-stu-id="4b476-106">Permissions</span></span>

<span data-ttu-id="4b476-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b476-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b476-109">Permission type</span></span>      | <span data-ttu-id="4b476-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b476-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b476-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b476-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4b476-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b476-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b476-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b476-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b476-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b476-114">Not supported.</span></span>    |
|<span data-ttu-id="4b476-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b476-115">Application</span></span> | <span data-ttu-id="4b476-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b476-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b476-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b476-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="4b476-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="4b476-118">Optional request headers</span></span>

| <span data-ttu-id="4b476-119">名称</span><span class="sxs-lookup"><span data-stu-id="4b476-119">Name</span></span>       | <span data-ttu-id="4b476-120">值</span><span class="sxs-lookup"><span data-stu-id="4b476-120">Value</span></span> | <span data-ttu-id="4b476-121">说明</span><span class="sxs-lookup"><span data-stu-id="4b476-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="4b476-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="4b476-122">_if-match_</span></span> | <span data-ttu-id="4b476-123">etag</span><span class="sxs-lookup"><span data-stu-id="4b476-123">etag</span></span>  | <span data-ttu-id="4b476-124">如果包含此请求标头，且提供的 eTag 与项中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应，并且不会更新该项。</span><span class="sxs-lookup"><span data-stu-id="4b476-124">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="4b476-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b476-125">Request body</span></span>

<span data-ttu-id="4b476-126">在请求正文中，提供指定要更新的字段的 [fieldValueSet][] 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b476-126">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="4b476-127">示例</span><span class="sxs-lookup"><span data-stu-id="4b476-127">Example</span></span>

<span data-ttu-id="4b476-128">下面是一个示例，使用新值更新列表项的“颜色”和“数量”字段。</span><span class="sxs-lookup"><span data-stu-id="4b476-128">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="4b476-129">listItem 上的所有其他值都保持独立。</span><span class="sxs-lookup"><span data-stu-id="4b476-129">All other values on the listItem are left alone.</span></span> 


# <a name="http"></a>[<span data-ttu-id="4b476-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b476-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="c"></a>[<span data-ttu-id="4b476-131">C#</span><span class="sxs-lookup"><span data-stu-id="4b476-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b476-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b476-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b476-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b476-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="4b476-134">响应</span><span class="sxs-lookup"><span data-stu-id="4b476-134">Response</span></span>

<span data-ttu-id="4b476-135">如果成功，此方法在已更新列表项的响应正文中返回 [fieldValueSet][]。</span><span class="sxs-lookup"><span data-stu-id="4b476-135">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```http
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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
  ]
}
-->


