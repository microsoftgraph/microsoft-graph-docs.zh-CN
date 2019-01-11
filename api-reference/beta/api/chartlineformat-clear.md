---
title: 'ChartLineFormat: clear'
description: 清除图表元素的线条格式。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7ee575b846bcf85c9cca7d0c203a3589fd28f180
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843900"
---
# <a name="chartlineformat-clear"></a><span data-ttu-id="ba0a0-103">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="ba0a0-103">ChartLineFormat: clear</span></span>

> <span data-ttu-id="ba0a0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ba0a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba0a0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ba0a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba0a0-106">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="ba0a0-106">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba0a0-107">权限</span><span class="sxs-lookup"><span data-stu-id="ba0a0-107">Permissions</span></span>
<span data-ttu-id="ba0a0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba0a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba0a0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba0a0-110">Permission type</span></span>      | <span data-ttu-id="ba0a0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba0a0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba0a0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba0a0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba0a0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba0a0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ba0a0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba0a0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba0a0-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba0a0-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ba0a0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba0a0-116">Application</span></span> | <span data-ttu-id="ba0a0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba0a0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba0a0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba0a0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="ba0a0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba0a0-119">Request headers</span></span>
| <span data-ttu-id="ba0a0-120">名称</span><span class="sxs-lookup"><span data-stu-id="ba0a0-120">Name</span></span>       | <span data-ttu-id="ba0a0-121">说明</span><span class="sxs-lookup"><span data-stu-id="ba0a0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ba0a0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba0a0-122">Authorization</span></span>  | <span data-ttu-id="ba0a0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba0a0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba0a0-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ba0a0-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ba0a0-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ba0a0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba0a0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba0a0-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ba0a0-129">响应</span><span class="sxs-lookup"><span data-stu-id="ba0a0-129">Response</span></span>

<span data-ttu-id="ba0a0-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ba0a0-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba0a0-132">示例</span><span class="sxs-lookup"><span data-stu-id="ba0a0-132">Example</span></span>
<span data-ttu-id="ba0a0-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ba0a0-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ba0a0-134">请求</span><span class="sxs-lookup"><span data-stu-id="ba0a0-134">Request</span></span>
<span data-ttu-id="ba0a0-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba0a0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line/clear
```

##### <a name="response"></a><span data-ttu-id="ba0a0-136">响应</span><span class="sxs-lookup"><span data-stu-id="ba0a0-136">Response</span></span>
<span data-ttu-id="ba0a0-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ba0a0-137">Here is an example of the response.</span></span> 
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
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
