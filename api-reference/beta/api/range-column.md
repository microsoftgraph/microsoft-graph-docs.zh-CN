---
title: Range:Column
description: 获取范围中包含的列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 04724e43b5e26d89dcefc71c07a23051a6ed9719
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526016"
---
# <a name="range-column"></a><span data-ttu-id="28d51-103">Range:Column</span><span class="sxs-lookup"><span data-stu-id="28d51-103">Range: Column</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28d51-104">获取范围中包含的列。</span><span class="sxs-lookup"><span data-stu-id="28d51-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="28d51-105">权限</span><span class="sxs-lookup"><span data-stu-id="28d51-105">Permissions</span></span>
<span data-ttu-id="28d51-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28d51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28d51-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="28d51-108">Permission type</span></span>      | <span data-ttu-id="28d51-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28d51-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28d51-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28d51-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28d51-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28d51-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="28d51-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28d51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28d51-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28d51-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="28d51-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="28d51-114">Application</span></span> | <span data-ttu-id="28d51-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="28d51-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28d51-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28d51-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Column
GET /workbook/worksheets/{id|name}/range(address='<address>')/Column
GET /workbook/tables/{id|name}/columns/{id|name}/range/Column

```
## <a name="request-headers"></a><span data-ttu-id="28d51-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="28d51-117">Request headers</span></span>
| <span data-ttu-id="28d51-118">名称</span><span class="sxs-lookup"><span data-stu-id="28d51-118">Name</span></span>       | <span data-ttu-id="28d51-119">说明</span><span class="sxs-lookup"><span data-stu-id="28d51-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="28d51-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="28d51-120">Authorization</span></span>  | <span data-ttu-id="28d51-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28d51-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28d51-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="28d51-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="28d51-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="28d51-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28d51-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="28d51-126">Request body</span></span>
<span data-ttu-id="28d51-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="28d51-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="28d51-128">参数</span><span class="sxs-lookup"><span data-stu-id="28d51-128">Parameter</span></span>    | <span data-ttu-id="28d51-129">类型</span><span class="sxs-lookup"><span data-stu-id="28d51-129">Type</span></span>   |<span data-ttu-id="28d51-130">说明</span><span class="sxs-lookup"><span data-stu-id="28d51-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28d51-131">column</span><span class="sxs-lookup"><span data-stu-id="28d51-131">column</span></span>|<span data-ttu-id="28d51-132">number</span><span class="sxs-lookup"><span data-stu-id="28d51-132">number</span></span>|<span data-ttu-id="28d51-p104">要检索的区域的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="28d51-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="28d51-135">响应</span><span class="sxs-lookup"><span data-stu-id="28d51-135">Response</span></span>

<span data-ttu-id="28d51-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="28d51-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28d51-137">示例</span><span class="sxs-lookup"><span data-stu-id="28d51-137">Example</span></span>
<span data-ttu-id="28d51-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="28d51-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="28d51-139">请求</span><span class="sxs-lookup"><span data-stu-id="28d51-139">Request</span></span>
<span data-ttu-id="28d51-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28d51-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Column
Content-type: application/json
Content-length: 21

{
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="28d51-141">响应</span><span class="sxs-lookup"><span data-stu-id="28d51-141">Response</span></span>
<span data-ttu-id="28d51-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="28d51-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-column.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
