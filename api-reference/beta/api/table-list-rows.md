---
title: 列出行
description: 检索 tablerow 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 11d0db96bb338eaa6c8c66571064cbe4f6b4f8f2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271097"
---
# <a name="list-rows"></a><span data-ttu-id="1e07f-103">列出行</span><span class="sxs-lookup"><span data-stu-id="1e07f-103">List rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e07f-104">检索 tablerow 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1e07f-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e07f-105">权限</span><span class="sxs-lookup"><span data-stu-id="1e07f-105">Permissions</span></span>
<span data-ttu-id="1e07f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e07f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e07f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e07f-108">Permission type</span></span>      | <span data-ttu-id="1e07f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e07f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e07f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e07f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e07f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e07f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e07f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e07f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e07f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e07f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e07f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e07f-114">Application</span></span> | <span data-ttu-id="1e07f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e07f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e07f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e07f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1e07f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1e07f-117">Optional query parameters</span></span>
<span data-ttu-id="1e07f-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1e07f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="1e07f-119">为了获得可靠结果，请使用 [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) 和 [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) 查询参数逐个浏览结果。</span><span class="sxs-lookup"><span data-stu-id="1e07f-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="1e07f-120">这有助于避免较大的结果集带来的性能问题。</span><span class="sxs-lookup"><span data-stu-id="1e07f-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e07f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e07f-121">Request headers</span></span>
| <span data-ttu-id="1e07f-122">名称</span><span class="sxs-lookup"><span data-stu-id="1e07f-122">Name</span></span>      |<span data-ttu-id="1e07f-123">说明</span><span class="sxs-lookup"><span data-stu-id="1e07f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1e07f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e07f-124">Authorization</span></span>  | <span data-ttu-id="1e07f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e07f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e07f-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1e07f-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="1e07f-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1e07f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e07f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e07f-130">Request body</span></span>
<span data-ttu-id="1e07f-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e07f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e07f-132">响应</span><span class="sxs-lookup"><span data-stu-id="1e07f-132">Response</span></span>

<span data-ttu-id="1e07f-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[workbookTableRow](../resources/workbooktablerow.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="1e07f-133">If successful, this method returns a `200 OK` response code and collection of [workbookTableRow](../resources/workbooktablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e07f-134">示例</span><span class="sxs-lookup"><span data-stu-id="1e07f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e07f-135">请求</span><span class="sxs-lookup"><span data-stu-id="1e07f-135">Request</span></span>
<span data-ttu-id="1e07f-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e07f-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="1e07f-137">响应</span><span class="sxs-lookup"><span data-stu-id="1e07f-137">Response</span></span>
<span data-ttu-id="1e07f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e07f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1e07f-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1e07f-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1e07f-142">C#</span><span class="sxs-lookup"><span data-stu-id="1e07f-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_rows-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e07f-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="1e07f-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_rows-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1e07f-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="1e07f-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_rows-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

> <span data-ttu-id="1e07f-145">
  \**注意：\** 使用 [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) 和 [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) 查询参数可逐个浏览许多行。</span><span class="sxs-lookup"><span data-stu-id="1e07f-145">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="1e07f-146">示例：</span><span class="sxs-lookup"><span data-stu-id="1e07f-146">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-list-rows.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/table-list-rows.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/table-list-rows.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
