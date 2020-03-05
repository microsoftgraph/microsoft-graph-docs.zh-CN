---
title: 列出行
description: 检索 tablerow 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 82e2ba96758749eedbab9d2419e34bf0e88b99dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452821"
---
# <a name="list-rows"></a><span data-ttu-id="ec574-103">列出行</span><span class="sxs-lookup"><span data-stu-id="ec574-103">List rows</span></span>

<span data-ttu-id="ec574-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ec574-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec574-105">检索 tablerow 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ec574-105">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec574-106">权限</span><span class="sxs-lookup"><span data-stu-id="ec574-106">Permissions</span></span>
<span data-ttu-id="ec574-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec574-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec574-109">Permission type</span></span>      | <span data-ttu-id="ec574-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec574-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec574-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec574-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ec574-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec574-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec574-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec574-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec574-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec574-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec574-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec574-115">Application</span></span> | <span data-ttu-id="ec574-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec574-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec574-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec574-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec574-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ec574-118">Optional query parameters</span></span>
<span data-ttu-id="ec574-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ec574-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="ec574-120">为了获得可靠结果，请使用 [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) 和 [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) 查询参数逐个浏览结果。</span><span class="sxs-lookup"><span data-stu-id="ec574-120">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="ec574-121">这有助于避免较大的结果集带来的性能问题。</span><span class="sxs-lookup"><span data-stu-id="ec574-121">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec574-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec574-122">Request headers</span></span>
| <span data-ttu-id="ec574-123">名称</span><span class="sxs-lookup"><span data-stu-id="ec574-123">Name</span></span>      |<span data-ttu-id="ec574-124">说明</span><span class="sxs-lookup"><span data-stu-id="ec574-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec574-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec574-125">Authorization</span></span>  | <span data-ttu-id="ec574-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec574-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec574-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ec574-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="ec574-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ec574-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec574-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec574-131">Request body</span></span>
<span data-ttu-id="ec574-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec574-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec574-133">响应</span><span class="sxs-lookup"><span data-stu-id="ec574-133">Response</span></span>

<span data-ttu-id="ec574-134">如果成功，此方法在响应`200 OK`正文中返回响应代码和[workbookTableRow](../resources/workbooktablerow.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ec574-134">If successful, this method returns a `200 OK` response code and collection of [workbookTableRow](../resources/workbooktablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec574-135">示例</span><span class="sxs-lookup"><span data-stu-id="ec574-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec574-136">请求</span><span class="sxs-lookup"><span data-stu-id="ec574-136">Request</span></span>
<span data-ttu-id="ec574-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec574-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec574-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec574-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_table_rows"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
# <a name="c"></a>[<span data-ttu-id="ec574-139">C#</span><span class="sxs-lookup"><span data-stu-id="ec574-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-table-rows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec574-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec574-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-table-rows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec574-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec574-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-table-rows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ec574-142">响应</span><span class="sxs-lookup"><span data-stu-id="ec574-142">Response</span></span>
<span data-ttu-id="ec574-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec574-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

> <span data-ttu-id="ec574-146">
  \**注意：\** 使用 [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) 和 [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) 查询参数可逐个浏览许多行。</span><span class="sxs-lookup"><span data-stu-id="ec574-146">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="ec574-147">示例：</span><span class="sxs-lookup"><span data-stu-id="ec574-147">Example:</span></span> 

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
  ]
}
-->
