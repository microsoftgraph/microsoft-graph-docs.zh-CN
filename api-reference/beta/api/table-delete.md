---
title: 'Table: delete'
description: 删除表。
author: lumine2008
ms.openlocfilehash: f6b37823daab0b6f4bb2ec34d65f5d24d4c00710
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310610"
---
# <a name="table-delete"></a><span data-ttu-id="efd1b-103">Table: delete</span><span class="sxs-lookup"><span data-stu-id="efd1b-103">Table: delete</span></span>

> <span data-ttu-id="efd1b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="efd1b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efd1b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="efd1b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="efd1b-106">删除表。</span><span class="sxs-lookup"><span data-stu-id="efd1b-106">Deletes the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="efd1b-107">权限</span><span class="sxs-lookup"><span data-stu-id="efd1b-107">Permissions</span></span>
<span data-ttu-id="efd1b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efd1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd1b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="efd1b-110">Permission type</span></span>      | <span data-ttu-id="efd1b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="efd1b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efd1b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efd1b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="efd1b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efd1b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="efd1b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efd1b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efd1b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efd1b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="efd1b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="efd1b-116">Application</span></span> | <span data-ttu-id="efd1b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="efd1b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="efd1b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efd1b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="efd1b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="efd1b-119">Request headers</span></span>
| <span data-ttu-id="efd1b-120">Name</span><span class="sxs-lookup"><span data-stu-id="efd1b-120">Name</span></span>       | <span data-ttu-id="efd1b-121">说明</span><span class="sxs-lookup"><span data-stu-id="efd1b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="efd1b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="efd1b-122">Authorization</span></span>  | <span data-ttu-id="efd1b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="efd1b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="efd1b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="efd1b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="efd1b-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="efd1b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="efd1b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="efd1b-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="efd1b-129">响应</span><span class="sxs-lookup"><span data-stu-id="efd1b-129">Response</span></span>

<span data-ttu-id="efd1b-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="efd1b-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efd1b-132">示例</span><span class="sxs-lookup"><span data-stu-id="efd1b-132">Example</span></span>
<span data-ttu-id="efd1b-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="efd1b-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="efd1b-134">请求</span><span class="sxs-lookup"><span data-stu-id="efd1b-134">Request</span></span>
<span data-ttu-id="efd1b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efd1b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="efd1b-136">响应</span><span class="sxs-lookup"><span data-stu-id="efd1b-136">Response</span></span>
<span data-ttu-id="efd1b-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="efd1b-137">Here is an example of the response.</span></span> 
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
  "description": "Table: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->