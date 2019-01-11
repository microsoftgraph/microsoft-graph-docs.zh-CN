---
title: 'ChartLineFormat: clear'
description: 清除图表元素的线条格式。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a89b0f178ff0de8f1fe54bd8d3b7c01deaece91b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836594"
---
# <a name="chartlineformat-clear"></a><span data-ttu-id="3ed56-103">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="3ed56-103">ChartLineFormat: clear</span></span>

<span data-ttu-id="3ed56-104">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="3ed56-104">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ed56-105">权限</span><span class="sxs-lookup"><span data-stu-id="3ed56-105">Permissions</span></span>
<span data-ttu-id="3ed56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ed56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ed56-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ed56-108">Permission type</span></span>      | <span data-ttu-id="3ed56-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ed56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ed56-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ed56-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ed56-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ed56-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3ed56-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ed56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ed56-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ed56-113">Not supported.</span></span>    |
|<span data-ttu-id="3ed56-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ed56-114">Application</span></span> | <span data-ttu-id="3ed56-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ed56-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ed56-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ed56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="3ed56-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ed56-117">Request headers</span></span>
| <span data-ttu-id="3ed56-118">名称</span><span class="sxs-lookup"><span data-stu-id="3ed56-118">Name</span></span>       | <span data-ttu-id="3ed56-119">说明</span><span class="sxs-lookup"><span data-stu-id="3ed56-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3ed56-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ed56-120">Authorization</span></span>  | <span data-ttu-id="3ed56-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ed56-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ed56-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3ed56-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3ed56-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="3ed56-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ed56-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ed56-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3ed56-127">响应</span><span class="sxs-lookup"><span data-stu-id="3ed56-127">Response</span></span>

<span data-ttu-id="3ed56-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3ed56-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ed56-130">示例</span><span class="sxs-lookup"><span data-stu-id="3ed56-130">Example</span></span>
<span data-ttu-id="3ed56-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="3ed56-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3ed56-132">请求</span><span class="sxs-lookup"><span data-stu-id="3ed56-132">Request</span></span>
<span data-ttu-id="3ed56-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ed56-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line/clear
```

##### <a name="response"></a><span data-ttu-id="3ed56-134">响应</span><span class="sxs-lookup"><span data-stu-id="3ed56-134">Response</span></span>
<span data-ttu-id="3ed56-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3ed56-135">Here is an example of the response.</span></span> 
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
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
