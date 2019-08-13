---
title: 创建图表
description: 使用此 API 创建新图表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c30b16f4628a95e8f0c81e9ddd40afc6acc52e4f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361847"
---
# <a name="create-chart"></a><span data-ttu-id="cfeab-103">创建图表</span><span class="sxs-lookup"><span data-stu-id="cfeab-103">Create Chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfeab-104">使用此 API 创建新图表。</span><span class="sxs-lookup"><span data-stu-id="cfeab-104">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="cfeab-105">权限</span><span class="sxs-lookup"><span data-stu-id="cfeab-105">Permissions</span></span>
<span data-ttu-id="cfeab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfeab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfeab-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfeab-108">Permission type</span></span>      | <span data-ttu-id="cfeab-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfeab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfeab-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfeab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cfeab-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfeab-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cfeab-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfeab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfeab-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfeab-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cfeab-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfeab-114">Application</span></span> | <span data-ttu-id="cfeab-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfeab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfeab-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfeab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="cfeab-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfeab-117">Request headers</span></span>
| <span data-ttu-id="cfeab-118">名称</span><span class="sxs-lookup"><span data-stu-id="cfeab-118">Name</span></span>       | <span data-ttu-id="cfeab-119">说明</span><span class="sxs-lookup"><span data-stu-id="cfeab-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cfeab-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfeab-120">Authorization</span></span>  | <span data-ttu-id="cfeab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfeab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cfeab-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cfeab-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cfeab-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="cfeab-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfeab-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfeab-126">Request body</span></span>
<span data-ttu-id="cfeab-127">在请求正文中, 提供[workbookChart](../resources/workbookchart.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfeab-127">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cfeab-128">响应</span><span class="sxs-lookup"><span data-stu-id="cfeab-128">Response</span></span>

<span data-ttu-id="cfeab-129">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[workbookChart](../resources/workbookchart.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cfeab-129">If successful, this method returns `201 Created` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfeab-130">示例</span><span class="sxs-lookup"><span data-stu-id="cfeab-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfeab-131">请求</span><span class="sxs-lookup"><span data-stu-id="cfeab-131">Request</span></span>
<span data-ttu-id="cfeab-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cfeab-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cfeab-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="cfeab-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="cfeab-134">C#</span><span class="sxs-lookup"><span data-stu-id="cfeab-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chart-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfeab-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfeab-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chart-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cfeab-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="cfeab-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chart-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cfeab-137">Java</span><span class="sxs-lookup"><span data-stu-id="cfeab-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chart-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="cfeab-138">在请求正文中, 提供[workbookChart](../resources/workbookchart.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfeab-138">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cfeab-139">响应</span><span class="sxs-lookup"><span data-stu-id="cfeab-139">Response</span></span>
<span data-ttu-id="cfeab-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cfeab-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
