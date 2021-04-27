---
title: Range:Column
description: 获取范围中包含的列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f3e7de29404775b3eb888fe617018503d81fea49
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055132"
---
# <a name="range-column"></a><span data-ttu-id="44ff3-103">Range:Column</span><span class="sxs-lookup"><span data-stu-id="44ff3-103">Range: Column</span></span>

<span data-ttu-id="44ff3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44ff3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44ff3-105">获取范围中包含的列。</span><span class="sxs-lookup"><span data-stu-id="44ff3-105">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="44ff3-106">权限</span><span class="sxs-lookup"><span data-stu-id="44ff3-106">Permissions</span></span>
<span data-ttu-id="44ff3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44ff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44ff3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="44ff3-109">Permission type</span></span>      | <span data-ttu-id="44ff3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44ff3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44ff3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44ff3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="44ff3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44ff3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="44ff3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44ff3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44ff3-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44ff3-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="44ff3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="44ff3-115">Application</span></span> | <span data-ttu-id="44ff3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="44ff3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44ff3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44ff3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/Column
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/Column
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/Column
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/Column
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/Column
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/Column

```
## <a name="request-headers"></a><span data-ttu-id="44ff3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="44ff3-118">Request headers</span></span>
| <span data-ttu-id="44ff3-119">名称</span><span class="sxs-lookup"><span data-stu-id="44ff3-119">Name</span></span>       | <span data-ttu-id="44ff3-120">说明</span><span class="sxs-lookup"><span data-stu-id="44ff3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="44ff3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44ff3-121">Authorization</span></span>  | <span data-ttu-id="44ff3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44ff3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44ff3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="44ff3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="44ff3-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="44ff3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44ff3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="44ff3-127">Request body</span></span>
<span data-ttu-id="44ff3-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="44ff3-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="44ff3-129">参数</span><span class="sxs-lookup"><span data-stu-id="44ff3-129">Parameter</span></span>    | <span data-ttu-id="44ff3-130">类型</span><span class="sxs-lookup"><span data-stu-id="44ff3-130">Type</span></span>   |<span data-ttu-id="44ff3-131">说明</span><span class="sxs-lookup"><span data-stu-id="44ff3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44ff3-132">column</span><span class="sxs-lookup"><span data-stu-id="44ff3-132">column</span></span>|<span data-ttu-id="44ff3-133">number</span><span class="sxs-lookup"><span data-stu-id="44ff3-133">number</span></span>|<span data-ttu-id="44ff3-p104">要检索的区域的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="44ff3-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="44ff3-136">响应</span><span class="sxs-lookup"><span data-stu-id="44ff3-136">Response</span></span>

<span data-ttu-id="44ff3-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44ff3-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44ff3-138">示例</span><span class="sxs-lookup"><span data-stu-id="44ff3-138">Example</span></span>
<span data-ttu-id="44ff3-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="44ff3-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="44ff3-140">请求</span><span class="sxs-lookup"><span data-stu-id="44ff3-140">Request</span></span>
<span data-ttu-id="44ff3-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44ff3-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/Column
Content-type: application/json
Content-length: 21

{
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="44ff3-142">响应</span><span class="sxs-lookup"><span data-stu-id="44ff3-142">Response</span></span>
<span data-ttu-id="44ff3-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="44ff3-143">Here is an example of the response.</span></span> <span data-ttu-id="44ff3-144">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="44ff3-144">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


