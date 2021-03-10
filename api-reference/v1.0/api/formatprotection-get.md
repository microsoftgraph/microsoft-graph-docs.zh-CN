---
title: 获取 FormatProtection
description: 检索 formatprotection 对象的属性和关系。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f50641afa7d66989ed5438f7ba823a646b1b8ebe
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575593"
---
# <a name="get-formatprotection"></a><span data-ttu-id="35244-103">获取 FormatProtection</span><span class="sxs-lookup"><span data-stu-id="35244-103">Get FormatProtection</span></span>

<span data-ttu-id="35244-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35244-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35244-105">检索 formatprotection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35244-105">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="35244-106">权限</span><span class="sxs-lookup"><span data-stu-id="35244-106">Permissions</span></span>
<span data-ttu-id="35244-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35244-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35244-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="35244-109">Permission type</span></span>      | <span data-ttu-id="35244-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="35244-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35244-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35244-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35244-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35244-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="35244-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35244-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35244-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="35244-114">Not supported.</span></span>    |
|<span data-ttu-id="35244-115">Application</span><span class="sxs-lookup"><span data-stu-id="35244-115">Application</span></span> | <span data-ttu-id="35244-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="35244-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35244-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35244-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/format/protection
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/protection
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="35244-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="35244-118">Optional query parameters</span></span>
<span data-ttu-id="35244-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="35244-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35244-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="35244-120">Request headers</span></span>
| <span data-ttu-id="35244-121">名称</span><span class="sxs-lookup"><span data-stu-id="35244-121">Name</span></span>      |<span data-ttu-id="35244-122">说明</span><span class="sxs-lookup"><span data-stu-id="35244-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="35244-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35244-123">Authorization</span></span>  | <span data-ttu-id="35244-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="35244-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="35244-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="35244-126">Request body</span></span>
<span data-ttu-id="35244-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="35244-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35244-128">响应</span><span class="sxs-lookup"><span data-stu-id="35244-128">Response</span></span>

<span data-ttu-id="35244-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [FormatProtection](../resources/formatprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35244-129">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35244-130">示例</span><span class="sxs-lookup"><span data-stu-id="35244-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35244-131">请求</span><span class="sxs-lookup"><span data-stu-id="35244-131">Request</span></span>
<span data-ttu-id="35244-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35244-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="35244-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="35244-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
```
# <a name="c"></a>[<span data-ttu-id="35244-134">C#</span><span class="sxs-lookup"><span data-stu-id="35244-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35244-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35244-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35244-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35244-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35244-137">Java</span><span class="sxs-lookup"><span data-stu-id="35244-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-formatprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="35244-138">响应</span><span class="sxs-lookup"><span data-stu-id="35244-138">Response</span></span>
<span data-ttu-id="35244-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35244-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
