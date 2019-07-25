---
title: Get WorksheetProtection
description: 检索 worksheetprotection 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 971255f6472b3a09b0769ea13b72527f8a2459a5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884184"
---
# <a name="get-worksheetprotection"></a><span data-ttu-id="c5fd6-103">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="c5fd6-103">Get WorksheetProtection</span></span>

<span data-ttu-id="c5fd6-104">检索 worksheetprotection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c5fd6-104">Retrieve the properties and relationships of worksheetprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5fd6-105">权限</span><span class="sxs-lookup"><span data-stu-id="c5fd6-105">Permissions</span></span>
<span data-ttu-id="c5fd6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5fd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5fd6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5fd6-108">Permission type</span></span>      | <span data-ttu-id="c5fd6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5fd6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5fd6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5fd6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c5fd6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5fd6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5fd6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5fd6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5fd6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5fd6-113">Not supported.</span></span>    |
|<span data-ttu-id="c5fd6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5fd6-114">Application</span></span> | <span data-ttu-id="c5fd6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5fd6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5fd6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5fd6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5fd6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5fd6-117">Optional query parameters</span></span>
<span data-ttu-id="c5fd6-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c5fd6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5fd6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5fd6-119">Request headers</span></span>
| <span data-ttu-id="c5fd6-120">名称</span><span class="sxs-lookup"><span data-stu-id="c5fd6-120">Name</span></span>      |<span data-ttu-id="c5fd6-121">说明</span><span class="sxs-lookup"><span data-stu-id="c5fd6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5fd6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5fd6-122">Authorization</span></span>  | <span data-ttu-id="c5fd6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5fd6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5fd6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c5fd6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c5fd6-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c5fd6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5fd6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5fd6-128">Request body</span></span>
<span data-ttu-id="c5fd6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5fd6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5fd6-130">响应</span><span class="sxs-lookup"><span data-stu-id="c5fd6-130">Response</span></span>

<span data-ttu-id="c5fd6-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[WorkbookWorksheetProtection](../resources/worksheetprotection.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5fd6-131">If successful, this method returns a `200 OK` response code and [WorkbookWorksheetProtection](../resources/worksheetprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5fd6-132">示例</span><span class="sxs-lookup"><span data-stu-id="c5fd6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5fd6-133">请求</span><span class="sxs-lookup"><span data-stu-id="c5fd6-133">Request</span></span>
<span data-ttu-id="c5fd6-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5fd6-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c5fd6-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c5fd6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_worksheetprotection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c5fd6-136">C#</span><span class="sxs-lookup"><span data-stu-id="c5fd6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-worksheetprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5fd6-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="c5fd6-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-worksheetprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c5fd6-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="c5fd6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-worksheetprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c5fd6-139">Java</span><span class="sxs-lookup"><span data-stu-id="c5fd6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-worksheetprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c5fd6-140">响应</span><span class="sxs-lookup"><span data-stu-id="c5fd6-140">Response</span></span>
<span data-ttu-id="c5fd6-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5fd6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
