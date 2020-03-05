---
title: 'TableRow: delete'
description: 从表中删除行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e0a12f2160e1d3c9f35862c34fbe571ac2a8e3d7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452676"
---
# <a name="tablerow-delete"></a><span data-ttu-id="1c704-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="1c704-103">TableRow: delete</span></span>

<span data-ttu-id="1c704-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1c704-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c704-105">从表中删除行。</span><span class="sxs-lookup"><span data-stu-id="1c704-105">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c704-106">权限</span><span class="sxs-lookup"><span data-stu-id="1c704-106">Permissions</span></span>
<span data-ttu-id="1c704-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c704-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c704-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c704-109">Permission type</span></span>      | <span data-ttu-id="1c704-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c704-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c704-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c704-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c704-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c704-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c704-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c704-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c704-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c704-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c704-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c704-115">Application</span></span> | <span data-ttu-id="1c704-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c704-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c704-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c704-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/{index}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/delete

```
## <a name="request-headers"></a><span data-ttu-id="1c704-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c704-118">Request headers</span></span>
| <span data-ttu-id="1c704-119">名称</span><span class="sxs-lookup"><span data-stu-id="1c704-119">Name</span></span>       | <span data-ttu-id="1c704-120">说明</span><span class="sxs-lookup"><span data-stu-id="1c704-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1c704-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c704-121">Authorization</span></span>  | <span data-ttu-id="1c704-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c704-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c704-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1c704-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1c704-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1c704-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c704-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c704-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1c704-128">响应</span><span class="sxs-lookup"><span data-stu-id="1c704-128">Response</span></span>

<span data-ttu-id="1c704-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1c704-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c704-131">示例</span><span class="sxs-lookup"><span data-stu-id="1c704-131">Example</span></span>
<span data-ttu-id="1c704-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1c704-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1c704-133">请求</span><span class="sxs-lookup"><span data-stu-id="1c704-133">Request</span></span>
<span data-ttu-id="1c704-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c704-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/delete
```

##### <a name="response"></a><span data-ttu-id="1c704-135">响应</span><span class="sxs-lookup"><span data-stu-id="1c704-135">Response</span></span>
<span data-ttu-id="1c704-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1c704-136">Here is an example of the response.</span></span> 
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
