---
title: 获取 ChartGridlines
description: 检索 chartgridlines 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 66a487de4100d5d72349d28f3cfa0ce21fd91962
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931767"
---
# <a name="get-chartgridlines"></a><span data-ttu-id="709d1-103">获取 ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="709d1-103">Get ChartGridlines</span></span>

> <span data-ttu-id="709d1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="709d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="709d1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="709d1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="709d1-106">检索 chartgridlines 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="709d1-106">Retrieve the properties and relationships of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="709d1-107">权限</span><span class="sxs-lookup"><span data-stu-id="709d1-107">Permissions</span></span>
<span data-ttu-id="709d1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="709d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="709d1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="709d1-110">Permission type</span></span>      | <span data-ttu-id="709d1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="709d1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="709d1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="709d1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="709d1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="709d1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="709d1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="709d1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="709d1-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="709d1-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="709d1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="709d1-116">Application</span></span> | <span data-ttu-id="709d1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="709d1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="709d1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="709d1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/minorgridlines
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/majorgridlines
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines
```
## <a name="optional-query-parameters"></a><span data-ttu-id="709d1-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="709d1-119">Optional query parameters</span></span>
<span data-ttu-id="709d1-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="709d1-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="709d1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="709d1-121">Request headers</span></span>
| <span data-ttu-id="709d1-122">名称</span><span class="sxs-lookup"><span data-stu-id="709d1-122">Name</span></span>      |<span data-ttu-id="709d1-123">说明</span><span class="sxs-lookup"><span data-stu-id="709d1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="709d1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="709d1-124">Authorization</span></span>  | <span data-ttu-id="709d1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="709d1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="709d1-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="709d1-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="709d1-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="709d1-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="709d1-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="709d1-130">Request body</span></span>
<span data-ttu-id="709d1-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="709d1-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="709d1-132">响应</span><span class="sxs-lookup"><span data-stu-id="709d1-132">Response</span></span>

<span data-ttu-id="709d1-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ChartGridlines](../resources/chartgridlines.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="709d1-133">If successful, this method returns a `200 OK` response code and [ChartGridlines](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="709d1-134">示例</span><span class="sxs-lookup"><span data-stu-id="709d1-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="709d1-135">请求</span><span class="sxs-lookup"><span data-stu-id="709d1-135">Request</span></span>
<span data-ttu-id="709d1-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="709d1-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartgridlines"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/minorgridlines
```
##### <a name="response"></a><span data-ttu-id="709d1-137">响应</span><span class="sxs-lookup"><span data-stu-id="709d1-137">Response</span></span>
<span data-ttu-id="709d1-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="709d1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartGridLines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartGridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
