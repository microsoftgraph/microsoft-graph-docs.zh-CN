---
title: 获取 FormatProtection
description: 检索 formatprotection 对象的属性和关系。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 315fea99555a48066eb61aba1986ec9e3e1c0e86
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054012"
---
# <a name="get-formatprotection"></a><span data-ttu-id="2334e-103">获取 FormatProtection</span><span class="sxs-lookup"><span data-stu-id="2334e-103">Get FormatProtection</span></span>

<span data-ttu-id="2334e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2334e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2334e-105">检索 formatprotection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2334e-105">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2334e-106">权限</span><span class="sxs-lookup"><span data-stu-id="2334e-106">Permissions</span></span>
<span data-ttu-id="2334e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2334e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2334e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2334e-109">Permission type</span></span>      | <span data-ttu-id="2334e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2334e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2334e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2334e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2334e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2334e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2334e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2334e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2334e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2334e-114">Not supported.</span></span>    |
|<span data-ttu-id="2334e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2334e-115">Application</span></span> | <span data-ttu-id="2334e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2334e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2334e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2334e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/format/protection
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/protection
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2334e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2334e-118">Optional query parameters</span></span>
<span data-ttu-id="2334e-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2334e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2334e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2334e-120">Request headers</span></span>
| <span data-ttu-id="2334e-121">名称</span><span class="sxs-lookup"><span data-stu-id="2334e-121">Name</span></span>      |<span data-ttu-id="2334e-122">说明</span><span class="sxs-lookup"><span data-stu-id="2334e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2334e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2334e-123">Authorization</span></span>  | <span data-ttu-id="2334e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2334e-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2334e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2334e-126">Request body</span></span>
<span data-ttu-id="2334e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2334e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2334e-128">响应</span><span class="sxs-lookup"><span data-stu-id="2334e-128">Response</span></span>

<span data-ttu-id="2334e-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [FormatProtection](../resources/formatprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2334e-129">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2334e-130">示例</span><span class="sxs-lookup"><span data-stu-id="2334e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2334e-131">请求</span><span class="sxs-lookup"><span data-stu-id="2334e-131">Request</span></span>
<span data-ttu-id="2334e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2334e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2334e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2334e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
```
# <a name="c"></a>[<span data-ttu-id="2334e-134">C#</span><span class="sxs-lookup"><span data-stu-id="2334e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2334e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2334e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2334e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2334e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2334e-137">Java</span><span class="sxs-lookup"><span data-stu-id="2334e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-formatprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2334e-138">响应</span><span class="sxs-lookup"><span data-stu-id="2334e-138">Response</span></span>
<span data-ttu-id="2334e-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2334e-139">Here is an example of the response.</span></span> <span data-ttu-id="2334e-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2334e-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
