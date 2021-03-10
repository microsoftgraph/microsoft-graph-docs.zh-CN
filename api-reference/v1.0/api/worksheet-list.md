---
title: 列出 WorksheetCollection
description: 检索 worksheet 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 83cfd30ccd91a9c549e45be2a4d44106be465503
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573596"
---
# <a name="list-worksheetcollection"></a><span data-ttu-id="52ffc-103">列出 WorksheetCollection</span><span class="sxs-lookup"><span data-stu-id="52ffc-103">List WorksheetCollection</span></span>

<span data-ttu-id="52ffc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52ffc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52ffc-105">检索 worksheet 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="52ffc-105">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="52ffc-106">权限</span><span class="sxs-lookup"><span data-stu-id="52ffc-106">Permissions</span></span>
<span data-ttu-id="52ffc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52ffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52ffc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="52ffc-109">Permission type</span></span>      | <span data-ttu-id="52ffc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="52ffc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52ffc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52ffc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="52ffc-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52ffc-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52ffc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52ffc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52ffc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="52ffc-114">Not supported.</span></span>    |
|<span data-ttu-id="52ffc-115">Application</span><span class="sxs-lookup"><span data-stu-id="52ffc-115">Application</span></span> | <span data-ttu-id="52ffc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="52ffc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52ffc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52ffc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets
GET /me/drive/root:/{item-path}:/workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52ffc-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="52ffc-118">Optional query parameters</span></span>
<span data-ttu-id="52ffc-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="52ffc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52ffc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="52ffc-120">Request headers</span></span>
| <span data-ttu-id="52ffc-121">名称</span><span class="sxs-lookup"><span data-stu-id="52ffc-121">Name</span></span>      |<span data-ttu-id="52ffc-122">说明</span><span class="sxs-lookup"><span data-stu-id="52ffc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52ffc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52ffc-123">Authorization</span></span>  | <span data-ttu-id="52ffc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="52ffc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52ffc-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="52ffc-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="52ffc-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="52ffc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52ffc-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="52ffc-129">Request body</span></span>
<span data-ttu-id="52ffc-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="52ffc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52ffc-131">响应</span><span class="sxs-lookup"><span data-stu-id="52ffc-131">Response</span></span>

<span data-ttu-id="52ffc-132">如果成功，此方法在响应正文中返回 `200 OK` [一个响应代码和 WorkbookWorksheet](../resources/worksheet.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="52ffc-132">If successful, this method returns a `200 OK` response code and collection of [WorkbookWorksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52ffc-133">示例</span><span class="sxs-lookup"><span data-stu-id="52ffc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52ffc-134">请求</span><span class="sxs-lookup"><span data-stu-id="52ffc-134">Request</span></span>
<span data-ttu-id="52ffc-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="52ffc-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52ffc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="52ffc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_worksheetcollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
# <a name="c"></a>[<span data-ttu-id="52ffc-137">C#</span><span class="sxs-lookup"><span data-stu-id="52ffc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-worksheetcollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52ffc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52ffc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-worksheetcollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52ffc-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52ffc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-worksheetcollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52ffc-140">Java</span><span class="sxs-lookup"><span data-stu-id="52ffc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-worksheetcollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="52ffc-141">响应</span><span class="sxs-lookup"><span data-stu-id="52ffc-141">Response</span></span>
<span data-ttu-id="52ffc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="52ffc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List WorksheetCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
