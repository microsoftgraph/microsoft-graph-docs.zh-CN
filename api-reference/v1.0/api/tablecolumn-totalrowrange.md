---
title: 'TableColumn: TotalRowRange'
description: 获取与列的总计行相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 76fd4de67c3346f0891c11b28a08cee430a0adbe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889619"
---
# <a name="tablecolumn-totalrowrange"></a><span data-ttu-id="1270f-103">TableColumn: TotalRowRange</span><span class="sxs-lookup"><span data-stu-id="1270f-103">TableColumn: TotalRowRange</span></span>

<span data-ttu-id="1270f-104">获取与列的总计行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="1270f-104">Gets the range object associated with the totals row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="1270f-105">权限</span><span class="sxs-lookup"><span data-stu-id="1270f-105">Permissions</span></span>
<span data-ttu-id="1270f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1270f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1270f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1270f-108">Permission type</span></span>      | <span data-ttu-id="1270f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1270f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1270f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1270f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1270f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1270f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1270f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1270f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1270f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1270f-113">Not supported.</span></span>    |
|<span data-ttu-id="1270f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1270f-114">Application</span></span> | <span data-ttu-id="1270f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1270f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1270f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1270f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/totalRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/totalRowRange

```
## <a name="request-headers"></a><span data-ttu-id="1270f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1270f-117">Request headers</span></span>
| <span data-ttu-id="1270f-118">名称</span><span class="sxs-lookup"><span data-stu-id="1270f-118">Name</span></span>       | <span data-ttu-id="1270f-119">说明</span><span class="sxs-lookup"><span data-stu-id="1270f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1270f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1270f-120">Authorization</span></span>  | <span data-ttu-id="1270f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1270f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1270f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1270f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1270f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1270f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1270f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1270f-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1270f-127">响应</span><span class="sxs-lookup"><span data-stu-id="1270f-127">Response</span></span>

<span data-ttu-id="1270f-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1270f-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1270f-129">示例</span><span class="sxs-lookup"><span data-stu-id="1270f-129">Example</span></span>
<span data-ttu-id="1270f-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1270f-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1270f-131">请求</span><span class="sxs-lookup"><span data-stu-id="1270f-131">Request</span></span>
<span data-ttu-id="1270f-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1270f-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_totalrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/totalRowRange
```

##### <a name="response"></a><span data-ttu-id="1270f-133">响应</span><span class="sxs-lookup"><span data-stu-id="1270f-133">Response</span></span>
<span data-ttu-id="1270f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1270f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: TotalRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
