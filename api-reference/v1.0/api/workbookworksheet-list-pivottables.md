---
title: List pivotTables
description: 检索 workbookpivottable 对象的列表。
author: lumine2008
ms.openlocfilehash: ccb3904eed6b13f12662474df6763224b8ee1aba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326479"
---
# <a name="list-pivottables"></a><span data-ttu-id="84a12-103">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="84a12-103">List pivotTables</span></span>

<span data-ttu-id="84a12-104">检索 workbookpivottable 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="84a12-104">Retrieve a list of workbookpivottable objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="84a12-105">权限</span><span class="sxs-lookup"><span data-stu-id="84a12-105">Permissions</span></span>
<span data-ttu-id="84a12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84a12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="84a12-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="84a12-108">Permission type</span></span>      | <span data-ttu-id="84a12-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84a12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84a12-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84a12-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84a12-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84a12-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="84a12-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84a12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84a12-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="84a12-113">Not supported.</span></span>    |
|<span data-ttu-id="84a12-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="84a12-114">Application</span></span> | <span data-ttu-id="84a12-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="84a12-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84a12-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84a12-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84a12-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="84a12-117">Optional query parameters</span></span>
<span data-ttu-id="84a12-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="84a12-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84a12-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="84a12-119">Request headers</span></span>
| <span data-ttu-id="84a12-120">Name</span><span class="sxs-lookup"><span data-stu-id="84a12-120">Name</span></span>      |<span data-ttu-id="84a12-121">说明</span><span class="sxs-lookup"><span data-stu-id="84a12-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84a12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84a12-122">Authorization</span></span>  | <span data-ttu-id="84a12-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84a12-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84a12-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="84a12-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="84a12-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="84a12-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84a12-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="84a12-128">Request body</span></span>
<span data-ttu-id="84a12-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84a12-129">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="84a12-130">响应</span><span class="sxs-lookup"><span data-stu-id="84a12-130">Response</span></span>
<span data-ttu-id="84a12-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和一组 [workbookPivotTableworkbookPivotTable](../resources/workbookpivottable.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="84a12-131">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/workbookpivottable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84a12-132">示例</span><span class="sxs-lookup"><span data-stu-id="84a12-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84a12-133">请求</span><span class="sxs-lookup"><span data-stu-id="84a12-133">Request</span></span>
<span data-ttu-id="84a12-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84a12-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_pivottables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables
```
##### <a name="response"></a><span data-ttu-id="84a12-135">响应</span><span class="sxs-lookup"><span data-stu-id="84a12-135">Response</span></span>
<span data-ttu-id="84a12-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84a12-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```
