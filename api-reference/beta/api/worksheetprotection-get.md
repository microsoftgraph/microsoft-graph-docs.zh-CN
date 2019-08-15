---
title: 获取 workbookWorksheetProtection
description: 检索 workbookworksheetprotection 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 295ac6ac4fb866a6ab6167a990c4309b08cac049
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420881"
---
# <a name="get-workbookworksheetprotection"></a><span data-ttu-id="6ad8c-103">获取 workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="6ad8c-103">Get workbookWorksheetProtection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ad8c-104">检索 workbookWorksheetProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6ad8c-104">Retrieve the properties and relationships of workbookWorksheetProtection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ad8c-105">权限</span><span class="sxs-lookup"><span data-stu-id="6ad8c-105">Permissions</span></span>
<span data-ttu-id="6ad8c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ad8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ad8c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ad8c-108">Permission type</span></span>      | <span data-ttu-id="6ad8c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ad8c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ad8c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ad8c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ad8c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ad8c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ad8c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ad8c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ad8c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ad8c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ad8c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ad8c-114">Application</span></span> | <span data-ttu-id="6ad8c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ad8c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ad8c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ad8c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ad8c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6ad8c-117">Optional query parameters</span></span>
<span data-ttu-id="6ad8c-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6ad8c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ad8c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ad8c-119">Request headers</span></span>
| <span data-ttu-id="6ad8c-120">名称</span><span class="sxs-lookup"><span data-stu-id="6ad8c-120">Name</span></span>      |<span data-ttu-id="6ad8c-121">说明</span><span class="sxs-lookup"><span data-stu-id="6ad8c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ad8c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ad8c-122">Authorization</span></span>  | <span data-ttu-id="6ad8c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ad8c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ad8c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6ad8c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6ad8c-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6ad8c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ad8c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ad8c-128">Request body</span></span>
<span data-ttu-id="6ad8c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ad8c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ad8c-130">响应</span><span class="sxs-lookup"><span data-stu-id="6ad8c-130">Response</span></span>

<span data-ttu-id="6ad8c-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6ad8c-131">If successful, this method returns a `200 OK` response code and [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ad8c-132">示例</span><span class="sxs-lookup"><span data-stu-id="6ad8c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ad8c-133">请求</span><span class="sxs-lookup"><span data-stu-id="6ad8c-133">Request</span></span>
<span data-ttu-id="6ad8c-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ad8c-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6ad8c-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6ad8c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookworksheetprotection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ad8c-136">C#</span><span class="sxs-lookup"><span data-stu-id="6ad8c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookworksheetprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ad8c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ad8c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookworksheetprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ad8c-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="6ad8c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookworksheetprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6ad8c-139">响应</span><span class="sxs-lookup"><span data-stu-id="6ad8c-139">Response</span></span>
<span data-ttu-id="6ad8c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ad8c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
