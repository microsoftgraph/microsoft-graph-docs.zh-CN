---
title: 创建图表
description: 使用此 API 创建新图表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: af852d0f1794906af3f95c55f4e0d7e054753f94
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055622"
---
# <a name="create-chart"></a><span data-ttu-id="45ddb-103">创建图表</span><span class="sxs-lookup"><span data-stu-id="45ddb-103">Create Chart</span></span>

<span data-ttu-id="45ddb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45ddb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45ddb-105">使用此 API 创建新图表。</span><span class="sxs-lookup"><span data-stu-id="45ddb-105">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="45ddb-106">权限</span><span class="sxs-lookup"><span data-stu-id="45ddb-106">Permissions</span></span>
<span data-ttu-id="45ddb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45ddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45ddb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45ddb-109">Permission type</span></span>      | <span data-ttu-id="45ddb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45ddb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45ddb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45ddb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45ddb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45ddb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="45ddb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45ddb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45ddb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45ddb-114">Not supported.</span></span>    |
|<span data-ttu-id="45ddb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45ddb-115">Application</span></span> | <span data-ttu-id="45ddb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="45ddb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45ddb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45ddb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="45ddb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="45ddb-118">Request headers</span></span>
| <span data-ttu-id="45ddb-119">名称</span><span class="sxs-lookup"><span data-stu-id="45ddb-119">Name</span></span>       | <span data-ttu-id="45ddb-120">说明</span><span class="sxs-lookup"><span data-stu-id="45ddb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="45ddb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45ddb-121">Authorization</span></span>  | <span data-ttu-id="45ddb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45ddb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45ddb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="45ddb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="45ddb-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="45ddb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45ddb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="45ddb-127">Request body</span></span>
<span data-ttu-id="45ddb-128">在请求正文中，提供 [WorkbookChart](../resources/chart.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45ddb-128">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="45ddb-129">响应</span><span class="sxs-lookup"><span data-stu-id="45ddb-129">Response</span></span>

<span data-ttu-id="45ddb-130">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [WorkbookChart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45ddb-130">If successful, this method returns `201 Created` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45ddb-131">示例</span><span class="sxs-lookup"><span data-stu-id="45ddb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45ddb-132">请求</span><span class="sxs-lookup"><span data-stu-id="45ddb-132">Request</span></span>
<span data-ttu-id="45ddb-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45ddb-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45ddb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="45ddb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
# <a name="c"></a>[<span data-ttu-id="45ddb-135">C#</span><span class="sxs-lookup"><span data-stu-id="45ddb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chart-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45ddb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45ddb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chart-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45ddb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45ddb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chart-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45ddb-138">Java</span><span class="sxs-lookup"><span data-stu-id="45ddb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chart-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="45ddb-139">在请求正文中，提供 [WorkbookChart](../resources/chart.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45ddb-139">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="45ddb-140">响应</span><span class="sxs-lookup"><span data-stu-id="45ddb-140">Response</span></span>
<span data-ttu-id="45ddb-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="45ddb-141">Here is an example of the response.</span></span> <span data-ttu-id="45ddb-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="45ddb-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

