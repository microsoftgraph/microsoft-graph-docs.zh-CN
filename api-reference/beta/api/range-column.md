---
title: Range:Column
description: 获取范围中包含的列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3bd6756568830f2b77c84870037bb14624e4eaa1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980613"
---
# <a name="range-column"></a><span data-ttu-id="a3883-103">Range:Column</span><span class="sxs-lookup"><span data-stu-id="a3883-103">Range: Column</span></span>

> <span data-ttu-id="a3883-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a3883-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3883-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a3883-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3883-106">获取范围中包含的列。</span><span class="sxs-lookup"><span data-stu-id="a3883-106">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3883-107">权限</span><span class="sxs-lookup"><span data-stu-id="a3883-107">Permissions</span></span>
<span data-ttu-id="a3883-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3883-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3883-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3883-110">Permission type</span></span>      | <span data-ttu-id="a3883-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3883-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3883-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3883-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a3883-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3883-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a3883-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3883-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3883-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3883-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a3883-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3883-116">Application</span></span> | <span data-ttu-id="a3883-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3883-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3883-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3883-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Column
GET /workbook/worksheets/{id|name}/range(address='<address>')/Column
GET /workbook/tables/{id|name}/columns/{id|name}/range/Column

```
## <a name="request-headers"></a><span data-ttu-id="a3883-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3883-119">Request headers</span></span>
| <span data-ttu-id="a3883-120">名称</span><span class="sxs-lookup"><span data-stu-id="a3883-120">Name</span></span>       | <span data-ttu-id="a3883-121">说明</span><span class="sxs-lookup"><span data-stu-id="a3883-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a3883-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3883-122">Authorization</span></span>  | <span data-ttu-id="a3883-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3883-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a3883-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a3883-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a3883-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a3883-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3883-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3883-128">Request body</span></span>
<span data-ttu-id="a3883-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a3883-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a3883-130">参数</span><span class="sxs-lookup"><span data-stu-id="a3883-130">Parameter</span></span>    | <span data-ttu-id="a3883-131">类型</span><span class="sxs-lookup"><span data-stu-id="a3883-131">Type</span></span>   |<span data-ttu-id="a3883-132">说明</span><span class="sxs-lookup"><span data-stu-id="a3883-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3883-133">column</span><span class="sxs-lookup"><span data-stu-id="a3883-133">column</span></span>|<span data-ttu-id="a3883-134">number</span><span class="sxs-lookup"><span data-stu-id="a3883-134">number</span></span>|<span data-ttu-id="a3883-p105">要检索的区域的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="a3883-p105">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="a3883-137">响应</span><span class="sxs-lookup"><span data-stu-id="a3883-137">Response</span></span>

<span data-ttu-id="a3883-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3883-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3883-139">示例</span><span class="sxs-lookup"><span data-stu-id="a3883-139">Example</span></span>
<span data-ttu-id="a3883-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a3883-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a3883-141">请求</span><span class="sxs-lookup"><span data-stu-id="a3883-141">Request</span></span>
<span data-ttu-id="a3883-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3883-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a3883-143">响应</span><span class="sxs-lookup"><span data-stu-id="a3883-143">Response</span></span>
<span data-ttu-id="a3883-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a3883-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
