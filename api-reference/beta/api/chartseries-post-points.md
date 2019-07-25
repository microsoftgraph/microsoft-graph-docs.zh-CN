---
title: 创建 ChartPoints
description: 使用此 API 创建新 ChartPoints。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9f04161d1e8c440ca69e528e7039ac004451e47d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863785"
---
# <a name="create-chartpoint"></a><span data-ttu-id="cd4c0-103">创建 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="cd4c0-103">Create ChartPoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd4c0-104">使用此 API 创建新的 ChartPoint。</span><span class="sxs-lookup"><span data-stu-id="cd4c0-104">Use this API to create a new ChartPoint.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd4c0-105">权限</span><span class="sxs-lookup"><span data-stu-id="cd4c0-105">Permissions</span></span>
<span data-ttu-id="cd4c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd4c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd4c0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd4c0-108">Permission type</span></span>      | <span data-ttu-id="cd4c0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd4c0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd4c0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd4c0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd4c0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd4c0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cd4c0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd4c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd4c0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd4c0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cd4c0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd4c0-114">Application</span></span> | <span data-ttu-id="cd4c0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd4c0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd4c0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd4c0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points

```
## <a name="request-headers"></a><span data-ttu-id="cd4c0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd4c0-117">Request headers</span></span>
| <span data-ttu-id="cd4c0-118">名称</span><span class="sxs-lookup"><span data-stu-id="cd4c0-118">Name</span></span>       | <span data-ttu-id="cd4c0-119">说明</span><span class="sxs-lookup"><span data-stu-id="cd4c0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cd4c0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd4c0-120">Authorization</span></span>  | <span data-ttu-id="cd4c0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd4c0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd4c0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cd4c0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cd4c0-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="cd4c0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd4c0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd4c0-126">Request body</span></span>
<span data-ttu-id="cd4c0-127">在请求正文中, 提供[workbookChartPoint](../resources/workbookchartpoint.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd4c0-127">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cd4c0-128">响应</span><span class="sxs-lookup"><span data-stu-id="cd4c0-128">Response</span></span>

<span data-ttu-id="cd4c0-129">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[workbookChartPoint](../resources/workbookchartpoint.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cd4c0-129">If successful, this method returns `201 Created` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd4c0-130">示例</span><span class="sxs-lookup"><span data-stu-id="cd4c0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd4c0-131">请求</span><span class="sxs-lookup"><span data-stu-id="cd4c0-131">Request</span></span>
<span data-ttu-id="cd4c0-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd4c0-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cd4c0-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="cd4c0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
Content-type: application/json
Content-length: 3

{
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cd4c0-134">C#</span><span class="sxs-lookup"><span data-stu-id="cd4c0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartpoints-from-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cd4c0-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="cd4c0-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartpoints-from-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cd4c0-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="cd4c0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartpoints-from-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cd4c0-137">Java</span><span class="sxs-lookup"><span data-stu-id="cd4c0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chartpoints-from-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="cd4c0-138">在请求正文中, 提供[workbookChartPoint](../resources/workbookchartpoint.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd4c0-138">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cd4c0-139">响应</span><span class="sxs-lookup"><span data-stu-id="cd4c0-139">Response</span></span>
<span data-ttu-id="cd4c0-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd4c0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
