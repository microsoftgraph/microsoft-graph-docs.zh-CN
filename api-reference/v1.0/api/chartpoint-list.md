---
title: 列出 ChartPointsCollection
description: 检索 chartpoint 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 47007c0cb6f128fad9b4e376fff2e065d5b37d8d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990815"
---
# <a name="list-chartpointscollection"></a><span data-ttu-id="490d9-103">列出 ChartPointsCollection</span><span class="sxs-lookup"><span data-stu-id="490d9-103">List ChartPointsCollection</span></span>

<span data-ttu-id="490d9-104">检索 chartpoint 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="490d9-104">Retrieve a list of chartpoint objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="490d9-105">权限</span><span class="sxs-lookup"><span data-stu-id="490d9-105">Permissions</span></span>
<span data-ttu-id="490d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="490d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="490d9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="490d9-108">Permission type</span></span>      | <span data-ttu-id="490d9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="490d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="490d9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="490d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="490d9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="490d9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="490d9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="490d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="490d9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="490d9-113">Not supported.</span></span>    |
|<span data-ttu-id="490d9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="490d9-114">Application</span></span> | <span data-ttu-id="490d9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="490d9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="490d9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="490d9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="490d9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="490d9-117">Optional query parameters</span></span>
<span data-ttu-id="490d9-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="490d9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="490d9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="490d9-119">Request headers</span></span>
| <span data-ttu-id="490d9-120">名称</span><span class="sxs-lookup"><span data-stu-id="490d9-120">Name</span></span>      |<span data-ttu-id="490d9-121">说明</span><span class="sxs-lookup"><span data-stu-id="490d9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="490d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="490d9-122">Authorization</span></span>  | <span data-ttu-id="490d9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="490d9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="490d9-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="490d9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="490d9-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="490d9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="490d9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="490d9-128">Request body</span></span>
<span data-ttu-id="490d9-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="490d9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="490d9-130">响应</span><span class="sxs-lookup"><span data-stu-id="490d9-130">Response</span></span>

<span data-ttu-id="490d9-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[WorkbookChartPoint](../resources/chartpoint.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="490d9-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookChartPoint](../resources/chartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="490d9-132">示例</span><span class="sxs-lookup"><span data-stu-id="490d9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="490d9-133">请求</span><span class="sxs-lookup"><span data-stu-id="490d9-133">Request</span></span>
<span data-ttu-id="490d9-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="490d9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartpointscollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
```
##### <a name="response"></a><span data-ttu-id="490d9-135">响应</span><span class="sxs-lookup"><span data-stu-id="490d9-135">Response</span></span>
<span data-ttu-id="490d9-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="490d9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
