---
title: 列出行
description: 检索 tablerow 对象的列表。
author: lumine2008
ms.openlocfilehash: d3ae25face1d2ca43d240c60621c390b7bf67da5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360114"
---
# <a name="list-rows"></a><span data-ttu-id="22faa-103">列出行</span><span class="sxs-lookup"><span data-stu-id="22faa-103">List rows</span></span>

> <span data-ttu-id="22faa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="22faa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22faa-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="22faa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22faa-106">检索 tablerow 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="22faa-106">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="22faa-107">权限</span><span class="sxs-lookup"><span data-stu-id="22faa-107">Permissions</span></span>
<span data-ttu-id="22faa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22faa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22faa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="22faa-110">Permission type</span></span>      | <span data-ttu-id="22faa-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22faa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22faa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22faa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="22faa-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22faa-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="22faa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22faa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22faa-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22faa-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="22faa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="22faa-116">Application</span></span> | <span data-ttu-id="22faa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="22faa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22faa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22faa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="22faa-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="22faa-119">Optional query parameters</span></span>
<span data-ttu-id="22faa-120">此方法支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 自定义响应。</span><span class="sxs-lookup"><span data-stu-id="22faa-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="22faa-121">为了获得可靠结果，请使用 [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) 和 [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) 查询参数逐个浏览结果。</span><span class="sxs-lookup"><span data-stu-id="22faa-121">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="22faa-122">这有助于避免较大的结果集带来的性能问题。</span><span class="sxs-lookup"><span data-stu-id="22faa-122">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22faa-123">请求头</span><span class="sxs-lookup"><span data-stu-id="22faa-123">Request headers</span></span>
| <span data-ttu-id="22faa-124">Name</span><span class="sxs-lookup"><span data-stu-id="22faa-124">Name</span></span>      |<span data-ttu-id="22faa-125">说明</span><span class="sxs-lookup"><span data-stu-id="22faa-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="22faa-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="22faa-126">Authorization</span></span>  | <span data-ttu-id="22faa-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22faa-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="22faa-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="22faa-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="22faa-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="22faa-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22faa-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="22faa-132">Request body</span></span>
<span data-ttu-id="22faa-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22faa-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22faa-134">响应</span><span class="sxs-lookup"><span data-stu-id="22faa-134">Response</span></span>

<span data-ttu-id="22faa-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableRow](../resources/tablerow.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="22faa-135">If successful, this method returns a `200 OK` response code and collection of [TableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="22faa-136">示例</span><span class="sxs-lookup"><span data-stu-id="22faa-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22faa-137">请求</span><span class="sxs-lookup"><span data-stu-id="22faa-137">Request</span></span>
<span data-ttu-id="22faa-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="22faa-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="22faa-139">响应</span><span class="sxs-lookup"><span data-stu-id="22faa-139">Response</span></span>
<span data-ttu-id="22faa-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22faa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow",
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

> <span data-ttu-id="22faa-143">
  \**注意：\** 使用 [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) 和 [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) 查询参数可逐个浏览许多行。</span><span class="sxs-lookup"><span data-stu-id="22faa-143">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="22faa-144">示例：</span><span class="sxs-lookup"><span data-stu-id="22faa-144">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->