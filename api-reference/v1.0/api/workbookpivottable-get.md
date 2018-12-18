---
title: Get workbookPivotTable
description: 检索 workbookPivotTable 对象的属性和关系。
author: lumine2008
ms.openlocfilehash: f4d42f05fe5e9908aa9f2d60c88533a6608850a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347955"
---
# <a name="get-workbookpivottable"></a><span data-ttu-id="e276d-103">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="e276d-103">Get workbookPivotTable</span></span>

<span data-ttu-id="e276d-104">检索 workbookPivotTable 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e276d-104">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e276d-105">权限</span><span class="sxs-lookup"><span data-stu-id="e276d-105">Permissions</span></span>
<span data-ttu-id="e276d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e276d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e276d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e276d-108">Permission type</span></span>      | <span data-ttu-id="e276d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e276d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e276d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e276d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e276d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e276d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e276d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e276d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e276d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e276d-113">Not supported.</span></span>    |
|<span data-ttu-id="e276d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e276d-114">Application</span></span> | <span data-ttu-id="e276d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e276d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e276d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e276d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e276d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e276d-117">Optional query parameters</span></span>
<span data-ttu-id="e276d-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e276d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e276d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e276d-119">Request headers</span></span>
| <span data-ttu-id="e276d-120">Name</span><span class="sxs-lookup"><span data-stu-id="e276d-120">Name</span></span>      |<span data-ttu-id="e276d-121">说明</span><span class="sxs-lookup"><span data-stu-id="e276d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e276d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e276d-122">Authorization</span></span>  | <span data-ttu-id="e276d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e276d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e276d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e276d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e276d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e276d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e276d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e276d-128">Request body</span></span>
<span data-ttu-id="e276d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e276d-129">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="e276d-130">响应</span><span class="sxs-lookup"><span data-stu-id="e276d-130">Response</span></span>
<span data-ttu-id="e276d-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookPivotTable](../resources/workbookpivottable.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e276d-131">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e276d-132">示例</span><span class="sxs-lookup"><span data-stu-id="e276d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e276d-133">请求</span><span class="sxs-lookup"><span data-stu-id="e276d-133">Request</span></span>
<span data-ttu-id="e276d-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e276d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a><span data-ttu-id="e276d-135">响应</span><span class="sxs-lookup"><span data-stu-id="e276d-135">Response</span></span>
<span data-ttu-id="e276d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e276d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```
