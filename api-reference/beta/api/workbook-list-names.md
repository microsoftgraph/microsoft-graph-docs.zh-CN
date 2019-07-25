---
title: 列出名称
description: 检索 nameditem 对象的列表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b14c8ca4ad0971133b025d7e3fef675d2e2b8c39
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866592"
---
# <a name="list-names"></a><span data-ttu-id="3d967-103">列出名称</span><span class="sxs-lookup"><span data-stu-id="3d967-103">List names</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d967-104">检索 nameditem 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3d967-104">Retrieve a list of nameditem objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="3d967-105">权限</span><span class="sxs-lookup"><span data-stu-id="3d967-105">Permissions</span></span>
<span data-ttu-id="3d967-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d967-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d967-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d967-108">Permission type</span></span>      | <span data-ttu-id="3d967-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3d967-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d967-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d967-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d967-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d967-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3d967-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d967-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d967-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d967-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3d967-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d967-114">Application</span></span> | <span data-ttu-id="3d967-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d967-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d967-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d967-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3d967-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3d967-117">Optional query parameters</span></span>
<span data-ttu-id="3d967-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3d967-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d967-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d967-119">Request headers</span></span>
| <span data-ttu-id="3d967-120">名称</span><span class="sxs-lookup"><span data-stu-id="3d967-120">Name</span></span>      |<span data-ttu-id="3d967-121">说明</span><span class="sxs-lookup"><span data-stu-id="3d967-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3d967-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d967-122">Authorization</span></span>  | <span data-ttu-id="3d967-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3d967-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d967-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3d967-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3d967-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="3d967-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d967-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d967-128">Request body</span></span>
<span data-ttu-id="3d967-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3d967-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d967-130">响应</span><span class="sxs-lookup"><span data-stu-id="3d967-130">Response</span></span>

<span data-ttu-id="3d967-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[workbookNamedItem](../resources/workbooknameditem.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="3d967-131">If successful, this method returns a `200 OK` response code and collection of [workbookNamedItem](../resources/workbooknameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d967-132">示例</span><span class="sxs-lookup"><span data-stu-id="3d967-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d967-133">请求</span><span class="sxs-lookup"><span data-stu-id="3d967-133">Request</span></span>
<span data-ttu-id="3d967-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d967-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3d967-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3d967-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3d967-136">C#</span><span class="sxs-lookup"><span data-stu-id="3d967-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-names-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d967-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d967-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-names-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3d967-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="3d967-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-names-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3d967-139">Java</span><span class="sxs-lookup"><span data-stu-id="3d967-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-names-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3d967-140">响应</span><span class="sxs-lookup"><span data-stu-id="3d967-140">Response</span></span>
<span data-ttu-id="3d967-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d967-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List names",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
