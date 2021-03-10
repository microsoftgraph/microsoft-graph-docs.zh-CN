---
title: 创建 RangeBorder
description: 使用此 API 创建新 RangeBorder。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a96efc8519e8e3a2247c06234ff389c818712bd8
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577210"
---
# <a name="create-rangeborder"></a><span data-ttu-id="0a124-103">创建 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="0a124-103">Create RangeBorder</span></span>

<span data-ttu-id="0a124-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a124-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0a124-105">使用此 API 创建新 RangeBorder。</span><span class="sxs-lookup"><span data-stu-id="0a124-105">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a124-106">权限</span><span class="sxs-lookup"><span data-stu-id="0a124-106">Permissions</span></span>
<span data-ttu-id="0a124-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a124-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a124-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a124-109">Permission type</span></span>      | <span data-ttu-id="0a124-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a124-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a124-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a124-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0a124-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a124-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a124-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a124-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a124-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a124-114">Not supported.</span></span>    |
|<span data-ttu-id="0a124-115">Application</span><span class="sxs-lookup"><span data-stu-id="0a124-115">Application</span></span> | <span data-ttu-id="0a124-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a124-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a124-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a124-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/format/borders
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/borders
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/borders
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="0a124-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a124-118">Request headers</span></span>
| <span data-ttu-id="0a124-119">名称</span><span class="sxs-lookup"><span data-stu-id="0a124-119">Name</span></span>       | <span data-ttu-id="0a124-120">说明</span><span class="sxs-lookup"><span data-stu-id="0a124-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0a124-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a124-121">Authorization</span></span>  | <span data-ttu-id="0a124-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a124-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a124-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0a124-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0a124-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0a124-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a124-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a124-127">Request body</span></span>
<span data-ttu-id="0a124-128">在请求正文中，提供 [WorkbookRangeBorder](../resources/rangeborder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a124-128">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0a124-129">响应</span><span class="sxs-lookup"><span data-stu-id="0a124-129">Response</span></span>

<span data-ttu-id="0a124-130">如果成功，此方法在 `201 Created` 响应正文中返回响应代码和 [WorkbookRangeBorder](../resources/rangeborder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0a124-130">If successful, this method returns `201 Created` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a124-131">示例</span><span class="sxs-lookup"><span data-stu-id="0a124-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a124-132">请求</span><span class="sxs-lookup"><span data-stu-id="0a124-132">Request</span></span>
<span data-ttu-id="0a124-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a124-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a124-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a124-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
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
# <a name="c"></a>[<span data-ttu-id="0a124-135">C#</span><span class="sxs-lookup"><span data-stu-id="0a124-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rangeborder-from-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a124-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a124-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rangeborder-from-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a124-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a124-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rangeborder-from-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a124-138">Java</span><span class="sxs-lookup"><span data-stu-id="0a124-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rangeborder-from-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0a124-139">在请求正文中，提供 [WorkbookRangeBorder](../resources/rangeborder.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a124-139">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0a124-140">响应</span><span class="sxs-lookup"><span data-stu-id="0a124-140">Response</span></span>
<span data-ttu-id="0a124-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a124-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

