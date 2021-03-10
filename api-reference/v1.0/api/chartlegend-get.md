---
title: 获取 ChartLegend
description: 检索 chartlegend 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5e29699395ca138379761682d2cdf6cc24c3fef6
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578057"
---
# <a name="get-chartlegend"></a><span data-ttu-id="2c07b-103">获取 ChartLegend</span><span class="sxs-lookup"><span data-stu-id="2c07b-103">Get ChartLegend</span></span>

<span data-ttu-id="2c07b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c07b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2c07b-105">检索 chartlegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2c07b-105">Retrieve the properties and relationships of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c07b-106">权限</span><span class="sxs-lookup"><span data-stu-id="2c07b-106">Permissions</span></span>
<span data-ttu-id="2c07b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c07b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c07b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c07b-109">Permission type</span></span>      | <span data-ttu-id="2c07b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c07b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c07b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c07b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2c07b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c07b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2c07b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c07b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c07b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c07b-114">Not supported.</span></span>    |
|<span data-ttu-id="2c07b-115">Application</span><span class="sxs-lookup"><span data-stu-id="2c07b-115">Application</span></span> | <span data-ttu-id="2c07b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c07b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c07b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c07b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2c07b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2c07b-118">Optional query parameters</span></span>
<span data-ttu-id="2c07b-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2c07b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c07b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c07b-120">Request headers</span></span>
| <span data-ttu-id="2c07b-121">名称</span><span class="sxs-lookup"><span data-stu-id="2c07b-121">Name</span></span>      |<span data-ttu-id="2c07b-122">说明</span><span class="sxs-lookup"><span data-stu-id="2c07b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2c07b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c07b-123">Authorization</span></span>  | <span data-ttu-id="2c07b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c07b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2c07b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2c07b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="2c07b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2c07b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c07b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c07b-129">Request body</span></span>
<span data-ttu-id="2c07b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c07b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c07b-131">响应</span><span class="sxs-lookup"><span data-stu-id="2c07b-131">Response</span></span>

<span data-ttu-id="2c07b-132">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [WorkbookChartLegend](../resources/chartlegend.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2c07b-132">If successful, this method returns a `200 OK` response code and [WorkbookChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2c07b-133">示例</span><span class="sxs-lookup"><span data-stu-id="2c07b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c07b-134">请求</span><span class="sxs-lookup"><span data-stu-id="2c07b-134">Request</span></span>
<span data-ttu-id="2c07b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c07b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c07b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c07b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartlegend"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
```
# <a name="c"></a>[<span data-ttu-id="2c07b-137">C#</span><span class="sxs-lookup"><span data-stu-id="2c07b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartlegend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c07b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c07b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartlegend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c07b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c07b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartlegend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c07b-140">Java</span><span class="sxs-lookup"><span data-stu-id="2c07b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartlegend-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2c07b-141">响应</span><span class="sxs-lookup"><span data-stu-id="2c07b-141">Response</span></span>
<span data-ttu-id="2c07b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c07b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartLegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
