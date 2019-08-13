---
title: 获取 RangeFormat
description: 检索 rangeformat 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: edcec162c3dfd728426cfaee5def0248c8ecd64f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308776"
---
# <a name="get-rangeformat"></a><span data-ttu-id="8903e-103">获取 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="8903e-103">Get RangeFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8903e-104">检索 rangeformat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8903e-104">Retrieve the properties and relationships of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8903e-105">权限</span><span class="sxs-lookup"><span data-stu-id="8903e-105">Permissions</span></span>
<span data-ttu-id="8903e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8903e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8903e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8903e-108">Permission type</span></span>      | <span data-ttu-id="8903e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8903e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8903e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8903e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8903e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8903e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8903e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8903e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8903e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8903e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8903e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8903e-114">Application</span></span> | <span data-ttu-id="8903e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8903e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8903e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8903e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format
GET /workbook/worksheets/{id|name}/range(address='<address>')/format
GET /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8903e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8903e-117">Optional query parameters</span></span>
<span data-ttu-id="8903e-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8903e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8903e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8903e-119">Request headers</span></span>
| <span data-ttu-id="8903e-120">名称</span><span class="sxs-lookup"><span data-stu-id="8903e-120">Name</span></span>      |<span data-ttu-id="8903e-121">说明</span><span class="sxs-lookup"><span data-stu-id="8903e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8903e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8903e-122">Authorization</span></span>  | <span data-ttu-id="8903e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8903e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8903e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8903e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8903e-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8903e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8903e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8903e-128">Request body</span></span>
<span data-ttu-id="8903e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8903e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8903e-130">响应</span><span class="sxs-lookup"><span data-stu-id="8903e-130">Response</span></span>

<span data-ttu-id="8903e-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[workbookRangeFormat](../resources/workbookrangeformat.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8903e-131">If successful, this method returns a `200 OK` response code and [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8903e-132">示例</span><span class="sxs-lookup"><span data-stu-id="8903e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8903e-133">请求</span><span class="sxs-lookup"><span data-stu-id="8903e-133">Request</span></span>
<span data-ttu-id="8903e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8903e-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8903e-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8903e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rangeformat"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8903e-136">C#</span><span class="sxs-lookup"><span data-stu-id="8903e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8903e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8903e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8903e-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="8903e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8903e-139">Java</span><span class="sxs-lookup"><span data-stu-id="8903e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8903e-140">响应</span><span class="sxs-lookup"><span data-stu-id="8903e-140">Response</span></span>
<span data-ttu-id="8903e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8903e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get RangeFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
