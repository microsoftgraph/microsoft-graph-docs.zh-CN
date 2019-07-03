---
title: 'Filter: clear'
description: 清除给定列上的筛选器。
localization_priority: Normal
ms.openlocfilehash: 2bc1d1f607f062ca7566189d184f37bc74ab09df
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440860"
---
# <a name="filter-clear"></a><span data-ttu-id="8fcc1-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="8fcc1-103">Filter: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fcc1-104">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="8fcc1-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="8fcc1-105">权限</span><span class="sxs-lookup"><span data-stu-id="8fcc1-105">Permissions</span></span>
<span data-ttu-id="8fcc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8fcc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fcc1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8fcc1-108">Permission type</span></span>      | <span data-ttu-id="8fcc1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8fcc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fcc1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8fcc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8fcc1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8fcc1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8fcc1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8fcc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fcc1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8fcc1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8fcc1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8fcc1-114">Application</span></span> | <span data-ttu-id="8fcc1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fcc1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fcc1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8fcc1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="8fcc1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8fcc1-117">Request headers</span></span>
| <span data-ttu-id="8fcc1-118">名称</span><span class="sxs-lookup"><span data-stu-id="8fcc1-118">Name</span></span>       | <span data-ttu-id="8fcc1-119">说明</span><span class="sxs-lookup"><span data-stu-id="8fcc1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8fcc1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fcc1-120">Authorization</span></span>  | <span data-ttu-id="8fcc1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8fcc1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fcc1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8fcc1-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8fcc1-124">响应</span><span class="sxs-lookup"><span data-stu-id="8fcc1-124">Response</span></span>

<span data-ttu-id="8fcc1-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8fcc1-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fcc1-127">示例</span><span class="sxs-lookup"><span data-stu-id="8fcc1-127">Example</span></span>
<span data-ttu-id="8fcc1-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8fcc1-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8fcc1-129">请求</span><span class="sxs-lookup"><span data-stu-id="8fcc1-129">Request</span></span>
<span data-ttu-id="8fcc1-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8fcc1-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8fcc1-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8fcc1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8fcc1-132">C#</span><span class="sxs-lookup"><span data-stu-id="8fcc1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8fcc1-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="8fcc1-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8fcc1-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="8fcc1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8fcc1-135">响应</span><span class="sxs-lookup"><span data-stu-id="8fcc1-135">Response</span></span>
<span data-ttu-id="8fcc1-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8fcc1-136">Here is an example of the response.</span></span> 
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
