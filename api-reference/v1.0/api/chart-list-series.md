---
title: 列出系列
description: 检索 chartseries 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b1de872cb02a63c72cd3287a37a81ffc4a70ec4c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443628"
---
# <a name="list-series"></a><span data-ttu-id="01562-103">列出系列</span><span class="sxs-lookup"><span data-stu-id="01562-103">List series</span></span>

<span data-ttu-id="01562-104">检索 chartseries 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="01562-104">Retrieve a list of chartseries objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="01562-105">权限</span><span class="sxs-lookup"><span data-stu-id="01562-105">Permissions</span></span>
<span data-ttu-id="01562-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01562-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01562-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="01562-108">Permission type</span></span>      | <span data-ttu-id="01562-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01562-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01562-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01562-110">Delegated (work or school account)</span></span> | <span data-ttu-id="01562-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01562-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01562-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01562-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01562-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="01562-113">Not supported.</span></span>    |
|<span data-ttu-id="01562-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="01562-114">Application</span></span> | <span data-ttu-id="01562-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01562-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01562-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01562-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01562-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="01562-117">Optional query parameters</span></span>
<span data-ttu-id="01562-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="01562-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01562-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="01562-119">Request headers</span></span>
| <span data-ttu-id="01562-120">名称</span><span class="sxs-lookup"><span data-stu-id="01562-120">Name</span></span>      |<span data-ttu-id="01562-121">说明</span><span class="sxs-lookup"><span data-stu-id="01562-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="01562-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01562-122">Authorization</span></span>  | <span data-ttu-id="01562-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01562-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01562-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="01562-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="01562-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="01562-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01562-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="01562-128">Request body</span></span>
<span data-ttu-id="01562-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01562-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01562-130">响应</span><span class="sxs-lookup"><span data-stu-id="01562-130">Response</span></span>

<span data-ttu-id="01562-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[WorkbookChartSeries](../resources/chartseries.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="01562-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookChartSeries](../resources/chartseries.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01562-132">示例</span><span class="sxs-lookup"><span data-stu-id="01562-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01562-133">请求</span><span class="sxs-lookup"><span data-stu-id="01562-133">Request</span></span>
<span data-ttu-id="01562-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01562-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="01562-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="01562-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_series"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="01562-136">C#</span><span class="sxs-lookup"><span data-stu-id="01562-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-series-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01562-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="01562-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-series-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="01562-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="01562-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-series-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="01562-139">响应</span><span class="sxs-lookup"><span data-stu-id="01562-139">Response</span></span>
<span data-ttu-id="01562-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01562-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 59

{
  "value": [
    {
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List series",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
