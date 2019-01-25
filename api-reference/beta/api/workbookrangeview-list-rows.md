---
title: List rangeView rows
description: 检索范围视图对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9d0d3cb5f29f9588481b5e87c7a20cc96e3850e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522999"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="eb341-103">List rangeView rows</span><span class="sxs-lookup"><span data-stu-id="eb341-103">List rangeView rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb341-104">检索范围视图对象的列表。</span><span class="sxs-lookup"><span data-stu-id="eb341-104">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb341-105">权限</span><span class="sxs-lookup"><span data-stu-id="eb341-105">Permissions</span></span>
<span data-ttu-id="eb341-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb341-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb341-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb341-108">Permission type</span></span>      | <span data-ttu-id="eb341-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb341-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb341-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb341-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eb341-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb341-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eb341-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb341-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb341-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb341-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eb341-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb341-114">Application</span></span> | <span data-ttu-id="eb341-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb341-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb341-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb341-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="eb341-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eb341-117">Optional query parameters</span></span>
<span data-ttu-id="eb341-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eb341-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb341-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb341-119">Request headers</span></span>
| <span data-ttu-id="eb341-120">名称</span><span class="sxs-lookup"><span data-stu-id="eb341-120">Name</span></span>      |<span data-ttu-id="eb341-121">说明</span><span class="sxs-lookup"><span data-stu-id="eb341-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb341-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb341-122">Authorization</span></span>  | <span data-ttu-id="eb341-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb341-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb341-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eb341-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="eb341-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="eb341-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb341-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb341-128">Request body</span></span>
<span data-ttu-id="eb341-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb341-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb341-130">响应</span><span class="sxs-lookup"><span data-stu-id="eb341-130">Response</span></span>

<span data-ttu-id="eb341-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和一组 [workbookRangeView](../resources/workbookrangeview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb341-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eb341-132">示例</span><span class="sxs-lookup"><span data-stu-id="eb341-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb341-133">请求</span><span class="sxs-lookup"><span data-stu-id="eb341-133">Request</span></span>
<span data-ttu-id="eb341-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb341-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/rows 
```
##### <a name="response"></a><span data-ttu-id="eb341-135">响应</span><span class="sxs-lookup"><span data-stu-id="eb341-135">Response</span></span>
<span data-ttu-id="eb341-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb341-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 247

{
  "value": [
    {
      "cellAddresses": "cellAddresses-value",
      "columnCount": 99,
      "formulas": "formulas-value",
      "formulasLocal": "formulasLocal-value",
      "formulasR1C1": "formulasR1C1-value",
      "index": 99
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrangeview-list-rows.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
