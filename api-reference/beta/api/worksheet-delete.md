---
title: 'Worksheet: delete'
description: 从工作簿中删除工作表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 53f8dab1cd20107733827cbfdea358b48a150d12
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339670"
---
# <a name="worksheet-delete"></a><span data-ttu-id="92cf1-103">Worksheet: delete</span><span class="sxs-lookup"><span data-stu-id="92cf1-103">Worksheet: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92cf1-104">从工作簿中删除工作表。</span><span class="sxs-lookup"><span data-stu-id="92cf1-104">Deletes the worksheet from the workbook.</span></span>
## <a name="permissions"></a><span data-ttu-id="92cf1-105">权限</span><span class="sxs-lookup"><span data-stu-id="92cf1-105">Permissions</span></span>
<span data-ttu-id="92cf1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92cf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92cf1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="92cf1-108">Permission type</span></span>      | <span data-ttu-id="92cf1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92cf1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92cf1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92cf1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="92cf1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92cf1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="92cf1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92cf1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92cf1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92cf1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="92cf1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="92cf1-114">Application</span></span> | <span data-ttu-id="92cf1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="92cf1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92cf1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92cf1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="92cf1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="92cf1-117">Request headers</span></span>
| <span data-ttu-id="92cf1-118">名称</span><span class="sxs-lookup"><span data-stu-id="92cf1-118">Name</span></span>       | <span data-ttu-id="92cf1-119">说明</span><span class="sxs-lookup"><span data-stu-id="92cf1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="92cf1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="92cf1-120">Authorization</span></span>  | <span data-ttu-id="92cf1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92cf1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="92cf1-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="92cf1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="92cf1-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="92cf1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92cf1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="92cf1-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="92cf1-127">响应</span><span class="sxs-lookup"><span data-stu-id="92cf1-127">Response</span></span>

<span data-ttu-id="92cf1-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="92cf1-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92cf1-130">示例</span><span class="sxs-lookup"><span data-stu-id="92cf1-130">Example</span></span>
<span data-ttu-id="92cf1-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="92cf1-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="92cf1-132">请求</span><span class="sxs-lookup"><span data-stu-id="92cf1-132">Request</span></span>
<span data-ttu-id="92cf1-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92cf1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="92cf1-134">响应</span><span class="sxs-lookup"><span data-stu-id="92cf1-134">Response</span></span>
<span data-ttu-id="92cf1-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="92cf1-135">Here is an example of the response.</span></span> 
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
  "description": "Worksheet: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
