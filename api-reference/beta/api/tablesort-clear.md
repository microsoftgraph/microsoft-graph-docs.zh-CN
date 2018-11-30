---
title: 'TableSort: clear'
description: 清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。
ms.openlocfilehash: f93b640188faedc228c56b6e13497ade84190765
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048349"
---
# <a name="tablesort-clear"></a><span data-ttu-id="913fa-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="913fa-104">TableSort: clear</span></span>

> <span data-ttu-id="913fa-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="913fa-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="913fa-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="913fa-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="913fa-p103">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="913fa-p103">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="913fa-109">权限</span><span class="sxs-lookup"><span data-stu-id="913fa-109">Permissions</span></span>
<span data-ttu-id="913fa-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="913fa-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="913fa-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="913fa-112">Permission type</span></span>      | <span data-ttu-id="913fa-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="913fa-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="913fa-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="913fa-114">Delegated (work or school account)</span></span> | <span data-ttu-id="913fa-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="913fa-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="913fa-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="913fa-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="913fa-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="913fa-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="913fa-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="913fa-118">Application</span></span> | <span data-ttu-id="913fa-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="913fa-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="913fa-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="913fa-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="913fa-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="913fa-121">Request headers</span></span>
| <span data-ttu-id="913fa-122">名称</span><span class="sxs-lookup"><span data-stu-id="913fa-122">Name</span></span>       | <span data-ttu-id="913fa-123">说明</span><span class="sxs-lookup"><span data-stu-id="913fa-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="913fa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="913fa-124">Authorization</span></span>  | <span data-ttu-id="913fa-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="913fa-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="913fa-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="913fa-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="913fa-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="913fa-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="913fa-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="913fa-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="913fa-131">响应</span><span class="sxs-lookup"><span data-stu-id="913fa-131">Response</span></span>

<span data-ttu-id="913fa-p107">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="913fa-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="913fa-134">示例</span><span class="sxs-lookup"><span data-stu-id="913fa-134">Example</span></span>
<span data-ttu-id="913fa-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="913fa-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="913fa-136">请求</span><span class="sxs-lookup"><span data-stu-id="913fa-136">Request</span></span>
<span data-ttu-id="913fa-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="913fa-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="913fa-138">响应</span><span class="sxs-lookup"><span data-stu-id="913fa-138">Response</span></span>
<span data-ttu-id="913fa-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="913fa-139">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->