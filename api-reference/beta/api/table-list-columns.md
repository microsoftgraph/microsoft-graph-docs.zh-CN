---
title: 列出列
description: 检索 tablecolumn 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a4d870a51a6e78981446dec9c94331189607c21d
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313973"
---
# <a name="list-columns"></a><span data-ttu-id="20205-103">列出列</span><span class="sxs-lookup"><span data-stu-id="20205-103">List columns</span></span>

<span data-ttu-id="20205-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20205-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20205-105">检索 tablecolumn 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="20205-105">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="20205-106">权限</span><span class="sxs-lookup"><span data-stu-id="20205-106">Permissions</span></span>
<span data-ttu-id="20205-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20205-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20205-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="20205-109">Permission type</span></span>      | <span data-ttu-id="20205-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20205-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20205-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20205-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20205-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20205-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20205-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20205-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20205-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20205-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20205-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="20205-115">Application</span></span> | <span data-ttu-id="20205-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="20205-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20205-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20205-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20205-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="20205-118">Optional query parameters</span></span>
<span data-ttu-id="20205-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="20205-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="20205-120">为了获得可靠结果，请使用 [$top](/graph/query-parameters#top) 和 [$skip](/graph/query-parameters#skip-parameter) 查询参数逐个浏览结果。</span><span class="sxs-lookup"><span data-stu-id="20205-120">For reliable results, use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="20205-121">这有助于避免较大的结果集带来的性能问题。</span><span class="sxs-lookup"><span data-stu-id="20205-121">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20205-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="20205-122">Request headers</span></span>
| <span data-ttu-id="20205-123">名称</span><span class="sxs-lookup"><span data-stu-id="20205-123">Name</span></span>      |<span data-ttu-id="20205-124">说明</span><span class="sxs-lookup"><span data-stu-id="20205-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20205-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="20205-125">Authorization</span></span>  | <span data-ttu-id="20205-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20205-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20205-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="20205-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="20205-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="20205-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20205-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="20205-131">Request body</span></span>
<span data-ttu-id="20205-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="20205-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20205-133">响应</span><span class="sxs-lookup"><span data-stu-id="20205-133">Response</span></span>

<span data-ttu-id="20205-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [workbookTableColumn](../resources/workbooktablecolumn.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="20205-134">If successful, this method returns a `200 OK` response code and collection of [workbookTableColumn](../resources/workbooktablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20205-135">示例</span><span class="sxs-lookup"><span data-stu-id="20205-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20205-136">请求</span><span class="sxs-lookup"><span data-stu-id="20205-136">Request</span></span>
<span data-ttu-id="20205-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20205-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20205-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="20205-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
# <a name="c"></a>[<span data-ttu-id="20205-139">C#</span><span class="sxs-lookup"><span data-stu-id="20205-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20205-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20205-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20205-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20205-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="20205-142">响应</span><span class="sxs-lookup"><span data-stu-id="20205-142">Response</span></span>
<span data-ttu-id="20205-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="20205-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

> <span data-ttu-id="20205-146">
  \**注意：\** 使用 [$top](/graph/query-parameters#top) 和 [$skip](/graph/query-parameters#skip-parameter) 查询参数可逐个浏览许多列。</span><span class="sxs-lookup"><span data-stu-id="20205-146">**Note:** Use the [$top](/graph/query-parameters#top) and [$skip](/graph/query-parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="20205-147">示例：</span><span class="sxs-lookup"><span data-stu-id="20205-147">Example:</span></span> 

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
  ]
}
-->