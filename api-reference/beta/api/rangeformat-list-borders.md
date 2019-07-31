---
title: 列出边框
description: 检索 rangeborder 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ae1708ef0d1e1ffdb795d072f332431bb142d07a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978263"
---
# <a name="list-borders"></a><span data-ttu-id="f7951-103">列出边框</span><span class="sxs-lookup"><span data-stu-id="f7951-103">List borders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7951-104">检索 rangeborder 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f7951-104">Retrieve a list of rangeborder objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7951-105">权限</span><span class="sxs-lookup"><span data-stu-id="f7951-105">Permissions</span></span>
<span data-ttu-id="f7951-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7951-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7951-108">Permission type</span></span>      | <span data-ttu-id="f7951-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7951-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7951-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7951-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7951-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7951-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7951-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7951-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7951-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7951-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7951-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7951-114">Application</span></span> | <span data-ttu-id="f7951-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7951-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7951-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7951-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7951-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f7951-117">Optional query parameters</span></span>
<span data-ttu-id="f7951-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f7951-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7951-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7951-119">Request headers</span></span>
| <span data-ttu-id="f7951-120">名称</span><span class="sxs-lookup"><span data-stu-id="f7951-120">Name</span></span>      |<span data-ttu-id="f7951-121">说明</span><span class="sxs-lookup"><span data-stu-id="f7951-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7951-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7951-122">Authorization</span></span>  | <span data-ttu-id="f7951-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7951-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7951-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f7951-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f7951-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f7951-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7951-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7951-128">Request body</span></span>
<span data-ttu-id="f7951-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7951-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7951-130">响应</span><span class="sxs-lookup"><span data-stu-id="f7951-130">Response</span></span>

<span data-ttu-id="f7951-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[workbookRangeBorder](../resources/workbookrangeborder.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f7951-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeBorder](../resources/workbookrangeborder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7951-132">示例</span><span class="sxs-lookup"><span data-stu-id="f7951-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7951-133">请求</span><span class="sxs-lookup"><span data-stu-id="f7951-133">Request</span></span>
<span data-ttu-id="f7951-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7951-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f7951-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f7951-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_borders"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7951-136">C#</span><span class="sxs-lookup"><span data-stu-id="f7951-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-borders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7951-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7951-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-borders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7951-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="f7951-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-borders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f7951-139">Java</span><span class="sxs-lookup"><span data-stu-id="f7951-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-borders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f7951-140">响应</span><span class="sxs-lookup"><span data-stu-id="f7951-140">Response</span></span>
<span data-ttu-id="f7951-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7951-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List borders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
