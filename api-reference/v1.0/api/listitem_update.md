---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "更新 SharePoint 列表中的记录"
ms.openlocfilehash: fc025ef8c38a7d0768240038955187ee551d6b42
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="6f4e7-102">更新列表中的项</span><span class="sxs-lookup"><span data-stu-id="6f4e7-102">Update an item in a list</span></span>

<span data-ttu-id="6f4e7-103">更新 **[listItem][]** 上的属性。</span><span class="sxs-lookup"><span data-stu-id="6f4e7-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f4e7-104">权限</span><span class="sxs-lookup"><span data-stu-id="6f4e7-104">Permissions</span></span>

<span data-ttu-id="6f4e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6f4e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6f4e7-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f4e7-107">Permission type</span></span>      | <span data-ttu-id="6f4e7-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f4e7-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f4e7-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f4e7-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6f4e7-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f4e7-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f4e7-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f4e7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f4e7-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f4e7-112">Not supported.</span></span>    |
|<span data-ttu-id="6f4e7-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f4e7-113">Application</span></span> | <span data-ttu-id="6f4e7-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f4e7-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f4e7-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f4e7-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="6f4e7-116">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="6f4e7-116">Optional request headers</span></span>

| <span data-ttu-id="6f4e7-117">名称</span><span class="sxs-lookup"><span data-stu-id="6f4e7-117">Name</span></span>       | <span data-ttu-id="6f4e7-118">值</span><span class="sxs-lookup"><span data-stu-id="6f4e7-118">Value</span></span> | <span data-ttu-id="6f4e7-119">说明</span><span class="sxs-lookup"><span data-stu-id="6f4e7-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="6f4e7-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="6f4e7-120">_if-match_</span></span> | <span data-ttu-id="6f4e7-121">etag</span><span class="sxs-lookup"><span data-stu-id="6f4e7-121">etag</span></span>  | <span data-ttu-id="6f4e7-122">如果包含此请求标头，且提供的 eTag 与项上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应并且不会更新该项。</span><span class="sxs-lookup"><span data-stu-id="6f4e7-122">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>


## <a name="request-body"></a><span data-ttu-id="6f4e7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f4e7-123">Request body</span></span>

<span data-ttu-id="6f4e7-124">在请求正文中，提供指定要更新的字段的 [fieldValueSet][] 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f4e7-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="6f4e7-125">示例</span><span class="sxs-lookup"><span data-stu-id="6f4e7-125">Example</span></span>

<span data-ttu-id="6f4e7-126">下面的示例使用新值更新列表项的“颜色”和“数量”字段。</span><span class="sxs-lookup"><span data-stu-id="6f4e7-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="6f4e7-127">listItem 上的所有其他值都保持不变。</span><span class="sxs-lookup"><span data-stu-id="6f4e7-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="6f4e7-128">响应</span><span class="sxs-lookup"><span data-stu-id="6f4e7-128">Response</span></span>

<span data-ttu-id="6f4e7-129">如果成功，此方法将在已更新列表项的响应正文中返回 [fieldValueSet][]。</span><span class="sxs-lookup"><span data-stu-id="6f4e7-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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

[fieldValueSet]: ../resources/fieldValueSet.md
[listItem]: ../resources/listItem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update"
} -->
