---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 更新 SharePoint 列表中的记录
localization_priority: Normal
ms.openlocfilehash: 0b6053f997422f396825aafe058dfd5252986ca1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872476"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="06fdd-102">更新列表中的项</span><span class="sxs-lookup"><span data-stu-id="06fdd-102">Update an item in a list</span></span>

> <span data-ttu-id="06fdd-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="06fdd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06fdd-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="06fdd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06fdd-105">更新 **[listItem][]** 上的属性。</span><span class="sxs-lookup"><span data-stu-id="06fdd-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="06fdd-106">权限</span><span class="sxs-lookup"><span data-stu-id="06fdd-106">Permissions</span></span>

<span data-ttu-id="06fdd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06fdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06fdd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="06fdd-109">Permission type</span></span>      | <span data-ttu-id="06fdd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06fdd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06fdd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06fdd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="06fdd-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fdd-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="06fdd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06fdd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06fdd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="06fdd-114">Not supported.</span></span>    |
|<span data-ttu-id="06fdd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="06fdd-115">Application</span></span> | <span data-ttu-id="06fdd-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fdd-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06fdd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06fdd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="06fdd-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="06fdd-118">Optional request headers</span></span>

| <span data-ttu-id="06fdd-119">名称</span><span class="sxs-lookup"><span data-stu-id="06fdd-119">Name</span></span>       | <span data-ttu-id="06fdd-120">值</span><span class="sxs-lookup"><span data-stu-id="06fdd-120">Value</span></span> | <span data-ttu-id="06fdd-121">说明</span><span class="sxs-lookup"><span data-stu-id="06fdd-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="06fdd-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="06fdd-122">_if-match_</span></span> | <span data-ttu-id="06fdd-123">etag</span><span class="sxs-lookup"><span data-stu-id="06fdd-123">etag</span></span>  | <span data-ttu-id="06fdd-124">如果包含此请求标头，且提供的 eTag 与项中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应，并且不会更新该项。</span><span class="sxs-lookup"><span data-stu-id="06fdd-124">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="06fdd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="06fdd-125">Request body</span></span>

<span data-ttu-id="06fdd-126">在请求正文中，提供指定要更新的字段的 [fieldValueSet][] 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06fdd-126">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="06fdd-127">示例</span><span class="sxs-lookup"><span data-stu-id="06fdd-127">Example</span></span>

<span data-ttu-id="06fdd-128">下面是一个示例，使用新值更新列表项的“颜色”和“数量”字段。</span><span class="sxs-lookup"><span data-stu-id="06fdd-128">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="06fdd-129">listItem 上的所有其他值都保持独立。</span><span class="sxs-lookup"><span data-stu-id="06fdd-129">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="06fdd-130">响应</span><span class="sxs-lookup"><span data-stu-id="06fdd-130">Response</span></span>

<span data-ttu-id="06fdd-131">如果成功，此方法在已更新列表项的响应正文中返回 [fieldValueSet][]。</span><span class="sxs-lookup"><span data-stu-id="06fdd-131">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update"
} -->
