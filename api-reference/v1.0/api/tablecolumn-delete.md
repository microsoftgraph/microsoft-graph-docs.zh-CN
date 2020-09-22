---
title: 'TableColumn: delete'
description: 从表中删除列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5794e9f26b3be667f52f8b63eb4886a3e457b49d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023056"
---
# <a name="tablecolumn-delete"></a><span data-ttu-id="3dd79-103">TableColumn: delete</span><span class="sxs-lookup"><span data-stu-id="3dd79-103">TableColumn: delete</span></span>

<span data-ttu-id="3dd79-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dd79-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3dd79-105">从表中删除列。</span><span class="sxs-lookup"><span data-stu-id="3dd79-105">Deletes the column from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="3dd79-106">权限</span><span class="sxs-lookup"><span data-stu-id="3dd79-106">Permissions</span></span>
<span data-ttu-id="3dd79-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3dd79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dd79-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dd79-109">Permission type</span></span>      | <span data-ttu-id="3dd79-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3dd79-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dd79-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dd79-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3dd79-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3dd79-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3dd79-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dd79-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dd79-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dd79-114">Not supported.</span></span>    |
|<span data-ttu-id="3dd79-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dd79-115">Application</span></span> | <span data-ttu-id="3dd79-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dd79-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3dd79-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dd79-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="3dd79-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dd79-118">Request headers</span></span>
| <span data-ttu-id="3dd79-119">名称</span><span class="sxs-lookup"><span data-stu-id="3dd79-119">Name</span></span>       | <span data-ttu-id="3dd79-120">说明</span><span class="sxs-lookup"><span data-stu-id="3dd79-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3dd79-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dd79-121">Authorization</span></span>  | <span data-ttu-id="3dd79-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3dd79-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3dd79-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3dd79-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3dd79-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="3dd79-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dd79-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dd79-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3dd79-128">响应</span><span class="sxs-lookup"><span data-stu-id="3dd79-128">Response</span></span>

<span data-ttu-id="3dd79-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3dd79-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dd79-131">示例</span><span class="sxs-lookup"><span data-stu-id="3dd79-131">Example</span></span>
<span data-ttu-id="3dd79-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="3dd79-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3dd79-133">请求</span><span class="sxs-lookup"><span data-stu-id="3dd79-133">Request</span></span>
<span data-ttu-id="3dd79-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3dd79-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="3dd79-135">响应</span><span class="sxs-lookup"><span data-stu-id="3dd79-135">Response</span></span>
<span data-ttu-id="3dd79-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3dd79-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

