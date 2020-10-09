---
title: 获取 workbookWorksheetProtection
description: 检索 workbookworksheetprotection 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bac6180f92a4ad7d0cfc2bc72770f0b1939f3ea4
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405685"
---
# <a name="get-workbookworksheetprotection"></a><span data-ttu-id="ddf22-103">获取 workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="ddf22-103">Get workbookWorksheetProtection</span></span>

<span data-ttu-id="ddf22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddf22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddf22-105">检索 workbookWorksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ddf22-105">Retrieve the properties and relationships of workbookWorksheetProtection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ddf22-106">权限</span><span class="sxs-lookup"><span data-stu-id="ddf22-106">Permissions</span></span>
<span data-ttu-id="ddf22-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddf22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddf22-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddf22-109">Permission type</span></span>      | <span data-ttu-id="ddf22-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ddf22-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddf22-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddf22-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ddf22-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddf22-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ddf22-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddf22-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddf22-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddf22-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ddf22-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddf22-115">Application</span></span> | <span data-ttu-id="ddf22-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddf22-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddf22-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddf22-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ddf22-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ddf22-118">Optional query parameters</span></span>
<span data-ttu-id="ddf22-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ddf22-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddf22-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddf22-120">Request headers</span></span>
| <span data-ttu-id="ddf22-121">名称</span><span class="sxs-lookup"><span data-stu-id="ddf22-121">Name</span></span>      |<span data-ttu-id="ddf22-122">说明</span><span class="sxs-lookup"><span data-stu-id="ddf22-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ddf22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddf22-123">Authorization</span></span>  | <span data-ttu-id="ddf22-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ddf22-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddf22-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ddf22-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="ddf22-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ddf22-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddf22-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddf22-129">Request body</span></span>
<span data-ttu-id="ddf22-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ddf22-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddf22-131">响应</span><span class="sxs-lookup"><span data-stu-id="ddf22-131">Response</span></span>

<span data-ttu-id="ddf22-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ddf22-132">If successful, this method returns a `200 OK` response code and [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ddf22-133">示例</span><span class="sxs-lookup"><span data-stu-id="ddf22-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ddf22-134">请求</span><span class="sxs-lookup"><span data-stu-id="ddf22-134">Request</span></span>
<span data-ttu-id="ddf22-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddf22-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddf22-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddf22-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookworksheetprotection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection
```
# <a name="c"></a>[<span data-ttu-id="ddf22-137">C#</span><span class="sxs-lookup"><span data-stu-id="ddf22-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookworksheetprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddf22-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddf22-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookworksheetprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddf22-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddf22-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookworksheetprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ddf22-140">响应</span><span class="sxs-lookup"><span data-stu-id="ddf22-140">Response</span></span>
<span data-ttu-id="ddf22-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ddf22-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get workbookWorksheetProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->