---
title: Table:DataBodyRange
description: 获取与表的数据体相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: aed58949852ab7f9640e6eec101d002d2ee6bc1a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024558"
---
# <a name="table-databodyrange"></a><span data-ttu-id="ee855-103">Table:DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="ee855-103">Table: DataBodyRange</span></span>

<span data-ttu-id="ee855-104">获取与表的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="ee855-104">Gets the range object associated with the data body of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee855-105">权限</span><span class="sxs-lookup"><span data-stu-id="ee855-105">Permissions</span></span>
<span data-ttu-id="ee855-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee855-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee855-108">Permission type</span></span>      | <span data-ttu-id="ee855-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee855-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee855-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee855-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee855-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee855-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ee855-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee855-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee855-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee855-113">Not supported.</span></span>    |
|<span data-ttu-id="ee855-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee855-114">Application</span></span> | <span data-ttu-id="ee855-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee855-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee855-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee855-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ee855-117">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ee855-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/dataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/dataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="ee855-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee855-118">Request headers</span></span>
| <span data-ttu-id="ee855-119">名称</span><span class="sxs-lookup"><span data-stu-id="ee855-119">Name</span></span>       | <span data-ttu-id="ee855-120">说明</span><span class="sxs-lookup"><span data-stu-id="ee855-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee855-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee855-121">Authorization</span></span>  | <span data-ttu-id="ee855-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee855-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee855-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ee855-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ee855-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ee855-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee855-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee855-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ee855-128">响应</span><span class="sxs-lookup"><span data-stu-id="ee855-128">Response</span></span>

<span data-ttu-id="ee855-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee855-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee855-130">示例</span><span class="sxs-lookup"><span data-stu-id="ee855-130">Example</span></span>
<span data-ttu-id="ee855-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ee855-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ee855-132">请求</span><span class="sxs-lookup"><span data-stu-id="ee855-132">Request</span></span>
<span data-ttu-id="ee855-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ee855-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_databodyrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/dataBodyRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ee855-134">C#</span><span class="sxs-lookup"><span data-stu-id="ee855-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-databodyrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee855-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="ee855-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-databodyrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ee855-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="ee855-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-databodyrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ee855-137">Java</span><span class="sxs-lookup"><span data-stu-id="ee855-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-databodyrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee855-138">响应</span><span class="sxs-lookup"><span data-stu-id="ee855-138">Response</span></span>
<span data-ttu-id="ee855-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ee855-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
