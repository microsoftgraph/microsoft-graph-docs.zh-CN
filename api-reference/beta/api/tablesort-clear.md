---
title: 'TableSort: clear'
description: 清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 5097498c1221a7cfd2e231232540cbef2d34a66e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536896"
---
# <a name="tablesort-clear"></a><span data-ttu-id="6ac8b-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="6ac8b-104">TableSort: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ac8b-p102">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="6ac8b-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ac8b-107">权限</span><span class="sxs-lookup"><span data-stu-id="6ac8b-107">Permissions</span></span>
<span data-ttu-id="6ac8b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ac8b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ac8b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ac8b-110">Permission type</span></span>      | <span data-ttu-id="6ac8b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ac8b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ac8b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac8b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6ac8b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ac8b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ac8b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac8b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ac8b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ac8b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ac8b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ac8b-116">Application</span></span> | <span data-ttu-id="6ac8b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ac8b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ac8b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ac8b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="6ac8b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ac8b-119">Request headers</span></span>
| <span data-ttu-id="6ac8b-120">名称</span><span class="sxs-lookup"><span data-stu-id="6ac8b-120">Name</span></span>       | <span data-ttu-id="6ac8b-121">说明</span><span class="sxs-lookup"><span data-stu-id="6ac8b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6ac8b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ac8b-122">Authorization</span></span>  | <span data-ttu-id="6ac8b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ac8b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ac8b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6ac8b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6ac8b-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6ac8b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ac8b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ac8b-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6ac8b-129">响应</span><span class="sxs-lookup"><span data-stu-id="6ac8b-129">Response</span></span>

<span data-ttu-id="6ac8b-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6ac8b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ac8b-132">示例</span><span class="sxs-lookup"><span data-stu-id="6ac8b-132">Example</span></span>
<span data-ttu-id="6ac8b-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6ac8b-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6ac8b-134">请求</span><span class="sxs-lookup"><span data-stu-id="6ac8b-134">Request</span></span>
<span data-ttu-id="6ac8b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ac8b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="6ac8b-136">响应</span><span class="sxs-lookup"><span data-stu-id="6ac8b-136">Response</span></span>
<span data-ttu-id="6ac8b-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6ac8b-137">Here is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/tablesort-clear.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
