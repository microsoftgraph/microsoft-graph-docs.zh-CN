---
title: 列出 TableRowCollection
description: 检索 tablerow 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 09dadd17b305ea4dd78bd87718f9f9896e606997
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729103"
---
# <a name="list-tablerowcollection"></a><span data-ttu-id="9911f-103">列出 TableRowCollection</span><span class="sxs-lookup"><span data-stu-id="9911f-103">List TableRowCollection</span></span>

<span data-ttu-id="9911f-104">检索 tablerow 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9911f-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9911f-105">权限</span><span class="sxs-lookup"><span data-stu-id="9911f-105">Permissions</span></span>
<span data-ttu-id="9911f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9911f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9911f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9911f-108">Permission type</span></span>      | <span data-ttu-id="9911f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9911f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9911f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9911f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9911f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9911f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9911f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9911f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9911f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9911f-113">Not supported.</span></span>    |
|<span data-ttu-id="9911f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9911f-114">Application</span></span> | <span data-ttu-id="9911f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9911f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9911f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9911f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9911f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9911f-117">Optional query parameters</span></span>
<span data-ttu-id="9911f-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9911f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9911f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9911f-119">Request headers</span></span>
| <span data-ttu-id="9911f-120">名称</span><span class="sxs-lookup"><span data-stu-id="9911f-120">Name</span></span>      |<span data-ttu-id="9911f-121">说明</span><span class="sxs-lookup"><span data-stu-id="9911f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9911f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9911f-122">Authorization</span></span>  | <span data-ttu-id="9911f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9911f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9911f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9911f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9911f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9911f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9911f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9911f-128">Request body</span></span>
<span data-ttu-id="9911f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9911f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9911f-130">响应</span><span class="sxs-lookup"><span data-stu-id="9911f-130">Response</span></span>

<span data-ttu-id="9911f-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[WorkbookTableRow](../resources/tablerow.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="9911f-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9911f-132">示例</span><span class="sxs-lookup"><span data-stu-id="9911f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9911f-133">请求</span><span class="sxs-lookup"><span data-stu-id="9911f-133">Request</span></span>
<span data-ttu-id="9911f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9911f-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9911f-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9911f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablerowcollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9911f-136">C#</span><span class="sxs-lookup"><span data-stu-id="9911f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablerowcollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9911f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9911f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablerowcollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9911f-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="9911f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablerowcollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9911f-139">Java</span><span class="sxs-lookup"><span data-stu-id="9911f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablerowcollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9911f-140">响应</span><span class="sxs-lookup"><span data-stu-id="9911f-140">Response</span></span>
<span data-ttu-id="9911f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9911f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 82

{
  "value": [
    {
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableRowCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
