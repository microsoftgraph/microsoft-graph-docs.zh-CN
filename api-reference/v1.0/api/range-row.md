---
title: Range:Row
description: 获取范围中包含的行。
author: lumine2008
ms.openlocfilehash: d758af607fa80314abe6c3f90e611eb87ac62914
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315027"
---
# <a name="range-row"></a><span data-ttu-id="f7e6f-103">Range:Row</span><span class="sxs-lookup"><span data-stu-id="f7e6f-103">Range: Row</span></span>

<span data-ttu-id="f7e6f-104">获取范围中包含的行。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-104">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7e6f-105">权限</span><span class="sxs-lookup"><span data-stu-id="f7e6f-105">Permissions</span></span>
<span data-ttu-id="f7e6f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e6f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7e6f-108">Permission type</span></span>      | <span data-ttu-id="f7e6f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7e6f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7e6f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7e6f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7e6f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7e6f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7e6f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7e6f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7e6f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-113">Not supported.</span></span>    |
|<span data-ttu-id="f7e6f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7e6f-114">Application</span></span> | <span data-ttu-id="f7e6f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7e6f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7e6f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/row
POST /workbook/worksheets/{id|name}/range(address='<address>')/row
POST /workbook/tables/{id|name}/columns/{id|name}/range/row

```
## <a name="request-headers"></a><span data-ttu-id="f7e6f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7e6f-117">Request headers</span></span>
| <span data-ttu-id="f7e6f-118">Name</span><span class="sxs-lookup"><span data-stu-id="f7e6f-118">Name</span></span>       | <span data-ttu-id="f7e6f-119">说明</span><span class="sxs-lookup"><span data-stu-id="f7e6f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7e6f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7e6f-120">Authorization</span></span>  | <span data-ttu-id="f7e6f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7e6f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f7e6f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f7e6f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7e6f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7e6f-126">Request body</span></span>
<span data-ttu-id="f7e6f-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7e6f-128">参数</span><span class="sxs-lookup"><span data-stu-id="f7e6f-128">Parameter</span></span>    | <span data-ttu-id="f7e6f-129">Type</span><span class="sxs-lookup"><span data-stu-id="f7e6f-129">Type</span></span>   |<span data-ttu-id="f7e6f-130">说明</span><span class="sxs-lookup"><span data-stu-id="f7e6f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7e6f-131">row</span><span class="sxs-lookup"><span data-stu-id="f7e6f-131">row</span></span>|<span data-ttu-id="f7e6f-132">Int32</span><span class="sxs-lookup"><span data-stu-id="f7e6f-132">Int32</span></span>|<span data-ttu-id="f7e6f-p104">要检索的区域的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-p104">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="f7e6f-135">响应</span><span class="sxs-lookup"><span data-stu-id="f7e6f-135">Response</span></span>

<span data-ttu-id="f7e6f-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7e6f-137">示例</span><span class="sxs-lookup"><span data-stu-id="f7e6f-137">Example</span></span>
<span data-ttu-id="f7e6f-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f7e6f-139">请求</span><span class="sxs-lookup"><span data-stu-id="f7e6f-139">Request</span></span>
<span data-ttu-id="f7e6f-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_row",
  "idempotent": true,
  "@type": "requestBodyResourceFor.range_row"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/row
Content-type: application/json
Content-length: 18

{
  "row": 2
}
```

##### <a name="response"></a><span data-ttu-id="f7e6f-141">响应</span><span class="sxs-lookup"><span data-stu-id="f7e6f-141">Response</span></span>
<span data-ttu-id="f7e6f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7e6f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Row",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->