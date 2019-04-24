---
title: 列出表集合
description: 检索 table 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 056abfc392a5d3b16407f6125b6bd752e21305e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520625"
---
# <a name="list-tablecollection"></a><span data-ttu-id="31016-103">列出表集合</span><span class="sxs-lookup"><span data-stu-id="31016-103">List TableCollection</span></span>

<span data-ttu-id="31016-104">检索 table 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="31016-104">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="31016-105">权限</span><span class="sxs-lookup"><span data-stu-id="31016-105">Permissions</span></span>
<span data-ttu-id="31016-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31016-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31016-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="31016-108">Permission type</span></span>      | <span data-ttu-id="31016-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31016-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31016-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31016-110">Delegated (work or school account)</span></span> | <span data-ttu-id="31016-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31016-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="31016-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31016-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31016-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="31016-113">Not supported.</span></span>    |
|<span data-ttu-id="31016-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="31016-114">Application</span></span> | <span data-ttu-id="31016-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="31016-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31016-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31016-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables
GET /workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="31016-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31016-117">Optional query parameters</span></span>
<span data-ttu-id="31016-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31016-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31016-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="31016-119">Request headers</span></span>
| <span data-ttu-id="31016-120">名称</span><span class="sxs-lookup"><span data-stu-id="31016-120">Name</span></span>      |<span data-ttu-id="31016-121">说明</span><span class="sxs-lookup"><span data-stu-id="31016-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31016-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31016-122">Authorization</span></span>  | <span data-ttu-id="31016-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31016-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="31016-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="31016-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="31016-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="31016-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31016-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="31016-128">Request body</span></span>
<span data-ttu-id="31016-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31016-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31016-130">响应</span><span class="sxs-lookup"><span data-stu-id="31016-130">Response</span></span>

<span data-ttu-id="31016-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[WorkbookTable](../resources/table.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="31016-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookTable](../resources/table.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31016-132">示例</span><span class="sxs-lookup"><span data-stu-id="31016-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31016-133">请求</span><span class="sxs-lookup"><span data-stu-id="31016-133">Request</span></span>
<span data-ttu-id="31016-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31016-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables
```
##### <a name="response"></a><span data-ttu-id="31016-135">响应</span><span class="sxs-lookup"><span data-stu-id="31016-135">Response</span></span>
<span data-ttu-id="31016-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31016-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "id": "99",
      "name": "name-value",
      "showHeaders": true,
      "showTotals": true,
      "style": "style-value"
    }
  ]
}
```
> <span data-ttu-id="31016-139">**注意：** 使用 [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) 和 [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) 查询参数可逐个浏览许多表。</span><span class="sxs-lookup"><span data-stu-id="31016-139">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) query parameters to page through large numbers of tables.</span></span>

<span data-ttu-id="31016-140">示例：</span><span class="sxs-lookup"><span data-stu-id="31016-140">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
