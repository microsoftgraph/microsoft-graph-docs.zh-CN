---
title: Table:DataBodyRange
description: 获取与表的数据体相关的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 61473a8bec62188e251c75233fdb073bee333e7d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576636"
---
# <a name="table-databodyrange"></a><span data-ttu-id="a403c-103">Table:DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="a403c-103">Table: DataBodyRange</span></span>

<span data-ttu-id="a403c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a403c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a403c-105">获取与表的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="a403c-105">Gets the range object associated with the data body of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="a403c-106">权限</span><span class="sxs-lookup"><span data-stu-id="a403c-106">Permissions</span></span>
<span data-ttu-id="a403c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a403c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a403c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a403c-109">Permission type</span></span>      | <span data-ttu-id="a403c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a403c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a403c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a403c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a403c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a403c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a403c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a403c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a403c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a403c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a403c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a403c-115">Application</span></span> | <span data-ttu-id="a403c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a403c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a403c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a403c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/DataBodyRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/DataBodyRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/DataBodyRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/DataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="a403c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a403c-118">Request headers</span></span>
| <span data-ttu-id="a403c-119">名称</span><span class="sxs-lookup"><span data-stu-id="a403c-119">Name</span></span>       | <span data-ttu-id="a403c-120">说明</span><span class="sxs-lookup"><span data-stu-id="a403c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a403c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a403c-121">Authorization</span></span>  | <span data-ttu-id="a403c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a403c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a403c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a403c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a403c-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a403c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a403c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a403c-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a403c-128">响应</span><span class="sxs-lookup"><span data-stu-id="a403c-128">Response</span></span>

<span data-ttu-id="a403c-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a403c-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a403c-130">示例</span><span class="sxs-lookup"><span data-stu-id="a403c-130">Example</span></span>
<span data-ttu-id="a403c-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a403c-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a403c-132">请求</span><span class="sxs-lookup"><span data-stu-id="a403c-132">Request</span></span>
<span data-ttu-id="a403c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a403c-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a403c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a403c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_databodyrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/DataBodyRange
```
# <a name="c"></a>[<span data-ttu-id="a403c-135">C#</span><span class="sxs-lookup"><span data-stu-id="a403c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-databodyrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a403c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a403c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-databodyrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a403c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a403c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-databodyrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a403c-138">Java</span><span class="sxs-lookup"><span data-stu-id="a403c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-databodyrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a403c-139">响应</span><span class="sxs-lookup"><span data-stu-id="a403c-139">Response</span></span>
<span data-ttu-id="a403c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a403c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


