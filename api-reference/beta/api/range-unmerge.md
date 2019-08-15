---
title: 'Range: unmerge'
description: 将范围单元格取消合并为各个单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ab6dcf840b1b5e3c0470e6c9d1eed12d889d40f1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412171"
---
# <a name="range-unmerge"></a><span data-ttu-id="a25ee-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="a25ee-103">Range: unmerge</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a25ee-104">将范围单元格取消合并为各个单元格。</span><span class="sxs-lookup"><span data-stu-id="a25ee-104">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="a25ee-105">权限</span><span class="sxs-lookup"><span data-stu-id="a25ee-105">Permissions</span></span>
<span data-ttu-id="a25ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a25ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a25ee-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a25ee-108">Permission type</span></span>      | <span data-ttu-id="a25ee-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a25ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a25ee-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a25ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a25ee-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a25ee-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a25ee-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a25ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a25ee-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a25ee-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a25ee-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a25ee-114">Application</span></span> | <span data-ttu-id="a25ee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a25ee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a25ee-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a25ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/unmerge
POST /workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="a25ee-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a25ee-117">Request headers</span></span>
| <span data-ttu-id="a25ee-118">名称</span><span class="sxs-lookup"><span data-stu-id="a25ee-118">Name</span></span>       | <span data-ttu-id="a25ee-119">说明</span><span class="sxs-lookup"><span data-stu-id="a25ee-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a25ee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a25ee-120">Authorization</span></span>  | <span data-ttu-id="a25ee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a25ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a25ee-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a25ee-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a25ee-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a25ee-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a25ee-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a25ee-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a25ee-127">响应</span><span class="sxs-lookup"><span data-stu-id="a25ee-127">Response</span></span>

<span data-ttu-id="a25ee-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a25ee-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a25ee-130">示例</span><span class="sxs-lookup"><span data-stu-id="a25ee-130">Example</span></span>
<span data-ttu-id="a25ee-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a25ee-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a25ee-132">请求</span><span class="sxs-lookup"><span data-stu-id="a25ee-132">Request</span></span>
<span data-ttu-id="a25ee-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a25ee-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a25ee-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a25ee-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/unmerge
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a25ee-135">C#</span><span class="sxs-lookup"><span data-stu-id="a25ee-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-unmerge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a25ee-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a25ee-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-unmerge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a25ee-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="a25ee-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-unmerge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a25ee-138">响应</span><span class="sxs-lookup"><span data-stu-id="a25ee-138">Response</span></span>
<span data-ttu-id="a25ee-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a25ee-139">Here is an example of the response.</span></span> 
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
  "description": "Range: unmerge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
