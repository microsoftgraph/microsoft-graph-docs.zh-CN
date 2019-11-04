---
title: List rangeView rows
description: 检索范围视图对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c4c3b2f6a62427e3d30d9e157ba2deddcefa2a9c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937432"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="b2df5-103">List rangeView rows</span><span class="sxs-lookup"><span data-stu-id="b2df5-103">List rangeView rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2df5-104">检索范围视图对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b2df5-104">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2df5-105">权限</span><span class="sxs-lookup"><span data-stu-id="b2df5-105">Permissions</span></span>
<span data-ttu-id="b2df5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2df5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2df5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2df5-108">Permission type</span></span>      | <span data-ttu-id="b2df5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2df5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2df5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2df5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b2df5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2df5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b2df5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2df5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2df5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2df5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b2df5-114">Application</span><span class="sxs-lookup"><span data-stu-id="b2df5-114">Application</span></span> | <span data-ttu-id="b2df5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2df5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2df5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2df5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="b2df5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b2df5-117">Optional query parameters</span></span>
<span data-ttu-id="b2df5-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b2df5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2df5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2df5-119">Request headers</span></span>
| <span data-ttu-id="b2df5-120">名称</span><span class="sxs-lookup"><span data-stu-id="b2df5-120">Name</span></span>      |<span data-ttu-id="b2df5-121">说明</span><span class="sxs-lookup"><span data-stu-id="b2df5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b2df5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2df5-122">Authorization</span></span>  | <span data-ttu-id="b2df5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2df5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2df5-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b2df5-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b2df5-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="b2df5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2df5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2df5-128">Request body</span></span>
<span data-ttu-id="b2df5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b2df5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2df5-130">响应</span><span class="sxs-lookup"><span data-stu-id="b2df5-130">Response</span></span>

<span data-ttu-id="b2df5-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和一组 [workbookRangeView](../resources/workbookrangeview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2df5-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b2df5-132">示例</span><span class="sxs-lookup"><span data-stu-id="b2df5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2df5-133">请求</span><span class="sxs-lookup"><span data-stu-id="b2df5-133">Request</span></span>
<span data-ttu-id="b2df5-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2df5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows 
```
##### <a name="response"></a><span data-ttu-id="b2df5-135">响应</span><span class="sxs-lookup"><span data-stu-id="b2df5-135">Response</span></span>
<span data-ttu-id="b2df5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2df5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
