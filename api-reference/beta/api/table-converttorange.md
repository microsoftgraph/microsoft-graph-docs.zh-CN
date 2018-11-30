---
title: 'Table: convertToRange'
description: 将表转换为普通单元格区域。保留所有数据。
ms.openlocfilehash: fa91a62bebe3d59a2408999a42d06efd480a0fdc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047003"
---
# <a name="table-converttorange"></a><span data-ttu-id="7290f-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="7290f-104">Table: convertToRange</span></span>

> <span data-ttu-id="7290f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7290f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7290f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7290f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7290f-p103">将表转换为普通单元格区域。保留所有数据。</span><span class="sxs-lookup"><span data-stu-id="7290f-p103">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="7290f-109">权限</span><span class="sxs-lookup"><span data-stu-id="7290f-109">Permissions</span></span>
<span data-ttu-id="7290f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7290f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7290f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7290f-112">Permission type</span></span>      | <span data-ttu-id="7290f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7290f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7290f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7290f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7290f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7290f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7290f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7290f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7290f-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7290f-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7290f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7290f-118">Application</span></span> | <span data-ttu-id="7290f-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7290f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7290f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7290f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="7290f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7290f-121">Request headers</span></span>
| <span data-ttu-id="7290f-122">名称</span><span class="sxs-lookup"><span data-stu-id="7290f-122">Name</span></span>       | <span data-ttu-id="7290f-123">说明</span><span class="sxs-lookup"><span data-stu-id="7290f-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7290f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7290f-124">Authorization</span></span>  | <span data-ttu-id="7290f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7290f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7290f-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7290f-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="7290f-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7290f-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7290f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7290f-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7290f-131">响应</span><span class="sxs-lookup"><span data-stu-id="7290f-131">Response</span></span>

<span data-ttu-id="7290f-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7290f-132">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7290f-133">示例</span><span class="sxs-lookup"><span data-stu-id="7290f-133">Example</span></span>
<span data-ttu-id="7290f-134">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7290f-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7290f-135">请求</span><span class="sxs-lookup"><span data-stu-id="7290f-135">Request</span></span>
<span data-ttu-id="7290f-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7290f-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="7290f-137">响应</span><span class="sxs-lookup"><span data-stu-id="7290f-137">Response</span></span>
<span data-ttu-id="7290f-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7290f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->