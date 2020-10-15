---
title: 列出列
description: 检索 tablecolumn 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9f1d4f44509788dcc00c7d037956862fcd645994
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457301"
---
# <a name="list-columns"></a><span data-ttu-id="e3a11-103">列出列</span><span class="sxs-lookup"><span data-stu-id="e3a11-103">List columns</span></span>

<span data-ttu-id="e3a11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3a11-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3a11-105">检索 tablecolumn 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e3a11-105">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3a11-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e3a11-106">Permissions</span></span>
<span data-ttu-id="e3a11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3a11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3a11-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3a11-109">Permission type</span></span>      | <span data-ttu-id="e3a11-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3a11-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3a11-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3a11-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e3a11-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3a11-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e3a11-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3a11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3a11-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3a11-114">Not supported.</span></span>    |
|<span data-ttu-id="e3a11-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3a11-115">Application</span></span> | <span data-ttu-id="e3a11-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3a11-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3a11-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3a11-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3a11-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e3a11-118">Optional query parameters</span></span>
<span data-ttu-id="e3a11-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e3a11-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>  <span data-ttu-id="e3a11-120">为了获得可靠结果，请使用 [$top](/graph/query-parameters#top) 和 [$skip](/graph/query-parameters#skip-parameter) 查询参数逐个浏览结果。</span><span class="sxs-lookup"><span data-stu-id="e3a11-120">For reliable results, use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="e3a11-121">这有助于避免较大的结果集带来的性能问题。</span><span class="sxs-lookup"><span data-stu-id="e3a11-121">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3a11-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3a11-122">Request headers</span></span>
| <span data-ttu-id="e3a11-123">名称</span><span class="sxs-lookup"><span data-stu-id="e3a11-123">Name</span></span>      |<span data-ttu-id="e3a11-124">说明</span><span class="sxs-lookup"><span data-stu-id="e3a11-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3a11-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3a11-125">Authorization</span></span>  | <span data-ttu-id="e3a11-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3a11-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e3a11-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e3a11-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="e3a11-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e3a11-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3a11-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3a11-131">Request body</span></span>
<span data-ttu-id="e3a11-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e3a11-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3a11-133">响应</span><span class="sxs-lookup"><span data-stu-id="e3a11-133">Response</span></span>

<span data-ttu-id="e3a11-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [WorkbookTableColumn](../resources/workbooktablecolumn.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e3a11-134">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableColumn](../resources/workbooktablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3a11-135">示例</span><span class="sxs-lookup"><span data-stu-id="e3a11-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3a11-136">请求</span><span class="sxs-lookup"><span data-stu-id="e3a11-136">Request</span></span>
<span data-ttu-id="e3a11-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3a11-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3a11-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3a11-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
# <a name="c"></a>[<span data-ttu-id="e3a11-139">C#</span><span class="sxs-lookup"><span data-stu-id="e3a11-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3a11-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3a11-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3a11-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3a11-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3a11-142">Java</span><span class="sxs-lookup"><span data-stu-id="e3a11-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e3a11-143">响应</span><span class="sxs-lookup"><span data-stu-id="e3a11-143">Response</span></span>
<span data-ttu-id="e3a11-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e3a11-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

> <span data-ttu-id="e3a11-147">
  \**注意：\** 使用 [$top](/graph/query-parameters#top) 和 [$skip](/graph/query-parameters#skip-parameter) 查询参数可逐个浏览许多列。</span><span class="sxs-lookup"><span data-stu-id="e3a11-147">**Note:** Use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="e3a11-148">示例：</span><span class="sxs-lookup"><span data-stu-id="e3a11-148">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
