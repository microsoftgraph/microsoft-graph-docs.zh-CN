---
title: 列出 ChartPointsCollection
description: 检索 chartpoint 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 47007c0cb6f128fad9b4e376fff2e065d5b37d8d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463661"
---
# <a name="list-chartpointscollection"></a><span data-ttu-id="53ee4-103">列出 ChartPointsCollection</span><span class="sxs-lookup"><span data-stu-id="53ee4-103">List ChartPointsCollection</span></span>

<span data-ttu-id="53ee4-104">检索 chartpoint 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="53ee4-104">Retrieve a list of chartpoint objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="53ee4-105">权限</span><span class="sxs-lookup"><span data-stu-id="53ee4-105">Permissions</span></span>
<span data-ttu-id="53ee4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53ee4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53ee4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="53ee4-108">Permission type</span></span>      | <span data-ttu-id="53ee4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53ee4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53ee4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53ee4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53ee4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53ee4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53ee4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53ee4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53ee4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="53ee4-113">Not supported.</span></span>    |
|<span data-ttu-id="53ee4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="53ee4-114">Application</span></span> | <span data-ttu-id="53ee4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53ee4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53ee4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53ee4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53ee4-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53ee4-117">Optional query parameters</span></span>
<span data-ttu-id="53ee4-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="53ee4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53ee4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="53ee4-119">Request headers</span></span>
| <span data-ttu-id="53ee4-120">名称</span><span class="sxs-lookup"><span data-stu-id="53ee4-120">Name</span></span>      |<span data-ttu-id="53ee4-121">说明</span><span class="sxs-lookup"><span data-stu-id="53ee4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="53ee4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53ee4-122">Authorization</span></span>  | <span data-ttu-id="53ee4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53ee4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53ee4-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="53ee4-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="53ee4-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="53ee4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53ee4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="53ee4-128">Request body</span></span>
<span data-ttu-id="53ee4-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53ee4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53ee4-130">响应</span><span class="sxs-lookup"><span data-stu-id="53ee4-130">Response</span></span>

<span data-ttu-id="53ee4-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[WorkbookChartPoint](../resources/chartpoint.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="53ee4-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookChartPoint](../resources/chartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53ee4-132">示例</span><span class="sxs-lookup"><span data-stu-id="53ee4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53ee4-133">请求</span><span class="sxs-lookup"><span data-stu-id="53ee4-133">Request</span></span>
<span data-ttu-id="53ee4-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53ee4-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartpointscollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
```
##### <a name="response"></a><span data-ttu-id="53ee4-135">响应</span><span class="sxs-lookup"><span data-stu-id="53ee4-135">Response</span></span>
<span data-ttu-id="53ee4-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53ee4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
