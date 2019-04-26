---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 更新 SharePoint 列表中的记录
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f80f2607e953ba760893170366179f6751d9665d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541407"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="42a37-102">更新列表中的项</span><span class="sxs-lookup"><span data-stu-id="42a37-102">Update an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42a37-103">更新 **[listItem][]** 上的属性。</span><span class="sxs-lookup"><span data-stu-id="42a37-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="42a37-104">权限</span><span class="sxs-lookup"><span data-stu-id="42a37-104">Permissions</span></span>

<span data-ttu-id="42a37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42a37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42a37-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="42a37-107">Permission type</span></span>      | <span data-ttu-id="42a37-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42a37-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42a37-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42a37-109">Delegated (work or school account)</span></span> | <span data-ttu-id="42a37-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42a37-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="42a37-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42a37-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42a37-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="42a37-112">Not supported.</span></span>    |
|<span data-ttu-id="42a37-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="42a37-113">Application</span></span> | <span data-ttu-id="42a37-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42a37-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42a37-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42a37-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="42a37-116">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="42a37-116">Optional request headers</span></span>

| <span data-ttu-id="42a37-117">名称</span><span class="sxs-lookup"><span data-stu-id="42a37-117">Name</span></span>       | <span data-ttu-id="42a37-118">值</span><span class="sxs-lookup"><span data-stu-id="42a37-118">Value</span></span> | <span data-ttu-id="42a37-119">说明</span><span class="sxs-lookup"><span data-stu-id="42a37-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="42a37-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="42a37-120">_if-match_</span></span> | <span data-ttu-id="42a37-121">etag</span><span class="sxs-lookup"><span data-stu-id="42a37-121">etag</span></span>  | <span data-ttu-id="42a37-122">如果包含此请求标头，且提供的 eTag 与项中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应，并且不会更新该项。</span><span class="sxs-lookup"><span data-stu-id="42a37-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="42a37-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="42a37-123">Request body</span></span>

<span data-ttu-id="42a37-124">在请求正文中，提供指定要更新的字段的 [fieldValueSet][] 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42a37-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="42a37-125">示例</span><span class="sxs-lookup"><span data-stu-id="42a37-125">Example</span></span>

<span data-ttu-id="42a37-126">下面是一个示例，使用新值更新列表项的“颜色”和“数量”字段。</span><span class="sxs-lookup"><span data-stu-id="42a37-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="42a37-127">listItem 上的所有其他值都保持独立。</span><span class="sxs-lookup"><span data-stu-id="42a37-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="42a37-128">响应</span><span class="sxs-lookup"><span data-stu-id="42a37-128">Response</span></span>

<span data-ttu-id="42a37-129">如果成功，此方法在已更新列表项的响应正文中返回 [fieldValueSet][]。</span><span class="sxs-lookup"><span data-stu-id="42a37-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

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
  "suppressions": []
}
-->
