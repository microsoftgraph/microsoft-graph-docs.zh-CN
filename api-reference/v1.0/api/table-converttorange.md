---
title: 'Table: convertToRange'
description: 将表转换为普通单元格区域。保留所有数据。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4528daab7cfde480e93d75cdcb5f9a969f583144
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825373"
---
# <a name="table-converttorange"></a><span data-ttu-id="98e5d-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="98e5d-104">Table: convertToRange</span></span>

<span data-ttu-id="98e5d-p102">将表转换为普通单元格区域。保留所有数据。</span><span class="sxs-lookup"><span data-stu-id="98e5d-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="98e5d-107">权限</span><span class="sxs-lookup"><span data-stu-id="98e5d-107">Permissions</span></span>
<span data-ttu-id="98e5d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98e5d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98e5d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="98e5d-110">Permission type</span></span>      | <span data-ttu-id="98e5d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98e5d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98e5d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98e5d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="98e5d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98e5d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="98e5d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98e5d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98e5d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="98e5d-115">Not supported.</span></span>    |
|<span data-ttu-id="98e5d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="98e5d-116">Application</span></span> | <span data-ttu-id="98e5d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="98e5d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98e5d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98e5d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="98e5d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="98e5d-119">Request headers</span></span>
| <span data-ttu-id="98e5d-120">名称</span><span class="sxs-lookup"><span data-stu-id="98e5d-120">Name</span></span>       | <span data-ttu-id="98e5d-121">说明</span><span class="sxs-lookup"><span data-stu-id="98e5d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="98e5d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="98e5d-122">Authorization</span></span>  | <span data-ttu-id="98e5d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98e5d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="98e5d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="98e5d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="98e5d-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="98e5d-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98e5d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="98e5d-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="98e5d-129">响应</span><span class="sxs-lookup"><span data-stu-id="98e5d-129">Response</span></span>

<span data-ttu-id="98e5d-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98e5d-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98e5d-131">示例</span><span class="sxs-lookup"><span data-stu-id="98e5d-131">Example</span></span>
<span data-ttu-id="98e5d-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="98e5d-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="98e5d-133">请求</span><span class="sxs-lookup"><span data-stu-id="98e5d-133">Request</span></span>
<span data-ttu-id="98e5d-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="98e5d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="98e5d-135">响应</span><span class="sxs-lookup"><span data-stu-id="98e5d-135">Response</span></span>
<span data-ttu-id="98e5d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="98e5d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
