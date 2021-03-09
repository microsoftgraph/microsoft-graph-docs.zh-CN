---
title: 'Table: convertToRange'
description: 将表转换为普通单元格区域。保留所有数据。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0f7ea44f7157872f6174c247a6c10d207b153456
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576657"
---
# <a name="table-converttorange"></a><span data-ttu-id="7010e-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="7010e-104">Table: convertToRange</span></span>

<span data-ttu-id="7010e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7010e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7010e-p102">将表转换为普通单元格区域。保留所有数据。</span><span class="sxs-lookup"><span data-stu-id="7010e-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="7010e-108">权限</span><span class="sxs-lookup"><span data-stu-id="7010e-108">Permissions</span></span>
<span data-ttu-id="7010e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7010e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7010e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7010e-111">Permission type</span></span>      | <span data-ttu-id="7010e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7010e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7010e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7010e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7010e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7010e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7010e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7010e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7010e-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7010e-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7010e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7010e-117">Application</span></span> | <span data-ttu-id="7010e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7010e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7010e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7010e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/convertToRange
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/convertToRange
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="7010e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7010e-120">Request headers</span></span>
| <span data-ttu-id="7010e-121">名称</span><span class="sxs-lookup"><span data-stu-id="7010e-121">Name</span></span>       | <span data-ttu-id="7010e-122">说明</span><span class="sxs-lookup"><span data-stu-id="7010e-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7010e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7010e-123">Authorization</span></span>  | <span data-ttu-id="7010e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7010e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7010e-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7010e-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="7010e-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7010e-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7010e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7010e-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7010e-130">响应</span><span class="sxs-lookup"><span data-stu-id="7010e-130">Response</span></span>

<span data-ttu-id="7010e-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7010e-131">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7010e-132">示例</span><span class="sxs-lookup"><span data-stu-id="7010e-132">Example</span></span>
<span data-ttu-id="7010e-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7010e-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7010e-134">请求</span><span class="sxs-lookup"><span data-stu-id="7010e-134">Request</span></span>
<span data-ttu-id="7010e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7010e-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7010e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7010e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```
# <a name="c"></a>[<span data-ttu-id="7010e-137">C#</span><span class="sxs-lookup"><span data-stu-id="7010e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-converttorange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7010e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7010e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-converttorange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7010e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7010e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-converttorange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7010e-140">Java</span><span class="sxs-lookup"><span data-stu-id="7010e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-converttorange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7010e-141">响应</span><span class="sxs-lookup"><span data-stu-id="7010e-141">Response</span></span>
<span data-ttu-id="7010e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7010e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


