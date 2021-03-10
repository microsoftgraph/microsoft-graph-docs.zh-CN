---
title: 创建 ChartPoints
description: 使用此 API 创建新 ChartPoints。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 35dc6925c71fcdf40adfef6bf2941f31e4abb042
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573703"
---
# <a name="create-chartpoints"></a><span data-ttu-id="d2330-103">创建 ChartPoints</span><span class="sxs-lookup"><span data-stu-id="d2330-103">Create ChartPoints</span></span>

<span data-ttu-id="d2330-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2330-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2330-105">使用此 API 创建新 ChartPoints。</span><span class="sxs-lookup"><span data-stu-id="d2330-105">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2330-106">权限</span><span class="sxs-lookup"><span data-stu-id="d2330-106">Permissions</span></span>
<span data-ttu-id="d2330-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2330-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2330-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2330-109">Permission type</span></span>      | <span data-ttu-id="d2330-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2330-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2330-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2330-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d2330-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2330-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2330-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2330-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2330-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2330-114">Not supported.</span></span>    |
|<span data-ttu-id="d2330-115">Application</span><span class="sxs-lookup"><span data-stu-id="d2330-115">Application</span></span> | <span data-ttu-id="d2330-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2330-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2330-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2330-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points

```
## <a name="request-headers"></a><span data-ttu-id="d2330-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2330-118">Request headers</span></span>
| <span data-ttu-id="d2330-119">名称</span><span class="sxs-lookup"><span data-stu-id="d2330-119">Name</span></span>       | <span data-ttu-id="d2330-120">说明</span><span class="sxs-lookup"><span data-stu-id="d2330-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d2330-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2330-121">Authorization</span></span>  | <span data-ttu-id="d2330-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2330-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2330-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d2330-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d2330-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d2330-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2330-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2330-127">Request body</span></span>
<span data-ttu-id="d2330-128">在请求正文中，提供 [ChartPoints](../resources/chartpoint.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2330-128">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d2330-129">响应</span><span class="sxs-lookup"><span data-stu-id="d2330-129">Response</span></span>

<span data-ttu-id="d2330-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ChartPoints](../resources/chartpoint.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2330-130">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2330-131">示例</span><span class="sxs-lookup"><span data-stu-id="d2330-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2330-132">请求</span><span class="sxs-lookup"><span data-stu-id="d2330-132">Request</span></span>
<span data-ttu-id="d2330-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2330-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2330-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2330-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points
Content-type: application/json
Content-length: 3

{
}
```
# <a name="c"></a>[<span data-ttu-id="d2330-135">C#</span><span class="sxs-lookup"><span data-stu-id="d2330-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartpoints-from-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2330-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2330-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartpoints-from-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2330-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2330-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartpoints-from-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2330-138">Java</span><span class="sxs-lookup"><span data-stu-id="d2330-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chartpoints-from-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d2330-139">在请求正文中，提供 [ChartPoints](../resources/chartpoint.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2330-139">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d2330-140">响应</span><span class="sxs-lookup"><span data-stu-id="d2330-140">Response</span></span>
<span data-ttu-id="d2330-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2330-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

