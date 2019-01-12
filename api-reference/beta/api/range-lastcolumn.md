---
title: Range:LastColumn
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d15b3611c7449da8ca03623f59e5cbb4f9c2e98a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942981"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="d7782-103">Range:LastColumn</span><span class="sxs-lookup"><span data-stu-id="d7782-103">Range: LastColumn</span></span>

> <span data-ttu-id="d7782-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d7782-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7782-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d7782-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7782-p102">获取区域内的最后一列。例如，“B2:D5”的最后一列是“D2:D5”。</span><span class="sxs-lookup"><span data-stu-id="d7782-p102">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="d7782-108">权限</span><span class="sxs-lookup"><span data-stu-id="d7782-108">Permissions</span></span>
<span data-ttu-id="d7782-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7782-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7782-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7782-111">Permission type</span></span>      | <span data-ttu-id="d7782-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7782-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7782-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7782-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d7782-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7782-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7782-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7782-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7782-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7782-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7782-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7782-117">Application</span></span> | <span data-ttu-id="d7782-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7782-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7782-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7782-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastColumn

```
## <a name="request-headers"></a><span data-ttu-id="d7782-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7782-120">Request headers</span></span>
| <span data-ttu-id="d7782-121">名称</span><span class="sxs-lookup"><span data-stu-id="d7782-121">Name</span></span>       | <span data-ttu-id="d7782-122">说明</span><span class="sxs-lookup"><span data-stu-id="d7782-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7782-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7782-123">Authorization</span></span>  | <span data-ttu-id="d7782-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7782-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7782-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d7782-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="d7782-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d7782-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7782-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7782-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d7782-130">响应</span><span class="sxs-lookup"><span data-stu-id="d7782-130">Response</span></span>

<span data-ttu-id="d7782-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d7782-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7782-132">示例</span><span class="sxs-lookup"><span data-stu-id="d7782-132">Example</span></span>
<span data-ttu-id="d7782-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d7782-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7782-134">请求</span><span class="sxs-lookup"><span data-stu-id="d7782-134">Request</span></span>
<span data-ttu-id="d7782-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7782-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastColumn
```

##### <a name="response"></a><span data-ttu-id="d7782-136">响应</span><span class="sxs-lookup"><span data-stu-id="d7782-136">Response</span></span>
<span data-ttu-id="d7782-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d7782-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
