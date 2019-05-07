---
title: 列出列
description: 检索 tablecolumn 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ca7f39dbf86a981f01397a743edf034b6065dea2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637876"
---
# <a name="list-columns"></a><span data-ttu-id="5c2c7-103">列出列</span><span class="sxs-lookup"><span data-stu-id="5c2c7-103">List columns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c2c7-104">检索 tablecolumn 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-104">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c2c7-105">权限</span><span class="sxs-lookup"><span data-stu-id="5c2c7-105">Permissions</span></span>
<span data-ttu-id="5c2c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c2c7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c2c7-108">Permission type</span></span>      | <span data-ttu-id="5c2c7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c2c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c2c7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c2c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c2c7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c2c7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c2c7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c2c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c2c7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c2c7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c2c7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c2c7-114">Application</span></span> | <span data-ttu-id="5c2c7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c2c7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c2c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5c2c7-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5c2c7-117">Optional query parameters</span></span>
<span data-ttu-id="5c2c7-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="5c2c7-119">为了获得可靠结果，请使用 [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) 和 [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) 查询参数逐个浏览结果。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="5c2c7-120">这有助于避免较大的结果集带来的性能问题。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c2c7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c2c7-121">Request headers</span></span>
| <span data-ttu-id="5c2c7-122">名称</span><span class="sxs-lookup"><span data-stu-id="5c2c7-122">Name</span></span>      |<span data-ttu-id="5c2c7-123">说明</span><span class="sxs-lookup"><span data-stu-id="5c2c7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5c2c7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c2c7-124">Authorization</span></span>  | <span data-ttu-id="5c2c7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c2c7-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5c2c7-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="5c2c7-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c2c7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c2c7-130">Request body</span></span>
<span data-ttu-id="5c2c7-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c2c7-132">响应</span><span class="sxs-lookup"><span data-stu-id="5c2c7-132">Response</span></span>

<span data-ttu-id="5c2c7-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[workbookTableColumn](../resources/workbooktablecolumn.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-133">If successful, this method returns a `200 OK` response code and collection of [workbookTableColumn](../resources/workbooktablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c2c7-134">示例</span><span class="sxs-lookup"><span data-stu-id="5c2c7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c2c7-135">请求</span><span class="sxs-lookup"><span data-stu-id="5c2c7-135">Request</span></span>
<span data-ttu-id="5c2c7-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="5c2c7-137">响应</span><span class="sxs-lookup"><span data-stu-id="5c2c7-137">Response</span></span>
<span data-ttu-id="5c2c7-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5c2c7-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5c2c7-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5c2c7-142">语言</span><span class="sxs-lookup"><span data-stu-id="5c2c7-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_columns-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c2c7-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="5c2c7-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_columns-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

> <span data-ttu-id="5c2c7-144">
  \**注意：\** 使用 [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) 和 [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) 查询参数可逐个浏览许多列。</span><span class="sxs-lookup"><span data-stu-id="5c2c7-144">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="5c2c7-145">示例：</span><span class="sxs-lookup"><span data-stu-id="5c2c7-145">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-list-columns.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/table-list-columns.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
