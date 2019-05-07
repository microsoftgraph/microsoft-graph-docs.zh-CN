---
title: 列出 WorksheetCollection
description: 检索 worksheet 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ecbc2c39755612de8af81154c2f1359ed65f7997
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601738"
---
# <a name="list-worksheetcollection"></a><span data-ttu-id="0ab66-103">列出 WorksheetCollection</span><span class="sxs-lookup"><span data-stu-id="0ab66-103">List WorksheetCollection</span></span>

<span data-ttu-id="0ab66-104">检索 worksheet 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="0ab66-104">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ab66-105">权限</span><span class="sxs-lookup"><span data-stu-id="0ab66-105">Permissions</span></span>
<span data-ttu-id="0ab66-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ab66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ab66-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ab66-108">Permission type</span></span>      | <span data-ttu-id="0ab66-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ab66-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ab66-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ab66-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ab66-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ab66-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ab66-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ab66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ab66-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ab66-113">Not supported.</span></span>    |
|<span data-ttu-id="0ab66-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ab66-114">Application</span></span> | <span data-ttu-id="0ab66-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ab66-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ab66-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ab66-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ab66-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ab66-117">Optional query parameters</span></span>
<span data-ttu-id="0ab66-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0ab66-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ab66-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ab66-119">Request headers</span></span>
| <span data-ttu-id="0ab66-120">名称</span><span class="sxs-lookup"><span data-stu-id="0ab66-120">Name</span></span>      |<span data-ttu-id="0ab66-121">说明</span><span class="sxs-lookup"><span data-stu-id="0ab66-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ab66-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ab66-122">Authorization</span></span>  | <span data-ttu-id="0ab66-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ab66-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ab66-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0ab66-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0ab66-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0ab66-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ab66-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ab66-128">Request body</span></span>
<span data-ttu-id="0ab66-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ab66-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ab66-130">响应</span><span class="sxs-lookup"><span data-stu-id="0ab66-130">Response</span></span>

<span data-ttu-id="0ab66-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[WorkbookWorksheet](../resources/worksheet.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="0ab66-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookWorksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ab66-132">示例</span><span class="sxs-lookup"><span data-stu-id="0ab66-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ab66-133">请求</span><span class="sxs-lookup"><span data-stu-id="0ab66-133">Request</span></span>
<span data-ttu-id="0ab66-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ab66-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheetcollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="0ab66-135">响应</span><span class="sxs-lookup"><span data-stu-id="0ab66-135">Response</span></span>
<span data-ttu-id="0ab66-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ab66-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0ab66-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0ab66-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0ab66-140">语言</span><span class="sxs-lookup"><span data-stu-id="0ab66-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_worksheetcollection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ab66-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ab66-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_worksheetcollection-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List WorksheetCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheet-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
