---
title: 列出 TableRowCollection
description: 检索 tablerow 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 54a24ec49bc45e72bed139e64293d2dc2a1a4f60
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602510"
---
# <a name="list-tablerowcollection"></a><span data-ttu-id="cb985-103">列出 TableRowCollection</span><span class="sxs-lookup"><span data-stu-id="cb985-103">List TableRowCollection</span></span>

<span data-ttu-id="cb985-104">检索 tablerow 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="cb985-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="cb985-105">权限</span><span class="sxs-lookup"><span data-stu-id="cb985-105">Permissions</span></span>
<span data-ttu-id="cb985-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb985-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb985-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb985-108">Permission type</span></span>      | <span data-ttu-id="cb985-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb985-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb985-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb985-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb985-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb985-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cb985-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb985-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb985-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb985-113">Not supported.</span></span>    |
|<span data-ttu-id="cb985-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb985-114">Application</span></span> | <span data-ttu-id="cb985-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb985-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb985-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb985-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cb985-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cb985-117">Optional query parameters</span></span>
<span data-ttu-id="cb985-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cb985-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb985-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb985-119">Request headers</span></span>
| <span data-ttu-id="cb985-120">名称</span><span class="sxs-lookup"><span data-stu-id="cb985-120">Name</span></span>      |<span data-ttu-id="cb985-121">说明</span><span class="sxs-lookup"><span data-stu-id="cb985-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cb985-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb985-122">Authorization</span></span>  | <span data-ttu-id="cb985-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb985-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cb985-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cb985-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="cb985-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="cb985-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb985-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb985-128">Request body</span></span>
<span data-ttu-id="cb985-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb985-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb985-130">响应</span><span class="sxs-lookup"><span data-stu-id="cb985-130">Response</span></span>

<span data-ttu-id="cb985-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[WorkbookTableRow](../resources/tablerow.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="cb985-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cb985-132">示例</span><span class="sxs-lookup"><span data-stu-id="cb985-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb985-133">请求</span><span class="sxs-lookup"><span data-stu-id="cb985-133">Request</span></span>
<span data-ttu-id="cb985-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cb985-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablerowcollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows
```
##### <a name="response"></a><span data-ttu-id="cb985-135">响应</span><span class="sxs-lookup"><span data-stu-id="cb985-135">Response</span></span>
<span data-ttu-id="cb985-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cb985-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cb985-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="cb985-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cb985-140">语言</span><span class="sxs-lookup"><span data-stu-id="cb985-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tablerowcollection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cb985-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="cb985-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tablerowcollection-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableRowCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablerow-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablerow-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
