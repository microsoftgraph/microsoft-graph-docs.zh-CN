---
title: 'TableColumn: DataBodyRange'
description: 获取与列的数据体相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2ba67e4585b3671a588173772b3f1313198e6a38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969035"
---
# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="facec-103">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="facec-103">TableColumn: DataBodyRange</span></span>

<span data-ttu-id="facec-104">获取与列的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="facec-104">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="facec-105">权限</span><span class="sxs-lookup"><span data-stu-id="facec-105">Permissions</span></span>
<span data-ttu-id="facec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="facec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="facec-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="facec-108">Permission type</span></span>      | <span data-ttu-id="facec-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="facec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="facec-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="facec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="facec-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="facec-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="facec-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="facec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="facec-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="facec-113">Not supported.</span></span>    |
|<span data-ttu-id="facec-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="facec-114">Application</span></span> | <span data-ttu-id="facec-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="facec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="facec-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="facec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/dataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="facec-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="facec-117">Request headers</span></span>
| <span data-ttu-id="facec-118">名称</span><span class="sxs-lookup"><span data-stu-id="facec-118">Name</span></span>       | <span data-ttu-id="facec-119">说明</span><span class="sxs-lookup"><span data-stu-id="facec-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="facec-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="facec-120">Authorization</span></span>  | <span data-ttu-id="facec-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="facec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="facec-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="facec-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="facec-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="facec-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="facec-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="facec-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="facec-127">响应</span><span class="sxs-lookup"><span data-stu-id="facec-127">Response</span></span>

<span data-ttu-id="facec-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="facec-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="facec-129">示例</span><span class="sxs-lookup"><span data-stu-id="facec-129">Example</span></span>
<span data-ttu-id="facec-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="facec-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="facec-131">请求</span><span class="sxs-lookup"><span data-stu-id="facec-131">Request</span></span>
<span data-ttu-id="facec-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="facec-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_databodyrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
```

##### <a name="response"></a><span data-ttu-id="facec-133">响应</span><span class="sxs-lookup"><span data-stu-id="facec-133">Response</span></span>
<span data-ttu-id="facec-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="facec-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
