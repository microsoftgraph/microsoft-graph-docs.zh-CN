---
title: 'TableSort: clear'
description: 清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f202c378ddf774fc2bae2400983a598d2f3a8918
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982506"
---
# <a name="tablesort-clear"></a><span data-ttu-id="f2b87-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="f2b87-104">TableSort: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2b87-p102">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="f2b87-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2b87-107">权限</span><span class="sxs-lookup"><span data-stu-id="f2b87-107">Permissions</span></span>
<span data-ttu-id="f2b87-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2b87-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2b87-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2b87-110">Permission type</span></span>      | <span data-ttu-id="f2b87-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2b87-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2b87-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b87-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2b87-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2b87-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f2b87-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b87-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2b87-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2b87-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f2b87-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2b87-116">Application</span></span> | <span data-ttu-id="f2b87-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2b87-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2b87-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2b87-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="f2b87-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2b87-119">Request headers</span></span>
| <span data-ttu-id="f2b87-120">名称</span><span class="sxs-lookup"><span data-stu-id="f2b87-120">Name</span></span>       | <span data-ttu-id="f2b87-121">说明</span><span class="sxs-lookup"><span data-stu-id="f2b87-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f2b87-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2b87-122">Authorization</span></span>  | <span data-ttu-id="f2b87-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2b87-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2b87-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f2b87-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f2b87-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f2b87-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2b87-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2b87-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f2b87-129">响应</span><span class="sxs-lookup"><span data-stu-id="f2b87-129">Response</span></span>

<span data-ttu-id="f2b87-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f2b87-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2b87-132">示例</span><span class="sxs-lookup"><span data-stu-id="f2b87-132">Example</span></span>
<span data-ttu-id="f2b87-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f2b87-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f2b87-134">请求</span><span class="sxs-lookup"><span data-stu-id="f2b87-134">Request</span></span>
<span data-ttu-id="f2b87-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2b87-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f2b87-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f2b87-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f2b87-137">C#</span><span class="sxs-lookup"><span data-stu-id="f2b87-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2b87-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="f2b87-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f2b87-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="f2b87-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f2b87-140">Java</span><span class="sxs-lookup"><span data-stu-id="f2b87-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f2b87-141">响应</span><span class="sxs-lookup"><span data-stu-id="f2b87-141">Response</span></span>
<span data-ttu-id="f2b87-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f2b87-142">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
