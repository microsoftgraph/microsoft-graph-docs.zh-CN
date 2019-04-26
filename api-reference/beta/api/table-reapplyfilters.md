---
title: 'Table: reapplyFilters'
description: 重新应用当前表上的所有筛选器。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 762f815126277bec33e649b0b33133c794e037f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330606"
---
# <a name="table-reapplyfilters"></a><span data-ttu-id="7d8ee-103">Table: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="7d8ee-103">Table: reapplyFilters</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d8ee-104">重新应用当前表上的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="7d8ee-104">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d8ee-105">权限</span><span class="sxs-lookup"><span data-stu-id="7d8ee-105">Permissions</span></span>
<span data-ttu-id="7d8ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d8ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d8ee-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d8ee-108">Permission type</span></span>      | <span data-ttu-id="7d8ee-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7d8ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d8ee-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d8ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d8ee-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d8ee-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d8ee-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d8ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d8ee-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d8ee-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d8ee-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d8ee-114">Application</span></span> | <span data-ttu-id="7d8ee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d8ee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d8ee-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d8ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/reapplyFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="7d8ee-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d8ee-117">Request headers</span></span>
| <span data-ttu-id="7d8ee-118">名称</span><span class="sxs-lookup"><span data-stu-id="7d8ee-118">Name</span></span>       | <span data-ttu-id="7d8ee-119">说明</span><span class="sxs-lookup"><span data-stu-id="7d8ee-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d8ee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d8ee-120">Authorization</span></span>  | <span data-ttu-id="7d8ee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7d8ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d8ee-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7d8ee-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7d8ee-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7d8ee-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d8ee-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d8ee-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7d8ee-127">响应</span><span class="sxs-lookup"><span data-stu-id="7d8ee-127">Response</span></span>

<span data-ttu-id="7d8ee-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7d8ee-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d8ee-130">示例</span><span class="sxs-lookup"><span data-stu-id="7d8ee-130">Example</span></span>
<span data-ttu-id="7d8ee-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7d8ee-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7d8ee-132">请求</span><span class="sxs-lookup"><span data-stu-id="7d8ee-132">Request</span></span>
<span data-ttu-id="7d8ee-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d8ee-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```

##### <a name="response"></a><span data-ttu-id="7d8ee-134">响应</span><span class="sxs-lookup"><span data-stu-id="7d8ee-134">Response</span></span>
<span data-ttu-id="7d8ee-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7d8ee-135">Here is an example of the response.</span></span> 
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
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
