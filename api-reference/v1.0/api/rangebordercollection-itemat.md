---
title: 'RangeBorderCollection: ItemAt'
description: 使用其索引获取 border 对象
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 037c040feaf65e6a6367b4eca8142524bc046772
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35461174"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="fa889-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="fa889-103">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="fa889-104">使用其索引获取 border 对象</span><span class="sxs-lookup"><span data-stu-id="fa889-104">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="fa889-105">权限</span><span class="sxs-lookup"><span data-stu-id="fa889-105">Permissions</span></span>
<span data-ttu-id="fa889-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa889-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa889-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa889-108">Permission type</span></span>      | <span data-ttu-id="fa889-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa889-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa889-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa889-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa889-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa889-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fa889-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa889-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa889-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa889-113">Not supported.</span></span>    |
|<span data-ttu-id="fa889-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa889-114">Application</span></span> | <span data-ttu-id="fa889-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa889-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa889-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa889-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa889-117">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fa889-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders/itemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/itemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="fa889-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa889-118">Request headers</span></span>
| <span data-ttu-id="fa889-119">名称</span><span class="sxs-lookup"><span data-stu-id="fa889-119">Name</span></span>       | <span data-ttu-id="fa889-120">说明</span><span class="sxs-lookup"><span data-stu-id="fa889-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fa889-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa889-121">Authorization</span></span>  | <span data-ttu-id="fa889-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa889-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa889-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fa889-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="fa889-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="fa889-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa889-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa889-127">Request body</span></span>
<span data-ttu-id="fa889-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fa889-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa889-129">参数</span><span class="sxs-lookup"><span data-stu-id="fa889-129">Parameter</span></span>    | <span data-ttu-id="fa889-130">类型</span><span class="sxs-lookup"><span data-stu-id="fa889-130">Type</span></span>   |<span data-ttu-id="fa889-131">说明</span><span class="sxs-lookup"><span data-stu-id="fa889-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa889-132">index</span><span class="sxs-lookup"><span data-stu-id="fa889-132">index</span></span>|<span data-ttu-id="fa889-133">Int32</span><span class="sxs-lookup"><span data-stu-id="fa889-133">Int32</span></span>|<span data-ttu-id="fa889-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="fa889-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="fa889-136">响应</span><span class="sxs-lookup"><span data-stu-id="fa889-136">Response</span></span>

<span data-ttu-id="fa889-137">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[WorkbookRangeBorder](../resources/rangeborder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fa889-137">If successful, this method returns `200 OK` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa889-138">示例</span><span class="sxs-lookup"><span data-stu-id="fa889-138">Example</span></span>
<span data-ttu-id="fa889-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fa889-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fa889-140">请求</span><span class="sxs-lookup"><span data-stu-id="fa889-140">Request</span></span>
<span data-ttu-id="fa889-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa889-141">Here is an example of the request.</span></span>
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa889-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa889-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangebordercollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa889-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="fa889-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangebordercollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fa889-144">响应</span><span class="sxs-lookup"><span data-stu-id="fa889-144">Response</span></span>
<span data-ttu-id="fa889-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa889-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
