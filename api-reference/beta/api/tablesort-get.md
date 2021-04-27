---
title: Get TableSort
description: 检索 tablesort 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ac6b76c6a7abdd0a773a2acdb62cd2abafc75b8b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050834"
---
# <a name="get-tablesort"></a><span data-ttu-id="10e45-103">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="10e45-103">Get TableSort</span></span>

<span data-ttu-id="10e45-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10e45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10e45-105">检索 tablesort 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10e45-105">Retrieve the properties and relationships of tablesort object.</span></span>
## <a name="permissions"></a><span data-ttu-id="10e45-106">权限</span><span class="sxs-lookup"><span data-stu-id="10e45-106">Permissions</span></span>
<span data-ttu-id="10e45-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10e45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10e45-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="10e45-109">Permission type</span></span>      | <span data-ttu-id="10e45-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10e45-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10e45-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10e45-111">Delegated (work or school account)</span></span> | <span data-ttu-id="10e45-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10e45-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="10e45-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10e45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10e45-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10e45-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="10e45-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="10e45-115">Application</span></span> | <span data-ttu-id="10e45-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="10e45-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10e45-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10e45-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/sort
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10e45-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="10e45-118">Optional query parameters</span></span>
<span data-ttu-id="10e45-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="10e45-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10e45-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="10e45-120">Request headers</span></span>
| <span data-ttu-id="10e45-121">名称</span><span class="sxs-lookup"><span data-stu-id="10e45-121">Name</span></span>      |<span data-ttu-id="10e45-122">说明</span><span class="sxs-lookup"><span data-stu-id="10e45-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10e45-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10e45-123">Authorization</span></span>  | <span data-ttu-id="10e45-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="10e45-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10e45-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="10e45-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="10e45-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="10e45-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10e45-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="10e45-129">Request body</span></span>
<span data-ttu-id="10e45-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10e45-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10e45-131">响应</span><span class="sxs-lookup"><span data-stu-id="10e45-131">Response</span></span>

<span data-ttu-id="10e45-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [workbookTableSort](../resources/workbooktablesort.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10e45-132">If successful, this method returns a `200 OK` response code and [workbookTableSort](../resources/workbooktablesort.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10e45-133">示例</span><span class="sxs-lookup"><span data-stu-id="10e45-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10e45-134">请求</span><span class="sxs-lookup"><span data-stu-id="10e45-134">Request</span></span>
<span data-ttu-id="10e45-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10e45-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10e45-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="10e45-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablesort"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort
```
# <a name="c"></a>[<span data-ttu-id="10e45-137">C#</span><span class="sxs-lookup"><span data-stu-id="10e45-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablesort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10e45-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10e45-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablesort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10e45-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10e45-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablesort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10e45-140">Java</span><span class="sxs-lookup"><span data-stu-id="10e45-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablesort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="10e45-141">响应</span><span class="sxs-lookup"><span data-stu-id="10e45-141">Response</span></span>
<span data-ttu-id="10e45-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="10e45-142">Here is an example of the response.</span></span> <span data-ttu-id="10e45-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="10e45-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableSort"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "matchCase": true,
  "method": "method-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get TableSort",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
