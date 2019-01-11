---
title: 列出 TableRowCollection
description: 检索 tablerow 对象的列表。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: afb37ed31fbcca19b5f54979a5221bd3d4272016
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815937"
---
# <a name="list-tablerowcollection"></a><span data-ttu-id="cdcdd-103">列出 TableRowCollection</span><span class="sxs-lookup"><span data-stu-id="cdcdd-103">List TableRowCollection</span></span>

<span data-ttu-id="cdcdd-104">检索 tablerow 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="cdcdd-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="cdcdd-105">权限</span><span class="sxs-lookup"><span data-stu-id="cdcdd-105">Permissions</span></span>
<span data-ttu-id="cdcdd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdcdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdcdd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdcdd-108">Permission type</span></span>      | <span data-ttu-id="cdcdd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdcdd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdcdd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdcdd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cdcdd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdcdd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cdcdd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdcdd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdcdd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdcdd-113">Not supported.</span></span>    |
|<span data-ttu-id="cdcdd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdcdd-114">Application</span></span> | <span data-ttu-id="cdcdd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdcdd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdcdd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdcdd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cdcdd-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cdcdd-117">Optional query parameters</span></span>
<span data-ttu-id="cdcdd-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cdcdd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdcdd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdcdd-119">Request headers</span></span>
| <span data-ttu-id="cdcdd-120">名称</span><span class="sxs-lookup"><span data-stu-id="cdcdd-120">Name</span></span>      |<span data-ttu-id="cdcdd-121">说明</span><span class="sxs-lookup"><span data-stu-id="cdcdd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cdcdd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdcdd-122">Authorization</span></span>  | <span data-ttu-id="cdcdd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cdcdd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cdcdd-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cdcdd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="cdcdd-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="cdcdd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdcdd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdcdd-128">Request body</span></span>
<span data-ttu-id="cdcdd-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cdcdd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdcdd-130">响应</span><span class="sxs-lookup"><span data-stu-id="cdcdd-130">Response</span></span>

<span data-ttu-id="cdcdd-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[WorkbookTableRow](../resources/tablerow.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="cdcdd-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cdcdd-132">示例</span><span class="sxs-lookup"><span data-stu-id="cdcdd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdcdd-133">请求</span><span class="sxs-lookup"><span data-stu-id="cdcdd-133">Request</span></span>
<span data-ttu-id="cdcdd-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cdcdd-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablerowcollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows
```
##### <a name="response"></a><span data-ttu-id="cdcdd-135">响应</span><span class="sxs-lookup"><span data-stu-id="cdcdd-135">Response</span></span>
<span data-ttu-id="cdcdd-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cdcdd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 82

{
  "value": [
    {
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableRowCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
