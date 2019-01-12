---
title: 'ChartFill: clear'
description: 清除图表元素的填充颜色。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b9a43093d00f6230e10333bf3ea0d8adb5a859f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918040"
---
# <a name="chartfill-clear"></a><span data-ttu-id="8f54b-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="8f54b-103">ChartFill: clear</span></span>

<span data-ttu-id="8f54b-104">清除图表元素的填充颜色。</span><span class="sxs-lookup"><span data-stu-id="8f54b-104">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f54b-105">权限</span><span class="sxs-lookup"><span data-stu-id="8f54b-105">Permissions</span></span>
<span data-ttu-id="8f54b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f54b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f54b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f54b-108">Permission type</span></span>      | <span data-ttu-id="8f54b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f54b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f54b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f54b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f54b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f54b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f54b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f54b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f54b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f54b-113">Not supported.</span></span>    |
|<span data-ttu-id="8f54b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f54b-114">Application</span></span> | <span data-ttu-id="8f54b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f54b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f54b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f54b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="8f54b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f54b-117">Request headers</span></span>
| <span data-ttu-id="8f54b-118">名称</span><span class="sxs-lookup"><span data-stu-id="8f54b-118">Name</span></span>       | <span data-ttu-id="8f54b-119">说明</span><span class="sxs-lookup"><span data-stu-id="8f54b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f54b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f54b-120">Authorization</span></span>  | <span data-ttu-id="8f54b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f54b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f54b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8f54b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8f54b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8f54b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f54b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f54b-126">Request body</span></span>
<span data-ttu-id="8f54b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f54b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f54b-128">响应</span><span class="sxs-lookup"><span data-stu-id="8f54b-128">Response</span></span>

<span data-ttu-id="8f54b-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8f54b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f54b-131">示例</span><span class="sxs-lookup"><span data-stu-id="8f54b-131">Example</span></span>
<span data-ttu-id="8f54b-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8f54b-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8f54b-133">请求</span><span class="sxs-lookup"><span data-stu-id="8f54b-133">Request</span></span>
<span data-ttu-id="8f54b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f54b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="8f54b-135">响应</span><span class="sxs-lookup"><span data-stu-id="8f54b-135">Response</span></span>
<span data-ttu-id="8f54b-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8f54b-136">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
