---
title: 'Range: delete'
description: 删除与范围相关的单元格。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 1817a1c1481d86e08de4146215da6f6fc8de6a8c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871783"
---
# <a name="range-delete"></a><span data-ttu-id="8d181-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="8d181-103">Range: delete</span></span>

> <span data-ttu-id="8d181-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8d181-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d181-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8d181-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d181-106">删除与范围相关的单元格。</span><span class="sxs-lookup"><span data-stu-id="8d181-106">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d181-107">权限</span><span class="sxs-lookup"><span data-stu-id="8d181-107">Permissions</span></span>
<span data-ttu-id="8d181-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d181-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d181-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d181-110">Permission type</span></span>      | <span data-ttu-id="8d181-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d181-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d181-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d181-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d181-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d181-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d181-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d181-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d181-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d181-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d181-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d181-116">Application</span></span> | <span data-ttu-id="8d181-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d181-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d181-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d181-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="8d181-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d181-119">Request headers</span></span>
| <span data-ttu-id="8d181-120">名称</span><span class="sxs-lookup"><span data-stu-id="8d181-120">Name</span></span>       | <span data-ttu-id="8d181-121">说明</span><span class="sxs-lookup"><span data-stu-id="8d181-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d181-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d181-122">Authorization</span></span>  | <span data-ttu-id="8d181-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d181-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8d181-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8d181-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8d181-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8d181-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d181-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d181-128">Request body</span></span>
<span data-ttu-id="8d181-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8d181-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8d181-130">参数</span><span class="sxs-lookup"><span data-stu-id="8d181-130">Parameter</span></span>    | <span data-ttu-id="8d181-131">类型</span><span class="sxs-lookup"><span data-stu-id="8d181-131">Type</span></span>   |<span data-ttu-id="8d181-132">说明</span><span class="sxs-lookup"><span data-stu-id="8d181-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d181-133">Shift</span><span class="sxs-lookup"><span data-stu-id="8d181-133">shift</span></span>|<span data-ttu-id="8d181-134">string</span><span class="sxs-lookup"><span data-stu-id="8d181-134">string</span></span>|<span data-ttu-id="8d181-p105">指定移动单元格的方式。可能的值是：`Up`、`Left`。</span><span class="sxs-lookup"><span data-stu-id="8d181-p105">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="8d181-137">响应</span><span class="sxs-lookup"><span data-stu-id="8d181-137">Response</span></span>

<span data-ttu-id="8d181-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8d181-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d181-140">示例</span><span class="sxs-lookup"><span data-stu-id="8d181-140">Example</span></span>
<span data-ttu-id="8d181-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8d181-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8d181-142">请求</span><span class="sxs-lookup"><span data-stu-id="8d181-142">Request</span></span>
<span data-ttu-id="8d181-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d181-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="8d181-144">响应</span><span class="sxs-lookup"><span data-stu-id="8d181-144">Response</span></span>
<span data-ttu-id="8d181-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8d181-145">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
