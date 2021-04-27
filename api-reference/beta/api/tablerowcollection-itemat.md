---
title: 'TableRowCollection: ItemAt'
description: 根据其在集合中的位置获取行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1fcb87a1422b28c8f086dc619076dba6ddd578c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054782"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="155d5-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="155d5-103">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="155d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="155d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="155d5-105">根据其在集合中的位置获取行。</span><span class="sxs-lookup"><span data-stu-id="155d5-105">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="155d5-106">权限</span><span class="sxs-lookup"><span data-stu-id="155d5-106">Permissions</span></span>
<span data-ttu-id="155d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="155d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="155d5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="155d5-109">Permission type</span></span>      | <span data-ttu-id="155d5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="155d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="155d5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="155d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="155d5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="155d5-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="155d5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="155d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="155d5-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="155d5-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="155d5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="155d5-115">Application</span></span> | <span data-ttu-id="155d5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="155d5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="155d5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="155d5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/ItemAt
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/ItemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="155d5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="155d5-118">Request headers</span></span>
| <span data-ttu-id="155d5-119">名称</span><span class="sxs-lookup"><span data-stu-id="155d5-119">Name</span></span>       | <span data-ttu-id="155d5-120">说明</span><span class="sxs-lookup"><span data-stu-id="155d5-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="155d5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="155d5-121">Authorization</span></span>  | <span data-ttu-id="155d5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="155d5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="155d5-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="155d5-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="155d5-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="155d5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="155d5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="155d5-127">Request body</span></span>
<span data-ttu-id="155d5-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="155d5-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="155d5-129">参数</span><span class="sxs-lookup"><span data-stu-id="155d5-129">Parameter</span></span>    | <span data-ttu-id="155d5-130">类型</span><span class="sxs-lookup"><span data-stu-id="155d5-130">Type</span></span>   |<span data-ttu-id="155d5-131">说明</span><span class="sxs-lookup"><span data-stu-id="155d5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="155d5-132">index</span><span class="sxs-lookup"><span data-stu-id="155d5-132">index</span></span>|<span data-ttu-id="155d5-133">number</span><span class="sxs-lookup"><span data-stu-id="155d5-133">number</span></span>|<span data-ttu-id="155d5-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="155d5-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="155d5-136">响应</span><span class="sxs-lookup"><span data-stu-id="155d5-136">Response</span></span>

<span data-ttu-id="155d5-137">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [workbookTableRow](../resources/workbooktablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="155d5-137">If successful, this method returns `200 OK` response code and [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="155d5-138">示例</span><span class="sxs-lookup"><span data-stu-id="155d5-138">Example</span></span>
<span data-ttu-id="155d5-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="155d5-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="155d5-140">请求</span><span class="sxs-lookup"><span data-stu-id="155d5-140">Request</span></span>
<span data-ttu-id="155d5-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="155d5-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="155d5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="155d5-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="155d5-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="155d5-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="155d5-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="155d5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerowcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="155d5-145">响应</span><span class="sxs-lookup"><span data-stu-id="155d5-145">Response</span></span>
<span data-ttu-id="155d5-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="155d5-146">Here is an example of the response.</span></span> <span data-ttu-id="155d5-147">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="155d5-147">Note: The response object shown here might be shortened for readability.</span></span>
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


