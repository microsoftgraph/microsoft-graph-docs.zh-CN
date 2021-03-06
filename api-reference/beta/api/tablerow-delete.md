---
title: 'TableRow: delete'
description: 从表中删除行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ca42ac135cbed97e137842fe643c792a6fcb4af5
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516771"
---
# <a name="tablerow-delete"></a><span data-ttu-id="4f4da-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="4f4da-103">TableRow: delete</span></span>

<span data-ttu-id="4f4da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f4da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f4da-105">从表中删除行。</span><span class="sxs-lookup"><span data-stu-id="4f4da-105">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f4da-106">权限</span><span class="sxs-lookup"><span data-stu-id="4f4da-106">Permissions</span></span>
<span data-ttu-id="4f4da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f4da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f4da-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f4da-109">Permission type</span></span>      | <span data-ttu-id="4f4da-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f4da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f4da-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f4da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f4da-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f4da-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f4da-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f4da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f4da-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f4da-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4f4da-115">Application</span><span class="sxs-lookup"><span data-stu-id="4f4da-115">Application</span></span> | <span data-ttu-id="4f4da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f4da-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f4da-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f4da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /workbook/tables/{id|name}/rows/{index}
DELETE /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}

```
## <a name="request-headers"></a><span data-ttu-id="4f4da-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f4da-118">Request headers</span></span>
| <span data-ttu-id="4f4da-119">名称</span><span class="sxs-lookup"><span data-stu-id="4f4da-119">Name</span></span>       | <span data-ttu-id="4f4da-120">说明</span><span class="sxs-lookup"><span data-stu-id="4f4da-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4f4da-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f4da-121">Authorization</span></span>  | <span data-ttu-id="4f4da-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f4da-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f4da-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4f4da-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4f4da-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="4f4da-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f4da-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f4da-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4f4da-128">响应</span><span class="sxs-lookup"><span data-stu-id="4f4da-128">Response</span></span>

<span data-ttu-id="4f4da-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4f4da-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f4da-131">示例</span><span class="sxs-lookup"><span data-stu-id="4f4da-131">Example</span></span>
<span data-ttu-id="4f4da-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4f4da-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4f4da-133">请求</span><span class="sxs-lookup"><span data-stu-id="4f4da-133">Request</span></span>
<span data-ttu-id="4f4da-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f4da-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
```

##### <a name="response"></a><span data-ttu-id="4f4da-135">响应</span><span class="sxs-lookup"><span data-stu-id="4f4da-135">Response</span></span>
<span data-ttu-id="4f4da-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4f4da-136">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


