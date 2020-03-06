---
title: 列出 ChartPointsCollection
description: 检索 chartpoint 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1ddb663656ea9b332ec13968d4667fff02ee8f87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518383"
---
# <a name="list-chartpointscollection"></a><span data-ttu-id="b5184-103">列出 ChartPointsCollection</span><span class="sxs-lookup"><span data-stu-id="b5184-103">List ChartPointsCollection</span></span>

<span data-ttu-id="b5184-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5184-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5184-105">检索 chartpoint 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b5184-105">Retrieve a list of chartpoint objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5184-106">权限</span><span class="sxs-lookup"><span data-stu-id="b5184-106">Permissions</span></span>
<span data-ttu-id="b5184-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5184-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5184-109">Permission type</span></span>      | <span data-ttu-id="b5184-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5184-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5184-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5184-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b5184-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5184-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b5184-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5184-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5184-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5184-114">Not supported.</span></span>    |
|<span data-ttu-id="b5184-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5184-115">Application</span></span> | <span data-ttu-id="b5184-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5184-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5184-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5184-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b5184-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b5184-118">Optional query parameters</span></span>
<span data-ttu-id="b5184-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b5184-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5184-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5184-120">Request headers</span></span>
| <span data-ttu-id="b5184-121">名称</span><span class="sxs-lookup"><span data-stu-id="b5184-121">Name</span></span>      |<span data-ttu-id="b5184-122">说明</span><span class="sxs-lookup"><span data-stu-id="b5184-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5184-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5184-123">Authorization</span></span>  | <span data-ttu-id="b5184-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5184-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5184-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b5184-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="b5184-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="b5184-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5184-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5184-129">Request body</span></span>
<span data-ttu-id="b5184-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5184-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5184-131">响应</span><span class="sxs-lookup"><span data-stu-id="b5184-131">Response</span></span>

<span data-ttu-id="b5184-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[WorkbookChartPoint](../resources/chartpoint.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b5184-132">If successful, this method returns a `200 OK` response code and collection of [WorkbookChartPoint](../resources/chartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5184-133">示例</span><span class="sxs-lookup"><span data-stu-id="b5184-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5184-134">请求</span><span class="sxs-lookup"><span data-stu-id="b5184-134">Request</span></span>
<span data-ttu-id="b5184-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5184-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5184-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5184-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartpointscollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
```
# <a name="c"></a>[<span data-ttu-id="b5184-137">C#</span><span class="sxs-lookup"><span data-stu-id="b5184-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartpointscollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5184-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5184-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartpointscollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5184-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5184-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartpointscollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5184-140">Java</span><span class="sxs-lookup"><span data-stu-id="b5184-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartpointscollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b5184-141">响应</span><span class="sxs-lookup"><span data-stu-id="b5184-141">Response</span></span>
<span data-ttu-id="b5184-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5184-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 57

{
  "value": [
    {
      "value": {
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ChartPointsCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
