---
title: TableColumn:Range
description: 获取与整个列相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 754fe9b22a20d8a0e082d7f4de7c183c47ed78ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330151"
---
# <a name="tablecolumn-range"></a><span data-ttu-id="d9c70-103">TableColumn:Range</span><span class="sxs-lookup"><span data-stu-id="d9c70-103">TableColumn: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9c70-104">获取与整个列相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="d9c70-104">Gets the range object associated with the entire column.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9c70-105">权限</span><span class="sxs-lookup"><span data-stu-id="d9c70-105">Permissions</span></span>
<span data-ttu-id="d9c70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9c70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9c70-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9c70-108">Permission type</span></span>      | <span data-ttu-id="d9c70-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9c70-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9c70-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9c70-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d9c70-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9c70-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d9c70-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9c70-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9c70-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9c70-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d9c70-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9c70-114">Application</span></span> | <span data-ttu-id="d9c70-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9c70-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9c70-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9c70-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/Range
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="d9c70-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9c70-117">Request headers</span></span>
| <span data-ttu-id="d9c70-118">名称</span><span class="sxs-lookup"><span data-stu-id="d9c70-118">Name</span></span>       | <span data-ttu-id="d9c70-119">说明</span><span class="sxs-lookup"><span data-stu-id="d9c70-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9c70-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9c70-120">Authorization</span></span>  | <span data-ttu-id="d9c70-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d9c70-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9c70-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d9c70-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d9c70-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d9c70-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9c70-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9c70-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d9c70-127">响应</span><span class="sxs-lookup"><span data-stu-id="d9c70-127">Response</span></span>

<span data-ttu-id="d9c70-128">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[workbookRange](../resources/workbookrange.md)) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9c70-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md)) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9c70-129">示例</span><span class="sxs-lookup"><span data-stu-id="d9c70-129">Example</span></span>
<span data-ttu-id="d9c70-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d9c70-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d9c70-131">请求</span><span class="sxs-lookup"><span data-stu-id="d9c70-131">Request</span></span>
<span data-ttu-id="d9c70-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9c70-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/Range
```

##### <a name="response"></a><span data-ttu-id="d9c70-133">响应</span><span class="sxs-lookup"><span data-stu-id="d9c70-133">Response</span></span>
<span data-ttu-id="d9c70-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9c70-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
