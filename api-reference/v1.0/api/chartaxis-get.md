---
title: 获取 ChartAxis
description: 检索 chartaxis 对象的属性和关系。
ms.openlocfilehash: 9738c49d768f45ae1ce134d36b227995f1b2df4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007920"
---
# <a name="get-chartaxis"></a><span data-ttu-id="9cb3d-103">获取 ChartAxis</span><span class="sxs-lookup"><span data-stu-id="9cb3d-103">Get ChartAxis</span></span>

<span data-ttu-id="9cb3d-104">检索 chartaxis 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9cb3d-104">Retrieve the properties and relationships of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9cb3d-105">权限</span><span class="sxs-lookup"><span data-stu-id="9cb3d-105">Permissions</span></span>
<span data-ttu-id="9cb3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cb3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cb3d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cb3d-108">Permission type</span></span>      | <span data-ttu-id="9cb3d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cb3d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cb3d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cb3d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9cb3d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cb3d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9cb3d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cb3d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cb3d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cb3d-113">Not supported.</span></span>    |
|<span data-ttu-id="9cb3d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cb3d-114">Application</span></span> | <span data-ttu-id="9cb3d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cb3d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cb3d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cb3d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9cb3d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9cb3d-117">Optional query parameters</span></span>
<span data-ttu-id="9cb3d-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9cb3d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cb3d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cb3d-119">Request headers</span></span>
| <span data-ttu-id="9cb3d-120">名称</span><span class="sxs-lookup"><span data-stu-id="9cb3d-120">Name</span></span>      |<span data-ttu-id="9cb3d-121">说明</span><span class="sxs-lookup"><span data-stu-id="9cb3d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9cb3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cb3d-122">Authorization</span></span>  | <span data-ttu-id="9cb3d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cb3d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9cb3d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9cb3d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9cb3d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9cb3d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cb3d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cb3d-128">Request body</span></span>
<span data-ttu-id="9cb3d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cb3d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cb3d-130">响应</span><span class="sxs-lookup"><span data-stu-id="9cb3d-130">Response</span></span>

<span data-ttu-id="9cb3d-131">如果成功，此方法返回`200 OK`响应代码和[WorkbookChartAxis](../resources/chartaxis.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="9cb3d-131">If successful, this method returns a `200 OK` response code and [WorkbookChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9cb3d-132">示例</span><span class="sxs-lookup"><span data-stu-id="9cb3d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cb3d-133">请求</span><span class="sxs-lookup"><span data-stu-id="9cb3d-133">Request</span></span>
<span data-ttu-id="9cb3d-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9cb3d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartaxis"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
```
##### <a name="response"></a><span data-ttu-id="9cb3d-135">响应</span><span class="sxs-lookup"><span data-stu-id="9cb3d-135">Response</span></span>
<span data-ttu-id="9cb3d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9cb3d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartAxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->