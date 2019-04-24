---
title: 列出点
description: 检索 chartpoints 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 435e7cbd53653c925740bdcbf823a6f91009b3a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456087"
---
# <a name="list-points"></a><span data-ttu-id="7595f-103">列出点</span><span class="sxs-lookup"><span data-stu-id="7595f-103">List points</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7595f-104">检索 chartpoints 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7595f-104">Retrieve a list of chartpoints objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7595f-105">权限</span><span class="sxs-lookup"><span data-stu-id="7595f-105">Permissions</span></span>
<span data-ttu-id="7595f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7595f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7595f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7595f-108">Permission type</span></span>      | <span data-ttu-id="7595f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7595f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7595f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7595f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7595f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7595f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7595f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7595f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7595f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7595f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7595f-114">Application</span><span class="sxs-lookup"><span data-stu-id="7595f-114">Application</span></span> | <span data-ttu-id="7595f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7595f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7595f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7595f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7595f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7595f-117">Optional query parameters</span></span>
<span data-ttu-id="7595f-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7595f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7595f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7595f-119">Request headers</span></span>
| <span data-ttu-id="7595f-120">名称</span><span class="sxs-lookup"><span data-stu-id="7595f-120">Name</span></span>      |<span data-ttu-id="7595f-121">说明</span><span class="sxs-lookup"><span data-stu-id="7595f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7595f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7595f-122">Authorization</span></span>  | <span data-ttu-id="7595f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7595f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7595f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7595f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7595f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7595f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7595f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7595f-128">Request body</span></span>
<span data-ttu-id="7595f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7595f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7595f-130">响应</span><span class="sxs-lookup"><span data-stu-id="7595f-130">Response</span></span>

<span data-ttu-id="7595f-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ChartPoints](../resources/chartpoint.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7595f-131">If successful, this method returns a `200 OK` response code and collection of [ChartPoints](../resources/chartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7595f-132">示例</span><span class="sxs-lookup"><span data-stu-id="7595f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7595f-133">请求</span><span class="sxs-lookup"><span data-stu-id="7595f-133">Request</span></span>
<span data-ttu-id="7595f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7595f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_points"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
##### <a name="response"></a><span data-ttu-id="7595f-135">响应</span><span class="sxs-lookup"><span data-stu-id="7595f-135">Response</span></span>
<span data-ttu-id="7595f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7595f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 32

{
  "value": [
    {
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List points",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartseries-list-points.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
