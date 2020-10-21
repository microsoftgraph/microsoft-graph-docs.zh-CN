---
title: 列出 NamedItemCollection
description: 检索 nameditem 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: 67b731cfc36925fe2e704b5506e681424b0c33d5
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635318"
---
# <a name="list-nameditemcollection"></a><span data-ttu-id="6ca03-103">列出 NamedItemCollection</span><span class="sxs-lookup"><span data-stu-id="6ca03-103">List NamedItemCollection</span></span>

<span data-ttu-id="6ca03-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ca03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ca03-105">检索 nameditem 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="6ca03-105">Retrieve a list of nameditem objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ca03-106">权限</span><span class="sxs-lookup"><span data-stu-id="6ca03-106">Permissions</span></span>
<span data-ttu-id="6ca03-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ca03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ca03-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ca03-109">Permission type</span></span>      | <span data-ttu-id="6ca03-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ca03-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ca03-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ca03-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6ca03-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ca03-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ca03-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ca03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ca03-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ca03-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ca03-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ca03-115">Application</span></span> | <span data-ttu-id="6ca03-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ca03-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ca03-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ca03-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ca03-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6ca03-118">Optional query parameters</span></span>
<span data-ttu-id="6ca03-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6ca03-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ca03-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ca03-120">Request headers</span></span>
| <span data-ttu-id="6ca03-121">名称</span><span class="sxs-lookup"><span data-stu-id="6ca03-121">Name</span></span>      |<span data-ttu-id="6ca03-122">说明</span><span class="sxs-lookup"><span data-stu-id="6ca03-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ca03-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ca03-123">Authorization</span></span>  | <span data-ttu-id="6ca03-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ca03-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ca03-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6ca03-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="6ca03-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6ca03-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ca03-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ca03-129">Request body</span></span>
<span data-ttu-id="6ca03-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ca03-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ca03-131">响应</span><span class="sxs-lookup"><span data-stu-id="6ca03-131">Response</span></span>

<span data-ttu-id="6ca03-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [workbookNamedItem](../resources/workbooknameditem.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6ca03-132">If successful, this method returns a `200 OK` response code and collection of [workbookNamedItem](../resources/workbooknameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ca03-133">示例</span><span class="sxs-lookup"><span data-stu-id="6ca03-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ca03-134">请求</span><span class="sxs-lookup"><span data-stu-id="6ca03-134">Request</span></span>
<span data-ttu-id="6ca03-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ca03-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ca03-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ca03-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_nameditemcollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names
```
# <a name="c"></a>[<span data-ttu-id="6ca03-137">C#</span><span class="sxs-lookup"><span data-stu-id="6ca03-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-nameditemcollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ca03-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ca03-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-nameditemcollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ca03-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ca03-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-nameditemcollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6ca03-140">响应</span><span class="sxs-lookup"><span data-stu-id="6ca03-140">Response</span></span>
<span data-ttu-id="6ca03-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ca03-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "value": [
    {
      "name": "name-value",
      "type": "type-value",
      "value": {
      },
      "visible": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List NamedItemCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
