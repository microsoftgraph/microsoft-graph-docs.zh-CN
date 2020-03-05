---
title: 获取 NamedItem
description: 检索 nameditem 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 48a61c6833619e77c37df9d9bb02f9daac756047
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456794"
---
# <a name="get-nameditem"></a><span data-ttu-id="36f6b-103">获取 NamedItem</span><span class="sxs-lookup"><span data-stu-id="36f6b-103">Get NamedItem</span></span>

<span data-ttu-id="36f6b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="36f6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36f6b-105">检索 nameditem 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="36f6b-105">Retrieve the properties and relationships of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="36f6b-106">权限</span><span class="sxs-lookup"><span data-stu-id="36f6b-106">Permissions</span></span>
<span data-ttu-id="36f6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36f6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36f6b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="36f6b-109">Permission type</span></span>      | <span data-ttu-id="36f6b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36f6b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36f6b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36f6b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="36f6b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36f6b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36f6b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36f6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36f6b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36f6b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36f6b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="36f6b-115">Application</span></span> | <span data-ttu-id="36f6b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36f6b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36f6b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36f6b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="36f6b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="36f6b-118">Optional query parameters</span></span>
<span data-ttu-id="36f6b-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="36f6b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36f6b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="36f6b-120">Request headers</span></span>
| <span data-ttu-id="36f6b-121">名称</span><span class="sxs-lookup"><span data-stu-id="36f6b-121">Name</span></span>      |<span data-ttu-id="36f6b-122">说明</span><span class="sxs-lookup"><span data-stu-id="36f6b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="36f6b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36f6b-123">Authorization</span></span>  | <span data-ttu-id="36f6b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36f6b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36f6b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="36f6b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="36f6b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="36f6b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36f6b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="36f6b-129">Request body</span></span>
<span data-ttu-id="36f6b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36f6b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36f6b-131">响应</span><span class="sxs-lookup"><span data-stu-id="36f6b-131">Response</span></span>

<span data-ttu-id="36f6b-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[workbookNamedItem](../resources/workbooknameditem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="36f6b-132">If successful, this method returns a `200 OK` response code and [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36f6b-133">示例</span><span class="sxs-lookup"><span data-stu-id="36f6b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36f6b-134">请求</span><span class="sxs-lookup"><span data-stu-id="36f6b-134">Request</span></span>
<span data-ttu-id="36f6b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36f6b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="36f6b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="36f6b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_nameditem"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}
```
# <a name="c"></a>[<span data-ttu-id="36f6b-137">C#</span><span class="sxs-lookup"><span data-stu-id="36f6b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-nameditem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36f6b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36f6b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-nameditem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36f6b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36f6b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-nameditem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="36f6b-140">响应</span><span class="sxs-lookup"><span data-stu-id="36f6b-140">Response</span></span>
<span data-ttu-id="36f6b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36f6b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get NamedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
