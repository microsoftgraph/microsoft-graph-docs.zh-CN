---
title: 'Table: clearFilters'
description: 清除当前表上应用的所有筛选器。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7d8a2190d34f51fe1321c5a85647299992881770
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452891"
---
# <a name="table-clearfilters"></a><span data-ttu-id="3af50-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="3af50-103">Table: clearFilters</span></span>

<span data-ttu-id="3af50-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3af50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3af50-105">清除当前表上应用的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="3af50-105">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="3af50-106">权限</span><span class="sxs-lookup"><span data-stu-id="3af50-106">Permissions</span></span>
<span data-ttu-id="3af50-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3af50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3af50-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3af50-109">Permission type</span></span>      | <span data-ttu-id="3af50-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3af50-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3af50-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3af50-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3af50-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3af50-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3af50-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3af50-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3af50-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3af50-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3af50-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3af50-115">Application</span></span> | <span data-ttu-id="3af50-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3af50-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3af50-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3af50-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="3af50-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3af50-118">Request headers</span></span>
| <span data-ttu-id="3af50-119">名称</span><span class="sxs-lookup"><span data-stu-id="3af50-119">Name</span></span>       | <span data-ttu-id="3af50-120">说明</span><span class="sxs-lookup"><span data-stu-id="3af50-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3af50-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3af50-121">Authorization</span></span>  | <span data-ttu-id="3af50-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3af50-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3af50-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3af50-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3af50-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="3af50-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3af50-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3af50-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3af50-128">响应</span><span class="sxs-lookup"><span data-stu-id="3af50-128">Response</span></span>

<span data-ttu-id="3af50-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3af50-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3af50-131">示例</span><span class="sxs-lookup"><span data-stu-id="3af50-131">Example</span></span>
<span data-ttu-id="3af50-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="3af50-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3af50-133">请求</span><span class="sxs-lookup"><span data-stu-id="3af50-133">Request</span></span>
<span data-ttu-id="3af50-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3af50-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3af50-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3af50-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```
# <a name="c"></a>[<span data-ttu-id="3af50-136">C#</span><span class="sxs-lookup"><span data-stu-id="3af50-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-clearfilters-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3af50-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3af50-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-clearfilters-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3af50-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3af50-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-clearfilters-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3af50-139">响应</span><span class="sxs-lookup"><span data-stu-id="3af50-139">Response</span></span>
<span data-ttu-id="3af50-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3af50-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
