---
title: 获取 ChartAxisTitle
description: 检索 chartaxistitle 对象的属性和关系。
author: lumine2008
ms.openlocfilehash: 8cee75a04aeadda2917690ec24104f8747ee89a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344084"
---
# <a name="get-chartaxistitle"></a><span data-ttu-id="52b8b-103">获取 ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="52b8b-103">Get ChartAxisTitle</span></span>

<span data-ttu-id="52b8b-104">检索 chartaxistitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="52b8b-104">Retrieve the properties and relationships of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="52b8b-105">权限</span><span class="sxs-lookup"><span data-stu-id="52b8b-105">Permissions</span></span>
<span data-ttu-id="52b8b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52b8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52b8b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="52b8b-108">Permission type</span></span>      | <span data-ttu-id="52b8b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="52b8b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52b8b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52b8b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="52b8b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52b8b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52b8b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52b8b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52b8b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="52b8b-113">Not supported.</span></span>    |
|<span data-ttu-id="52b8b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="52b8b-114">Application</span></span> | <span data-ttu-id="52b8b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="52b8b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52b8b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52b8b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52b8b-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="52b8b-117">Optional query parameters</span></span>
<span data-ttu-id="52b8b-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="52b8b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52b8b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="52b8b-119">Request headers</span></span>
| <span data-ttu-id="52b8b-120">Name</span><span class="sxs-lookup"><span data-stu-id="52b8b-120">Name</span></span>      |<span data-ttu-id="52b8b-121">说明</span><span class="sxs-lookup"><span data-stu-id="52b8b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52b8b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52b8b-122">Authorization</span></span>  | <span data-ttu-id="52b8b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="52b8b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52b8b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="52b8b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="52b8b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="52b8b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52b8b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="52b8b-128">Request body</span></span>
<span data-ttu-id="52b8b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="52b8b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52b8b-130">响应</span><span class="sxs-lookup"><span data-stu-id="52b8b-130">Response</span></span>

<span data-ttu-id="52b8b-131">如果成功，此方法返回`200 OK`响应代码和[WorkbookChartAxisTitle](../resources/chartaxistitle.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="52b8b-131">If successful, this method returns a `200 OK` response code and [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52b8b-132">示例</span><span class="sxs-lookup"><span data-stu-id="52b8b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52b8b-133">请求</span><span class="sxs-lookup"><span data-stu-id="52b8b-133">Request</span></span>
<span data-ttu-id="52b8b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="52b8b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartaxistitle"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
```
##### <a name="response"></a><span data-ttu-id="52b8b-135">响应</span><span class="sxs-lookup"><span data-stu-id="52b8b-135">Response</span></span>
<span data-ttu-id="52b8b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="52b8b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartAxisTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->