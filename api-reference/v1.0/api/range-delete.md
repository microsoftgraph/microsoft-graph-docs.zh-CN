---
title: 'Range: delete'
description: 删除与范围相关的单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 671dc5785aae4d912d60c2356fc7b1a204630c3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575224"
---
# <a name="range-delete"></a><span data-ttu-id="e8066-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="e8066-103">Range: delete</span></span>

<span data-ttu-id="e8066-104">删除与范围相关的单元格。</span><span class="sxs-lookup"><span data-stu-id="e8066-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8066-105">权限</span><span class="sxs-lookup"><span data-stu-id="e8066-105">Permissions</span></span>
<span data-ttu-id="e8066-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8066-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8066-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8066-108">Permission type</span></span>      | <span data-ttu-id="e8066-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8066-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8066-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8066-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8066-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8066-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8066-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8066-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8066-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8066-113">Not supported.</span></span>    |
|<span data-ttu-id="e8066-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8066-114">Application</span></span> | <span data-ttu-id="e8066-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8066-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8066-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8066-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="e8066-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8066-117">Request headers</span></span>
| <span data-ttu-id="e8066-118">名称</span><span class="sxs-lookup"><span data-stu-id="e8066-118">Name</span></span>       | <span data-ttu-id="e8066-119">说明</span><span class="sxs-lookup"><span data-stu-id="e8066-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e8066-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8066-120">Authorization</span></span>  | <span data-ttu-id="e8066-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8066-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8066-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e8066-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e8066-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e8066-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8066-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8066-126">Request body</span></span>
<span data-ttu-id="e8066-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e8066-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e8066-128">参数</span><span class="sxs-lookup"><span data-stu-id="e8066-128">Parameter</span></span>    | <span data-ttu-id="e8066-129">类型</span><span class="sxs-lookup"><span data-stu-id="e8066-129">Type</span></span>   |<span data-ttu-id="e8066-130">说明</span><span class="sxs-lookup"><span data-stu-id="e8066-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8066-131">Shift</span><span class="sxs-lookup"><span data-stu-id="e8066-131">shift</span></span>|<span data-ttu-id="e8066-132">string</span><span class="sxs-lookup"><span data-stu-id="e8066-132">string</span></span>|<span data-ttu-id="e8066-133">指定移动单元格的方式。</span><span class="sxs-lookup"><span data-stu-id="e8066-133">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="e8066-134">可能的值为: `Up`、 `Left`。</span><span class="sxs-lookup"><span data-stu-id="e8066-134">The possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="e8066-135">响应</span><span class="sxs-lookup"><span data-stu-id="e8066-135">Response</span></span>

<span data-ttu-id="e8066-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e8066-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8066-138">示例</span><span class="sxs-lookup"><span data-stu-id="e8066-138">Example</span></span>
<span data-ttu-id="e8066-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e8066-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e8066-140">请求</span><span class="sxs-lookup"><span data-stu-id="e8066-140">Request</span></span>
<span data-ttu-id="e8066-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8066-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="e8066-142">响应</span><span class="sxs-lookup"><span data-stu-id="e8066-142">Response</span></span>
<span data-ttu-id="e8066-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e8066-143">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
