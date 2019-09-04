---
title: 列出 RangeBorderCollection
description: 检索 rangeborder 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cb0492040c525257cc03f433803f160efda747f7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723229"
---
# <a name="list-rangebordercollection"></a><span data-ttu-id="d532a-103">列出 RangeBorderCollection</span><span class="sxs-lookup"><span data-stu-id="d532a-103">List RangeBorderCollection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d532a-104">检索 rangeborder 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d532a-104">Retrieve a list of rangeborder objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d532a-105">权限</span><span class="sxs-lookup"><span data-stu-id="d532a-105">Permissions</span></span>
<span data-ttu-id="d532a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d532a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d532a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d532a-108">Permission type</span></span>      | <span data-ttu-id="d532a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d532a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d532a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d532a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d532a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d532a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d532a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d532a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d532a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d532a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d532a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d532a-114">Application</span></span> | <span data-ttu-id="d532a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d532a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d532a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d532a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d532a-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d532a-117">Optional query parameters</span></span>
<span data-ttu-id="d532a-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d532a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d532a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d532a-119">Request headers</span></span>
| <span data-ttu-id="d532a-120">名称</span><span class="sxs-lookup"><span data-stu-id="d532a-120">Name</span></span>      |<span data-ttu-id="d532a-121">说明</span><span class="sxs-lookup"><span data-stu-id="d532a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d532a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d532a-122">Authorization</span></span>  | <span data-ttu-id="d532a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d532a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d532a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d532a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d532a-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d532a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d532a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d532a-128">Request body</span></span>
<span data-ttu-id="d532a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d532a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d532a-130">响应</span><span class="sxs-lookup"><span data-stu-id="d532a-130">Response</span></span>

<span data-ttu-id="d532a-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[workbookRangeBorder](../resources/workbookrangeborder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d532a-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeBorder](../resources/workbookrangeborder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d532a-132">示例</span><span class="sxs-lookup"><span data-stu-id="d532a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d532a-133">请求</span><span class="sxs-lookup"><span data-stu-id="d532a-133">Request</span></span>
<span data-ttu-id="d532a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d532a-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d532a-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d532a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rangebordercollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d532a-136">C#</span><span class="sxs-lookup"><span data-stu-id="d532a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rangebordercollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d532a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d532a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rangebordercollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d532a-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="d532a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rangebordercollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d532a-139">响应</span><span class="sxs-lookup"><span data-stu-id="d532a-139">Response</span></span>
<span data-ttu-id="d532a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d532a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 185

{
  "value": [
    {
      "id": "id-value",
      "color": "color-value",
      "style": "style-value",
      "sideIndex": "sideIndex-value",
      "weight": "weight-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List RangeBorderCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
