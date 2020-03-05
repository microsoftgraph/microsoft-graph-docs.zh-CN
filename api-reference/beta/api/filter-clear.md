---
title: 'Filter: clear'
description: 清除给定列上的筛选器。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 1f2a766167a629b976caadd7698884c794f2be68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421646"
---
# <a name="filter-clear"></a><span data-ttu-id="e56dd-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="e56dd-103">Filter: clear</span></span>

<span data-ttu-id="e56dd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e56dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e56dd-105">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="e56dd-105">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="e56dd-106">权限</span><span class="sxs-lookup"><span data-stu-id="e56dd-106">Permissions</span></span>
<span data-ttu-id="e56dd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e56dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e56dd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e56dd-109">Permission type</span></span>      | <span data-ttu-id="e56dd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e56dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e56dd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e56dd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e56dd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e56dd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e56dd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e56dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e56dd-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e56dd-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e56dd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e56dd-115">Application</span></span> | <span data-ttu-id="e56dd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e56dd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e56dd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e56dd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="e56dd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e56dd-118">Request headers</span></span>
| <span data-ttu-id="e56dd-119">名称</span><span class="sxs-lookup"><span data-stu-id="e56dd-119">Name</span></span>       | <span data-ttu-id="e56dd-120">说明</span><span class="sxs-lookup"><span data-stu-id="e56dd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e56dd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e56dd-121">Authorization</span></span>  | <span data-ttu-id="e56dd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e56dd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e56dd-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e56dd-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e56dd-125">响应</span><span class="sxs-lookup"><span data-stu-id="e56dd-125">Response</span></span>

<span data-ttu-id="e56dd-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e56dd-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e56dd-128">示例</span><span class="sxs-lookup"><span data-stu-id="e56dd-128">Example</span></span>
<span data-ttu-id="e56dd-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e56dd-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e56dd-130">请求</span><span class="sxs-lookup"><span data-stu-id="e56dd-130">Request</span></span>
<span data-ttu-id="e56dd-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e56dd-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e56dd-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e56dd-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="c"></a>[<span data-ttu-id="e56dd-133">C#</span><span class="sxs-lookup"><span data-stu-id="e56dd-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e56dd-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e56dd-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e56dd-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e56dd-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e56dd-136">响应</span><span class="sxs-lookup"><span data-stu-id="e56dd-136">Response</span></span>
<span data-ttu-id="e56dd-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e56dd-137">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
