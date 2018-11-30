---
title: 获取 ChartLegend
description: 检索 chartlegend 对象的属性和关系。
ms.openlocfilehash: 2a98ad13b93900c516921c246f18f6f4f370e574
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008958"
---
# <a name="get-chartlegend"></a><span data-ttu-id="d7ccf-103">获取 ChartLegend</span><span class="sxs-lookup"><span data-stu-id="d7ccf-103">Get ChartLegend</span></span>

<span data-ttu-id="d7ccf-104">检索 chartlegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d7ccf-104">Retrieve the properties and relationships of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7ccf-105">权限</span><span class="sxs-lookup"><span data-stu-id="d7ccf-105">Permissions</span></span>
<span data-ttu-id="d7ccf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7ccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7ccf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7ccf-108">Permission type</span></span>      | <span data-ttu-id="d7ccf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7ccf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7ccf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7ccf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7ccf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7ccf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7ccf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7ccf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7ccf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7ccf-113">Not supported.</span></span>    |
|<span data-ttu-id="d7ccf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7ccf-114">Application</span></span> | <span data-ttu-id="d7ccf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7ccf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7ccf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7ccf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7ccf-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d7ccf-117">Optional query parameters</span></span>
<span data-ttu-id="d7ccf-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d7ccf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7ccf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7ccf-119">Request headers</span></span>
| <span data-ttu-id="d7ccf-120">名称</span><span class="sxs-lookup"><span data-stu-id="d7ccf-120">Name</span></span>      |<span data-ttu-id="d7ccf-121">说明</span><span class="sxs-lookup"><span data-stu-id="d7ccf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d7ccf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7ccf-122">Authorization</span></span>  | <span data-ttu-id="d7ccf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7ccf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7ccf-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d7ccf-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d7ccf-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d7ccf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7ccf-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7ccf-128">Request body</span></span>
<span data-ttu-id="d7ccf-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d7ccf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7ccf-130">响应</span><span class="sxs-lookup"><span data-stu-id="d7ccf-130">Response</span></span>

<span data-ttu-id="d7ccf-131">如果成功，此方法返回`200 OK`响应代码和[WorkbookChartLegend](../resources/chartlegend.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="d7ccf-131">If successful, this method returns a `200 OK` response code and [WorkbookChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7ccf-132">示例</span><span class="sxs-lookup"><span data-stu-id="d7ccf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7ccf-133">请求</span><span class="sxs-lookup"><span data-stu-id="d7ccf-133">Request</span></span>
<span data-ttu-id="d7ccf-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7ccf-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartlegend"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
```
##### <a name="response"></a><span data-ttu-id="d7ccf-135">响应</span><span class="sxs-lookup"><span data-stu-id="d7ccf-135">Response</span></span>
<span data-ttu-id="d7ccf-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d7ccf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->