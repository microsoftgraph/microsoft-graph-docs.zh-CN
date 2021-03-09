---
title: 'Filter: clear'
description: 清除给定列上的筛选器。
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: a55ea3342a98ead3082bda3c3ef8a0aaf669c794
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574081"
---
# <a name="filter-clear"></a><span data-ttu-id="11ae7-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="11ae7-103">Filter: clear</span></span>

<span data-ttu-id="11ae7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11ae7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11ae7-105">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="11ae7-105">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="11ae7-106">权限</span><span class="sxs-lookup"><span data-stu-id="11ae7-106">Permissions</span></span>
<span data-ttu-id="11ae7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11ae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11ae7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="11ae7-109">Permission type</span></span>      | <span data-ttu-id="11ae7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11ae7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11ae7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11ae7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11ae7-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11ae7-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="11ae7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11ae7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11ae7-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11ae7-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="11ae7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="11ae7-115">Application</span></span> | <span data-ttu-id="11ae7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="11ae7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11ae7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11ae7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="11ae7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="11ae7-118">Request headers</span></span>
| <span data-ttu-id="11ae7-119">名称</span><span class="sxs-lookup"><span data-stu-id="11ae7-119">Name</span></span>       | <span data-ttu-id="11ae7-120">说明</span><span class="sxs-lookup"><span data-stu-id="11ae7-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="11ae7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="11ae7-121">Authorization</span></span>  | <span data-ttu-id="11ae7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="11ae7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11ae7-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="11ae7-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="11ae7-125">响应</span><span class="sxs-lookup"><span data-stu-id="11ae7-125">Response</span></span>

<span data-ttu-id="11ae7-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="11ae7-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11ae7-128">示例</span><span class="sxs-lookup"><span data-stu-id="11ae7-128">Example</span></span>
<span data-ttu-id="11ae7-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="11ae7-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="11ae7-130">请求</span><span class="sxs-lookup"><span data-stu-id="11ae7-130">Request</span></span>
<span data-ttu-id="11ae7-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="11ae7-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11ae7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="11ae7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="c"></a>[<span data-ttu-id="11ae7-133">C#</span><span class="sxs-lookup"><span data-stu-id="11ae7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11ae7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11ae7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11ae7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11ae7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11ae7-136">Java</span><span class="sxs-lookup"><span data-stu-id="11ae7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="11ae7-137">响应</span><span class="sxs-lookup"><span data-stu-id="11ae7-137">Response</span></span>
<span data-ttu-id="11ae7-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="11ae7-138">Here is an example of the response.</span></span>
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


