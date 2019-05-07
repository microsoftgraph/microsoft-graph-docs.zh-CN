---
title: 'RangeBorderCollection: ItemAt'
description: 使用其索引获取 border 对象
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2e206f1f0a4f01a3e2720ef9c60cee35b0160ca7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607834"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="7e6af-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="7e6af-103">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="7e6af-104">使用其索引获取 border 对象</span><span class="sxs-lookup"><span data-stu-id="7e6af-104">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="7e6af-105">权限</span><span class="sxs-lookup"><span data-stu-id="7e6af-105">Permissions</span></span>
<span data-ttu-id="7e6af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e6af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e6af-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e6af-108">Permission type</span></span>      | <span data-ttu-id="7e6af-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e6af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e6af-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e6af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e6af-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e6af-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7e6af-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e6af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e6af-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e6af-113">Not supported.</span></span>    |
|<span data-ttu-id="7e6af-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e6af-114">Application</span></span> | <span data-ttu-id="7e6af-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e6af-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e6af-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e6af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders/itemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/itemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="7e6af-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e6af-117">Request headers</span></span>
| <span data-ttu-id="7e6af-118">名称</span><span class="sxs-lookup"><span data-stu-id="7e6af-118">Name</span></span>       | <span data-ttu-id="7e6af-119">说明</span><span class="sxs-lookup"><span data-stu-id="7e6af-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7e6af-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e6af-120">Authorization</span></span>  | <span data-ttu-id="7e6af-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e6af-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e6af-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7e6af-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7e6af-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7e6af-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e6af-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e6af-126">Request body</span></span>
<span data-ttu-id="7e6af-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7e6af-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7e6af-128">参数</span><span class="sxs-lookup"><span data-stu-id="7e6af-128">Parameter</span></span>    | <span data-ttu-id="7e6af-129">类型</span><span class="sxs-lookup"><span data-stu-id="7e6af-129">Type</span></span>   |<span data-ttu-id="7e6af-130">说明</span><span class="sxs-lookup"><span data-stu-id="7e6af-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e6af-131">index</span><span class="sxs-lookup"><span data-stu-id="7e6af-131">index</span></span>|<span data-ttu-id="7e6af-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7e6af-132">Int32</span></span>|<span data-ttu-id="7e6af-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="7e6af-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="7e6af-135">响应</span><span class="sxs-lookup"><span data-stu-id="7e6af-135">Response</span></span>

<span data-ttu-id="7e6af-136">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[WorkbookRangeBorder](../resources/rangeborder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7e6af-136">If successful, this method returns `200 OK` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e6af-137">示例</span><span class="sxs-lookup"><span data-stu-id="7e6af-137">Example</span></span>
<span data-ttu-id="7e6af-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7e6af-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7e6af-139">请求</span><span class="sxs-lookup"><span data-stu-id="7e6af-139">Request</span></span>
<span data-ttu-id="7e6af-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7e6af-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "rangebordercollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 1
}
```

##### <a name="response"></a><span data-ttu-id="7e6af-141">响应</span><span class="sxs-lookup"><span data-stu-id="7e6af-141">Response</span></span>
<span data-ttu-id="7e6af-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7e6af-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7e6af-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7e6af-145">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e6af-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="7e6af-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/rangebordercollection_itemat-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangebordercollection-itemat.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
