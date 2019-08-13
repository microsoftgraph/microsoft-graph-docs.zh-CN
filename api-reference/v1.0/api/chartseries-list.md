---
title: 列出 ChartSeriesCollection
description: 检索 chartseries 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ea11e5f9fc91cb95dcdd3426a7d4e6b5a615f887
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316414"
---
# <a name="list-chartseriescollection"></a><span data-ttu-id="9eb2a-103">列出 ChartSeriesCollection</span><span class="sxs-lookup"><span data-stu-id="9eb2a-103">List ChartSeriesCollection</span></span>

<span data-ttu-id="9eb2a-104">检索 chartseries 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9eb2a-104">Retrieve a list of chartseries objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9eb2a-105">权限</span><span class="sxs-lookup"><span data-stu-id="9eb2a-105">Permissions</span></span>
<span data-ttu-id="9eb2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9eb2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9eb2a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9eb2a-108">Permission type</span></span>      | <span data-ttu-id="9eb2a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9eb2a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9eb2a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9eb2a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9eb2a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9eb2a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9eb2a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9eb2a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9eb2a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9eb2a-113">Not supported.</span></span>    |
|<span data-ttu-id="9eb2a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9eb2a-114">Application</span></span> | <span data-ttu-id="9eb2a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9eb2a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9eb2a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9eb2a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9eb2a-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9eb2a-117">Optional query parameters</span></span>
<span data-ttu-id="9eb2a-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9eb2a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9eb2a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9eb2a-119">Request headers</span></span>
| <span data-ttu-id="9eb2a-120">名称</span><span class="sxs-lookup"><span data-stu-id="9eb2a-120">Name</span></span>      |<span data-ttu-id="9eb2a-121">说明</span><span class="sxs-lookup"><span data-stu-id="9eb2a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9eb2a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9eb2a-122">Authorization</span></span>  | <span data-ttu-id="9eb2a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9eb2a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9eb2a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9eb2a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9eb2a-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9eb2a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9eb2a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9eb2a-128">Request body</span></span>
<span data-ttu-id="9eb2a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9eb2a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9eb2a-130">响应</span><span class="sxs-lookup"><span data-stu-id="9eb2a-130">Response</span></span>

<span data-ttu-id="9eb2a-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[WorkbookChartSeries](../resources/chartseries.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="9eb2a-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookChartSeries](../resources/chartseries.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9eb2a-132">示例</span><span class="sxs-lookup"><span data-stu-id="9eb2a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9eb2a-133">请求</span><span class="sxs-lookup"><span data-stu-id="9eb2a-133">Request</span></span>
<span data-ttu-id="9eb2a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9eb2a-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9eb2a-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9eb2a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartseriescollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9eb2a-136">C#</span><span class="sxs-lookup"><span data-stu-id="9eb2a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartseriescollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9eb2a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9eb2a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartseriescollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9eb2a-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="9eb2a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartseriescollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9eb2a-139">Java</span><span class="sxs-lookup"><span data-stu-id="9eb2a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartseriescollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9eb2a-140">响应</span><span class="sxs-lookup"><span data-stu-id="9eb2a-140">Response</span></span>
<span data-ttu-id="9eb2a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9eb2a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ChartSeriesCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
