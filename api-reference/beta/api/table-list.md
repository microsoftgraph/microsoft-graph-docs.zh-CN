---
title: 列出表集合
description: 检索 table 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4d0f9ca75314b4ad0ee4b4f10efdacd3f9c98f66
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637862"
---
# <a name="list-tablecollection"></a><span data-ttu-id="bbe5f-103">列出表集合</span><span class="sxs-lookup"><span data-stu-id="bbe5f-103">List TableCollection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbe5f-104">检索 table 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="bbe5f-104">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="bbe5f-105">权限</span><span class="sxs-lookup"><span data-stu-id="bbe5f-105">Permissions</span></span>
<span data-ttu-id="bbe5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbe5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbe5f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbe5f-108">Permission type</span></span>      | <span data-ttu-id="bbe5f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbe5f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbe5f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbe5f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bbe5f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bbe5f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bbe5f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbe5f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbe5f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bbe5f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bbe5f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbe5f-114">Application</span></span> | <span data-ttu-id="bbe5f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbe5f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbe5f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbe5f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables
GET /workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bbe5f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bbe5f-117">Optional query parameters</span></span>
<span data-ttu-id="bbe5f-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bbe5f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbe5f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbe5f-119">Request headers</span></span>
| <span data-ttu-id="bbe5f-120">名称</span><span class="sxs-lookup"><span data-stu-id="bbe5f-120">Name</span></span>      |<span data-ttu-id="bbe5f-121">说明</span><span class="sxs-lookup"><span data-stu-id="bbe5f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bbe5f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbe5f-122">Authorization</span></span>  | <span data-ttu-id="bbe5f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbe5f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bbe5f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bbe5f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="bbe5f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="bbe5f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbe5f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbe5f-128">Request body</span></span>
<span data-ttu-id="bbe5f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bbe5f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbe5f-130">响应</span><span class="sxs-lookup"><span data-stu-id="bbe5f-130">Response</span></span>

<span data-ttu-id="bbe5f-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[workbookTable](../resources/workbooktable.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="bbe5f-131">If successful, this method returns a `200 OK` response code and collection of [workbookTable](../resources/workbooktable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bbe5f-132">示例</span><span class="sxs-lookup"><span data-stu-id="bbe5f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbe5f-133">请求</span><span class="sxs-lookup"><span data-stu-id="bbe5f-133">Request</span></span>
<span data-ttu-id="bbe5f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bbe5f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables
```
##### <a name="response"></a><span data-ttu-id="bbe5f-135">响应</span><span class="sxs-lookup"><span data-stu-id="bbe5f-135">Response</span></span>
<span data-ttu-id="bbe5f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bbe5f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "id": "99",
      "name": "name-value",
      "showHeaders": true,
      "showTotals": true,
      "style": "style-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bbe5f-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bbe5f-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bbe5f-140">语言</span><span class="sxs-lookup"><span data-stu-id="bbe5f-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tablecollection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bbe5f-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="bbe5f-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tablecollection-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TableCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/table-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
