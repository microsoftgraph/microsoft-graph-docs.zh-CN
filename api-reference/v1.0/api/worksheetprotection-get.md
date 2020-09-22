---
title: Get WorksheetProtection
description: 检索 worksheetprotection 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8ff282521987b9962bc0ee99d8673be178200b06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086863"
---
# <a name="get-worksheetprotection"></a><span data-ttu-id="19041-103">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="19041-103">Get WorksheetProtection</span></span>

<span data-ttu-id="19041-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19041-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19041-105">检索 worksheetprotection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="19041-105">Retrieve the properties and relationships of worksheetprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="19041-106">权限</span><span class="sxs-lookup"><span data-stu-id="19041-106">Permissions</span></span>
<span data-ttu-id="19041-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19041-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19041-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="19041-109">Permission type</span></span>      | <span data-ttu-id="19041-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19041-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19041-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19041-111">Delegated (work or school account)</span></span> | <span data-ttu-id="19041-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19041-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19041-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19041-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19041-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="19041-114">Not supported.</span></span>    |
|<span data-ttu-id="19041-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="19041-115">Application</span></span> | <span data-ttu-id="19041-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19041-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19041-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19041-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="19041-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="19041-118">Optional query parameters</span></span>
<span data-ttu-id="19041-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="19041-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19041-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="19041-120">Request headers</span></span>
| <span data-ttu-id="19041-121">名称</span><span class="sxs-lookup"><span data-stu-id="19041-121">Name</span></span>      |<span data-ttu-id="19041-122">说明</span><span class="sxs-lookup"><span data-stu-id="19041-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19041-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19041-123">Authorization</span></span>  | <span data-ttu-id="19041-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19041-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19041-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="19041-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="19041-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="19041-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19041-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="19041-129">Request body</span></span>
<span data-ttu-id="19041-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19041-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19041-131">响应</span><span class="sxs-lookup"><span data-stu-id="19041-131">Response</span></span>

<span data-ttu-id="19041-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [WorkbookWorksheetProtection](../resources/worksheetprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19041-132">If successful, this method returns a `200 OK` response code and [WorkbookWorksheetProtection](../resources/worksheetprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19041-133">示例</span><span class="sxs-lookup"><span data-stu-id="19041-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19041-134">请求</span><span class="sxs-lookup"><span data-stu-id="19041-134">Request</span></span>
<span data-ttu-id="19041-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19041-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19041-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="19041-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_worksheetprotection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection
```
# <a name="c"></a>[<span data-ttu-id="19041-137">C#</span><span class="sxs-lookup"><span data-stu-id="19041-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-worksheetprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19041-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19041-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-worksheetprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19041-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19041-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-worksheetprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19041-140">Java</span><span class="sxs-lookup"><span data-stu-id="19041-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-worksheetprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="19041-141">响应</span><span class="sxs-lookup"><span data-stu-id="19041-141">Response</span></span>
<span data-ttu-id="19041-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19041-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 23

{
  "protected": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get WorksheetProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

