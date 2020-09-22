---
author: JeremyKelley
description: 更新 listItem 上的属性。
ms.date: 09/11/2017
title: 更新 SharePoint 列表中的记录
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b696c2417168de43d43770789dd8fdaf58ef59e5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062447"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="a3ef7-103">更新列表中的项</span><span class="sxs-lookup"><span data-stu-id="a3ef7-103">Update an item in a list</span></span>

<span data-ttu-id="a3ef7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3ef7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3ef7-105">更新 **[listItem][]** 上的属性。</span><span class="sxs-lookup"><span data-stu-id="a3ef7-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3ef7-106">权限</span><span class="sxs-lookup"><span data-stu-id="a3ef7-106">Permissions</span></span>

<span data-ttu-id="a3ef7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3ef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3ef7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3ef7-109">Permission type</span></span>      | <span data-ttu-id="a3ef7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3ef7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3ef7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3ef7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a3ef7-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3ef7-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3ef7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3ef7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3ef7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3ef7-114">Not supported.</span></span>    |
|<span data-ttu-id="a3ef7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3ef7-115">Application</span></span> | <span data-ttu-id="a3ef7-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3ef7-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3ef7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3ef7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="a3ef7-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="a3ef7-118">Optional request headers</span></span>

| <span data-ttu-id="a3ef7-119">名称</span><span class="sxs-lookup"><span data-stu-id="a3ef7-119">Name</span></span>       | <span data-ttu-id="a3ef7-120">值</span><span class="sxs-lookup"><span data-stu-id="a3ef7-120">Value</span></span> | <span data-ttu-id="a3ef7-121">说明</span><span class="sxs-lookup"><span data-stu-id="a3ef7-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="a3ef7-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="a3ef7-122">_if-match_</span></span> | <span data-ttu-id="a3ef7-123">etag</span><span class="sxs-lookup"><span data-stu-id="a3ef7-123">etag</span></span>  | <span data-ttu-id="a3ef7-124">如果包含此请求标头，且提供的 eTag 与项中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应，并且不会更新该项。</span><span class="sxs-lookup"><span data-stu-id="a3ef7-124">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="a3ef7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3ef7-125">Request body</span></span>

<span data-ttu-id="a3ef7-126">在请求正文中，提供指定要更新的字段的 [fieldValueSet][] 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3ef7-126">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="a3ef7-127">示例</span><span class="sxs-lookup"><span data-stu-id="a3ef7-127">Example</span></span>

<span data-ttu-id="a3ef7-128">下面是一个示例，使用新值更新列表项的“颜色”和“数量”字段。</span><span class="sxs-lookup"><span data-stu-id="a3ef7-128">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="a3ef7-129">listItem 上的所有其他值都保持独立。</span><span class="sxs-lookup"><span data-stu-id="a3ef7-129">All other values on the listItem are left alone.</span></span> 


# <a name="http"></a>[<span data-ttu-id="a3ef7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3ef7-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="c"></a>[<span data-ttu-id="a3ef7-131">C#</span><span class="sxs-lookup"><span data-stu-id="a3ef7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3ef7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3ef7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3ef7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3ef7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="a3ef7-134">响应</span><span class="sxs-lookup"><span data-stu-id="a3ef7-134">Response</span></span>

<span data-ttu-id="a3ef7-135">如果成功，此方法在已更新列表项的响应正文中返回 [fieldValueSet][]。</span><span class="sxs-lookup"><span data-stu-id="a3ef7-135">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

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


