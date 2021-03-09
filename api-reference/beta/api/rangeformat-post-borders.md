---
title: 创建 RangeBorder
description: 使用此 API 创建新 RangeBorder。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1c9d7eb22a11710b41d64c3284e4fd72789d8e4b
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577357"
---
# <a name="create-rangeborder"></a><span data-ttu-id="f47fd-103">创建 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="f47fd-103">Create RangeBorder</span></span>

<span data-ttu-id="f47fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f47fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f47fd-105">使用此 API 创建新 RangeBorder。</span><span class="sxs-lookup"><span data-stu-id="f47fd-105">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="f47fd-106">权限</span><span class="sxs-lookup"><span data-stu-id="f47fd-106">Permissions</span></span>
<span data-ttu-id="f47fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f47fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f47fd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f47fd-109">Permission type</span></span>      | <span data-ttu-id="f47fd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f47fd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f47fd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f47fd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f47fd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f47fd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f47fd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f47fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f47fd-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f47fd-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f47fd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f47fd-115">Application</span></span> | <span data-ttu-id="f47fd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f47fd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f47fd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f47fd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/format/borders
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/borders
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/borders
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="f47fd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f47fd-118">Request headers</span></span>
| <span data-ttu-id="f47fd-119">名称</span><span class="sxs-lookup"><span data-stu-id="f47fd-119">Name</span></span>       | <span data-ttu-id="f47fd-120">说明</span><span class="sxs-lookup"><span data-stu-id="f47fd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f47fd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f47fd-121">Authorization</span></span>  | <span data-ttu-id="f47fd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f47fd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f47fd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f47fd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f47fd-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f47fd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f47fd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f47fd-127">Request body</span></span>
<span data-ttu-id="f47fd-128">在请求正文中，提供 [workbookRangeBorder](../resources/workbookrangeborder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f47fd-128">In the request body, supply a JSON representation of [workbookRangeBorder](../resources/workbookrangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f47fd-129">响应</span><span class="sxs-lookup"><span data-stu-id="f47fd-129">Response</span></span>

<span data-ttu-id="f47fd-130">如果成功，此方法在 `201 Created` 响应正文中返回响应代码和 [workbookRangeBorder](../resources/workbookrangeborder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f47fd-130">If successful, this method returns `201 Created` response code and [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f47fd-131">示例</span><span class="sxs-lookup"><span data-stu-id="f47fd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f47fd-132">请求</span><span class="sxs-lookup"><span data-stu-id="f47fd-132">Request</span></span>
<span data-ttu-id="f47fd-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f47fd-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f47fd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f47fd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
# <a name="c"></a>[<span data-ttu-id="f47fd-135">C#</span><span class="sxs-lookup"><span data-stu-id="f47fd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rangeborder-from-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f47fd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f47fd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rangeborder-from-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f47fd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f47fd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rangeborder-from-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f47fd-138">Java</span><span class="sxs-lookup"><span data-stu-id="f47fd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rangeborder-from-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f47fd-139">在请求正文中，提供 [workbookRangeBorder](../resources/workbookrangeborder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f47fd-139">In the request body, supply a JSON representation of [workbookRangeBorder](../resources/workbookrangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f47fd-140">响应</span><span class="sxs-lookup"><span data-stu-id="f47fd-140">Response</span></span>
<span data-ttu-id="f47fd-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f47fd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


