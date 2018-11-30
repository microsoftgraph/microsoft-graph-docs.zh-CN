---
title: 创建 ChartSeries
description: 使用此 API 创建新 ChartSeries。
ms.openlocfilehash: fba694735f254d90fb00e0b8f3658cae3cdccf11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009086"
---
# <a name="create-chartseries"></a><span data-ttu-id="f2f6d-103">创建 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="f2f6d-103">Create ChartSeries</span></span>

<span data-ttu-id="f2f6d-104">使用此 API 创建新 ChartSeries。</span><span class="sxs-lookup"><span data-stu-id="f2f6d-104">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2f6d-105">权限</span><span class="sxs-lookup"><span data-stu-id="f2f6d-105">Permissions</span></span>
<span data-ttu-id="f2f6d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2f6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2f6d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2f6d-108">Permission type</span></span>      | <span data-ttu-id="f2f6d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2f6d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2f6d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2f6d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f2f6d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2f6d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f2f6d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2f6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2f6d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2f6d-113">Not supported.</span></span>    |
|<span data-ttu-id="f2f6d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2f6d-114">Application</span></span> | <span data-ttu-id="f2f6d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2f6d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2f6d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2f6d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="f2f6d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2f6d-117">Request headers</span></span>
| <span data-ttu-id="f2f6d-118">名称</span><span class="sxs-lookup"><span data-stu-id="f2f6d-118">Name</span></span>       | <span data-ttu-id="f2f6d-119">说明</span><span class="sxs-lookup"><span data-stu-id="f2f6d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f2f6d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2f6d-120">Authorization</span></span>  | <span data-ttu-id="f2f6d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2f6d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2f6d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f2f6d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f2f6d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f2f6d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2f6d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2f6d-126">Request body</span></span>
<span data-ttu-id="f2f6d-127">在请求正文中，提供[WorkbookChartSeries](../resources/chartseries.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2f6d-127">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f2f6d-128">响应</span><span class="sxs-lookup"><span data-stu-id="f2f6d-128">Response</span></span>

<span data-ttu-id="f2f6d-129">如果成功，此方法返回`201 Created`响应代码和[WorkbookChartSeries](../resources/chartseries.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="f2f6d-129">If successful, this method returns `201 Created` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2f6d-130">示例</span><span class="sxs-lookup"><span data-stu-id="f2f6d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2f6d-131">请求</span><span class="sxs-lookup"><span data-stu-id="f2f6d-131">Request</span></span>
<span data-ttu-id="f2f6d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2f6d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="f2f6d-133">在请求正文中，提供[WorkbookChartSeries](../resources/chartseries.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2f6d-133">In the request body, supply a JSON representation of [WorkbookChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f2f6d-134">响应</span><span class="sxs-lookup"><span data-stu-id="f2f6d-134">Response</span></span>
<span data-ttu-id="f2f6d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2f6d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->