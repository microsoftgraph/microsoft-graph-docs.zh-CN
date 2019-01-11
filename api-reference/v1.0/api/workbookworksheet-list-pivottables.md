---
title: List pivotTables
description: 检索 workbookpivottable 对象的列表。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6de7870f0fe16582e463ac1ff833ad282460888e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886014"
---
# <a name="list-pivottables"></a><span data-ttu-id="71af9-103">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="71af9-103">List pivotTables</span></span>

<span data-ttu-id="71af9-104">检索 workbookpivottable 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="71af9-104">Retrieve a list of workbookpivottable objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="71af9-105">权限</span><span class="sxs-lookup"><span data-stu-id="71af9-105">Permissions</span></span>
<span data-ttu-id="71af9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71af9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="71af9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="71af9-108">Permission type</span></span>      | <span data-ttu-id="71af9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71af9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71af9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71af9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71af9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71af9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71af9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71af9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71af9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="71af9-113">Not supported.</span></span>    |
|<span data-ttu-id="71af9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="71af9-114">Application</span></span> | <span data-ttu-id="71af9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="71af9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71af9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71af9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71af9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="71af9-117">Optional query parameters</span></span>
<span data-ttu-id="71af9-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="71af9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71af9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="71af9-119">Request headers</span></span>
| <span data-ttu-id="71af9-120">名称</span><span class="sxs-lookup"><span data-stu-id="71af9-120">Name</span></span>      |<span data-ttu-id="71af9-121">说明</span><span class="sxs-lookup"><span data-stu-id="71af9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71af9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71af9-122">Authorization</span></span>  | <span data-ttu-id="71af9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71af9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71af9-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="71af9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="71af9-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="71af9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71af9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="71af9-128">Request body</span></span>
<span data-ttu-id="71af9-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71af9-129">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="71af9-130">响应</span><span class="sxs-lookup"><span data-stu-id="71af9-130">Response</span></span>
<span data-ttu-id="71af9-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和一组 [workbookPivotTableworkbookPivotTable](../resources/workbookpivottable.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71af9-131">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/workbookpivottable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71af9-132">示例</span><span class="sxs-lookup"><span data-stu-id="71af9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71af9-133">请求</span><span class="sxs-lookup"><span data-stu-id="71af9-133">Request</span></span>
<span data-ttu-id="71af9-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71af9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_pivottables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables
```
##### <a name="response"></a><span data-ttu-id="71af9-135">响应</span><span class="sxs-lookup"><span data-stu-id="71af9-135">Response</span></span>
<span data-ttu-id="71af9-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71af9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
