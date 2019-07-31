---
title: 'TableRowCollection: ItemAt'
description: 根据其在集合中的位置获取行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bd5dbcfe4bd804589f3768218dd357cc4b1c3406
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990874"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="f71bc-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="f71bc-103">TableRowCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f71bc-104">根据其在集合中的位置获取行。</span><span class="sxs-lookup"><span data-stu-id="f71bc-104">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="f71bc-105">权限</span><span class="sxs-lookup"><span data-stu-id="f71bc-105">Permissions</span></span>
<span data-ttu-id="f71bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f71bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f71bc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f71bc-108">Permission type</span></span>      | <span data-ttu-id="f71bc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f71bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f71bc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f71bc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f71bc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f71bc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f71bc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f71bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f71bc-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f71bc-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f71bc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f71bc-114">Application</span></span> | <span data-ttu-id="f71bc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f71bc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f71bc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f71bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="f71bc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f71bc-117">Request headers</span></span>
| <span data-ttu-id="f71bc-118">名称</span><span class="sxs-lookup"><span data-stu-id="f71bc-118">Name</span></span>       | <span data-ttu-id="f71bc-119">说明</span><span class="sxs-lookup"><span data-stu-id="f71bc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f71bc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f71bc-120">Authorization</span></span>  | <span data-ttu-id="f71bc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f71bc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f71bc-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f71bc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f71bc-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f71bc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f71bc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f71bc-126">Request body</span></span>
<span data-ttu-id="f71bc-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f71bc-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f71bc-128">参数</span><span class="sxs-lookup"><span data-stu-id="f71bc-128">Parameter</span></span>    | <span data-ttu-id="f71bc-129">类型</span><span class="sxs-lookup"><span data-stu-id="f71bc-129">Type</span></span>   |<span data-ttu-id="f71bc-130">说明</span><span class="sxs-lookup"><span data-stu-id="f71bc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f71bc-131">index</span><span class="sxs-lookup"><span data-stu-id="f71bc-131">index</span></span>|<span data-ttu-id="f71bc-132">number</span><span class="sxs-lookup"><span data-stu-id="f71bc-132">number</span></span>|<span data-ttu-id="f71bc-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="f71bc-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="f71bc-135">响应</span><span class="sxs-lookup"><span data-stu-id="f71bc-135">Response</span></span>

<span data-ttu-id="f71bc-136">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[workbookTableRow](../resources/workbooktablerow.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f71bc-136">If successful, this method returns `200 OK` response code and [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f71bc-137">示例</span><span class="sxs-lookup"><span data-stu-id="f71bc-137">Example</span></span>
<span data-ttu-id="f71bc-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f71bc-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f71bc-139">请求</span><span class="sxs-lookup"><span data-stu-id="f71bc-139">Request</span></span>
<span data-ttu-id="f71bc-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f71bc-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f71bc-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f71bc-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f71bc-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="f71bc-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f71bc-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="f71bc-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerowcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f71bc-144">响应</span><span class="sxs-lookup"><span data-stu-id="f71bc-144">Response</span></span>
<span data-ttu-id="f71bc-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f71bc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
