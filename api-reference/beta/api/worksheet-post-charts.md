---
title: 创建图表
description: 使用此 API 创建新图表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 27bd441e6002d69cf94f79b8e3de40f9614ad6a6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544034"
---
# <a name="create-chart"></a><span data-ttu-id="be276-103">创建图表</span><span class="sxs-lookup"><span data-stu-id="be276-103">Create Chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be276-104">使用此 API 创建新图表。</span><span class="sxs-lookup"><span data-stu-id="be276-104">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="be276-105">权限</span><span class="sxs-lookup"><span data-stu-id="be276-105">Permissions</span></span>
<span data-ttu-id="be276-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be276-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="be276-108">Permission type</span></span>      | <span data-ttu-id="be276-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be276-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be276-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be276-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be276-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be276-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be276-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be276-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be276-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be276-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be276-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="be276-114">Application</span></span> | <span data-ttu-id="be276-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="be276-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be276-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be276-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="be276-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="be276-117">Request headers</span></span>
| <span data-ttu-id="be276-118">名称</span><span class="sxs-lookup"><span data-stu-id="be276-118">Name</span></span>       | <span data-ttu-id="be276-119">说明</span><span class="sxs-lookup"><span data-stu-id="be276-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="be276-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="be276-120">Authorization</span></span>  | <span data-ttu-id="be276-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be276-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be276-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="be276-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="be276-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="be276-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be276-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="be276-126">Request body</span></span>
<span data-ttu-id="be276-127">在请求正文中，提供 [Chart](../resources/chart.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be276-127">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="be276-128">响应</span><span class="sxs-lookup"><span data-stu-id="be276-128">Response</span></span>

<span data-ttu-id="be276-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Chart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be276-129">If successful, this method returns `201 Created` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be276-130">示例</span><span class="sxs-lookup"><span data-stu-id="be276-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be276-131">请求</span><span class="sxs-lookup"><span data-stu-id="be276-131">Request</span></span>
<span data-ttu-id="be276-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be276-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="be276-133">在请求正文中，提供 [Chart](../resources/chart.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be276-133">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="be276-134">响应</span><span class="sxs-lookup"><span data-stu-id="be276-134">Response</span></span>
<span data-ttu-id="be276-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be276-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-post-charts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
