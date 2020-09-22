---
title: 获取范围
description: 检索 range 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0558934420c6398e3fcc135dd9359983e97a195a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055807"
---
# <a name="get-range"></a><span data-ttu-id="dbf38-103">获取区域</span><span class="sxs-lookup"><span data-stu-id="dbf38-103">Get Range</span></span>

<span data-ttu-id="dbf38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbf38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbf38-105">检索 range 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dbf38-105">Retrieve the properties and relationships of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dbf38-106">权限</span><span class="sxs-lookup"><span data-stu-id="dbf38-106">Permissions</span></span>
<span data-ttu-id="dbf38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbf38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbf38-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbf38-109">Permission type</span></span>      | <span data-ttu-id="dbf38-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dbf38-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbf38-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbf38-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dbf38-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbf38-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dbf38-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbf38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbf38-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbf38-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dbf38-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbf38-115">Application</span></span> | <span data-ttu-id="dbf38-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbf38-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbf38-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbf38-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range(address='<address>')
GET /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dbf38-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dbf38-118">Optional query parameters</span></span>
<span data-ttu-id="dbf38-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dbf38-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbf38-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbf38-120">Request headers</span></span>
| <span data-ttu-id="dbf38-121">名称</span><span class="sxs-lookup"><span data-stu-id="dbf38-121">Name</span></span>      |<span data-ttu-id="dbf38-122">说明</span><span class="sxs-lookup"><span data-stu-id="dbf38-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dbf38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbf38-123">Authorization</span></span>  | <span data-ttu-id="dbf38-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dbf38-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dbf38-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dbf38-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="dbf38-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="dbf38-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbf38-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbf38-129">Request body</span></span>
<span data-ttu-id="dbf38-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dbf38-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbf38-131">响应</span><span class="sxs-lookup"><span data-stu-id="dbf38-131">Response</span></span>

<span data-ttu-id="dbf38-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dbf38-132">If successful, this method returns a `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dbf38-133">示例</span><span class="sxs-lookup"><span data-stu-id="dbf38-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dbf38-134">请求</span><span class="sxs-lookup"><span data-stu-id="dbf38-134">Request</span></span>
<span data-ttu-id="dbf38-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dbf38-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dbf38-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbf38-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range
```
# <a name="c"></a>[<span data-ttu-id="dbf38-137">C#</span><span class="sxs-lookup"><span data-stu-id="dbf38-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbf38-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbf38-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbf38-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbf38-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dbf38-140">响应</span><span class="sxs-lookup"><span data-stu-id="dbf38-140">Response</span></span>
<span data-ttu-id="dbf38-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dbf38-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


