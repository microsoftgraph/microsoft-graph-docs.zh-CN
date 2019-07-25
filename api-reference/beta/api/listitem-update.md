---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 更新 SharePoint 列表中的记录
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b8c0b3db13b956776357f99bad4c8aa7ac338a77
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880179"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="05a53-102">更新列表中的项</span><span class="sxs-lookup"><span data-stu-id="05a53-102">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05a53-103">更新 **[listItem][]** 上的属性。</span><span class="sxs-lookup"><span data-stu-id="05a53-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="05a53-104">权限</span><span class="sxs-lookup"><span data-stu-id="05a53-104">Permissions</span></span>

<span data-ttu-id="05a53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05a53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05a53-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="05a53-107">Permission type</span></span>      | <span data-ttu-id="05a53-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05a53-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05a53-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05a53-109">Delegated (work or school account)</span></span> | <span data-ttu-id="05a53-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05a53-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="05a53-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05a53-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05a53-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="05a53-112">Not supported.</span></span>    |
|<span data-ttu-id="05a53-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="05a53-113">Application</span></span> | <span data-ttu-id="05a53-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05a53-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05a53-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05a53-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="05a53-116">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="05a53-116">Optional request headers</span></span>

| <span data-ttu-id="05a53-117">名称</span><span class="sxs-lookup"><span data-stu-id="05a53-117">Name</span></span>       | <span data-ttu-id="05a53-118">值</span><span class="sxs-lookup"><span data-stu-id="05a53-118">Value</span></span> | <span data-ttu-id="05a53-119">说明</span><span class="sxs-lookup"><span data-stu-id="05a53-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="05a53-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="05a53-120">_if-match_</span></span> | <span data-ttu-id="05a53-121">etag</span><span class="sxs-lookup"><span data-stu-id="05a53-121">etag</span></span>  | <span data-ttu-id="05a53-122">如果包含此请求标头，且提供的 eTag 与项中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应，并且不会更新该项。</span><span class="sxs-lookup"><span data-stu-id="05a53-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="05a53-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="05a53-123">Request body</span></span>

<span data-ttu-id="05a53-124">在请求正文中，提供指定要更新的字段的 [fieldValueSet][] 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05a53-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="05a53-125">示例</span><span class="sxs-lookup"><span data-stu-id="05a53-125">Example</span></span>

<span data-ttu-id="05a53-126">下面是一个示例，使用新值更新列表项的“颜色”和“数量”字段。</span><span class="sxs-lookup"><span data-stu-id="05a53-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="05a53-127">listItem 上的所有其他值都保持独立。</span><span class="sxs-lookup"><span data-stu-id="05a53-127">All other values on the listItem are left alone.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="05a53-128">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="05a53-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="05a53-129">C#</span><span class="sxs-lookup"><span data-stu-id="05a53-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05a53-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="05a53-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="05a53-131">目标-C</span><span class="sxs-lookup"><span data-stu-id="05a53-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="05a53-132">Java</span><span class="sxs-lookup"><span data-stu-id="05a53-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="05a53-133">响应</span><span class="sxs-lookup"><span data-stu-id="05a53-133">Response</span></span>

<span data-ttu-id="05a53-134">如果成功，此方法在已更新列表项的响应正文中返回 [fieldValueSet][]。</span><span class="sxs-lookup"><span data-stu-id="05a53-134">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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
