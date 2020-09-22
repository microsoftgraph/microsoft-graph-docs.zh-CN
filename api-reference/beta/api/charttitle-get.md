---
title: 获取 ChartTitle
description: 检索 charttitle 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c5f464e23103aee0228adf20d2cfeeadd1ae800c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982743"
---
# <a name="get-charttitle"></a><span data-ttu-id="91083-103">获取 ChartTitle</span><span class="sxs-lookup"><span data-stu-id="91083-103">Get ChartTitle</span></span>

<span data-ttu-id="91083-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91083-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91083-105">检索 charttitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="91083-105">Retrieve the properties and relationships of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="91083-106">权限</span><span class="sxs-lookup"><span data-stu-id="91083-106">Permissions</span></span>
<span data-ttu-id="91083-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91083-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91083-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="91083-109">Permission type</span></span>      | <span data-ttu-id="91083-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91083-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91083-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91083-111">Delegated (work or school account)</span></span> | <span data-ttu-id="91083-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91083-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="91083-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91083-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91083-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91083-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="91083-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="91083-115">Application</span></span> | <span data-ttu-id="91083-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="91083-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91083-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91083-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91083-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="91083-118">Optional query parameters</span></span>
<span data-ttu-id="91083-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="91083-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91083-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="91083-120">Request headers</span></span>
| <span data-ttu-id="91083-121">名称</span><span class="sxs-lookup"><span data-stu-id="91083-121">Name</span></span>      |<span data-ttu-id="91083-122">说明</span><span class="sxs-lookup"><span data-stu-id="91083-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91083-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91083-123">Authorization</span></span>  | <span data-ttu-id="91083-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91083-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91083-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="91083-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="91083-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="91083-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91083-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="91083-129">Request body</span></span>
<span data-ttu-id="91083-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="91083-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91083-131">响应</span><span class="sxs-lookup"><span data-stu-id="91083-131">Response</span></span>

<span data-ttu-id="91083-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [workbookChartTitle](../resources/workbookcharttitle.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="91083-132">If successful, this method returns a `200 OK` response code and [workbookChartTitle](../resources/workbookcharttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91083-133">示例</span><span class="sxs-lookup"><span data-stu-id="91083-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91083-134">请求</span><span class="sxs-lookup"><span data-stu-id="91083-134">Request</span></span>
<span data-ttu-id="91083-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91083-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91083-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="91083-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_charttitle"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
```
# <a name="c"></a>[<span data-ttu-id="91083-137">C#</span><span class="sxs-lookup"><span data-stu-id="91083-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-charttitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91083-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91083-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-charttitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91083-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91083-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-charttitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91083-140">响应</span><span class="sxs-lookup"><span data-stu-id="91083-140">Response</span></span>
<span data-ttu-id="91083-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="91083-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


