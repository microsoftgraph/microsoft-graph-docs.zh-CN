---
title: 获取 RangeFill
description: 检索 rangefill 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 62c4cda8d81581b1f495f679aa26a0b7c8c295f2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055020"
---
# <a name="get-rangefill"></a><span data-ttu-id="9c29c-103">获取 RangeFill</span><span class="sxs-lookup"><span data-stu-id="9c29c-103">Get RangeFill</span></span>

<span data-ttu-id="9c29c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c29c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c29c-105">检索 rangefill 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9c29c-105">Retrieve the properties and relationships of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c29c-106">权限</span><span class="sxs-lookup"><span data-stu-id="9c29c-106">Permissions</span></span>
<span data-ttu-id="9c29c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c29c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c29c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c29c-109">Permission type</span></span>      | <span data-ttu-id="9c29c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c29c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c29c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c29c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9c29c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c29c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9c29c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c29c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c29c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c29c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9c29c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c29c-115">Application</span></span> | <span data-ttu-id="9c29c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c29c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c29c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c29c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/format/fill
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/fill
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/fill
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/fill
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/fill
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9c29c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9c29c-118">Optional query parameters</span></span>
<span data-ttu-id="9c29c-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9c29c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c29c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c29c-120">Request headers</span></span>
| <span data-ttu-id="9c29c-121">名称</span><span class="sxs-lookup"><span data-stu-id="9c29c-121">Name</span></span>      |<span data-ttu-id="9c29c-122">说明</span><span class="sxs-lookup"><span data-stu-id="9c29c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9c29c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c29c-123">Authorization</span></span>  | <span data-ttu-id="9c29c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c29c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c29c-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9c29c-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="9c29c-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9c29c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c29c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c29c-129">Request body</span></span>
<span data-ttu-id="9c29c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c29c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c29c-131">响应</span><span class="sxs-lookup"><span data-stu-id="9c29c-131">Response</span></span>

<span data-ttu-id="9c29c-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [workbookRangeFill](../resources/workbookrangefill.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c29c-132">If successful, this method returns a `200 OK` response code and [workbookRangeFill](../resources/workbookrangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c29c-133">示例</span><span class="sxs-lookup"><span data-stu-id="9c29c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c29c-134">请求</span><span class="sxs-lookup"><span data-stu-id="9c29c-134">Request</span></span>
<span data-ttu-id="9c29c-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c29c-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c29c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c29c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rangefill"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/fill
```
# <a name="c"></a>[<span data-ttu-id="9c29c-137">C#</span><span class="sxs-lookup"><span data-stu-id="9c29c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rangefill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c29c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c29c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rangefill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c29c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c29c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rangefill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c29c-140">Java</span><span class="sxs-lookup"><span data-stu-id="9c29c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rangefill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9c29c-141">响应</span><span class="sxs-lookup"><span data-stu-id="9c29c-141">Response</span></span>
<span data-ttu-id="9c29c-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9c29c-142">Here is an example of the response.</span></span> <span data-ttu-id="9c29c-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9c29c-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get RangeFill",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
