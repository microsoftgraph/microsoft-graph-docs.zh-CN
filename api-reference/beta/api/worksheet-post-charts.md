---
title: 创建图表
description: 使用此 API 创建新图表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e1c11cfc8c5c0876a01719c230ff03e1666396e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024687"
---
# <a name="create-chart"></a><span data-ttu-id="381fd-103">创建图表</span><span class="sxs-lookup"><span data-stu-id="381fd-103">Create Chart</span></span>

<span data-ttu-id="381fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="381fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="381fd-105">使用此 API 创建新图表。</span><span class="sxs-lookup"><span data-stu-id="381fd-105">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="381fd-106">权限</span><span class="sxs-lookup"><span data-stu-id="381fd-106">Permissions</span></span>
<span data-ttu-id="381fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="381fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="381fd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="381fd-109">Permission type</span></span>      | <span data-ttu-id="381fd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="381fd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="381fd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="381fd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="381fd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="381fd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="381fd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="381fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="381fd-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="381fd-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="381fd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="381fd-115">Application</span></span> | <span data-ttu-id="381fd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="381fd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="381fd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="381fd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="381fd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="381fd-118">Request headers</span></span>
| <span data-ttu-id="381fd-119">名称</span><span class="sxs-lookup"><span data-stu-id="381fd-119">Name</span></span>       | <span data-ttu-id="381fd-120">说明</span><span class="sxs-lookup"><span data-stu-id="381fd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="381fd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="381fd-121">Authorization</span></span>  | <span data-ttu-id="381fd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="381fd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="381fd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="381fd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="381fd-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="381fd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="381fd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="381fd-127">Request body</span></span>
<span data-ttu-id="381fd-128">在请求正文中，提供 [workbookChart](../resources/workbookchart.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="381fd-128">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="381fd-129">响应</span><span class="sxs-lookup"><span data-stu-id="381fd-129">Response</span></span>

<span data-ttu-id="381fd-130">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [workbookChart](../resources/workbookchart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="381fd-130">If successful, this method returns `201 Created` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="381fd-131">示例</span><span class="sxs-lookup"><span data-stu-id="381fd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="381fd-132">请求</span><span class="sxs-lookup"><span data-stu-id="381fd-132">Request</span></span>
<span data-ttu-id="381fd-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="381fd-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="381fd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="381fd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
# <a name="c"></a>[<span data-ttu-id="381fd-135">C#</span><span class="sxs-lookup"><span data-stu-id="381fd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chart-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="381fd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="381fd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chart-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="381fd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="381fd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chart-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="381fd-138">在请求正文中，提供 [workbookChart](../resources/workbookchart.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="381fd-138">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="381fd-139">响应</span><span class="sxs-lookup"><span data-stu-id="381fd-139">Response</span></span>
<span data-ttu-id="381fd-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="381fd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


