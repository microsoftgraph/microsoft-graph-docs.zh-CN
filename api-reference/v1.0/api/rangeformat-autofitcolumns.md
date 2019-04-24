---
title: 'RangeFormat: autofitColumns'
description: 根据列中的当前数据更改当前范围的列宽，以达到最佳宽度。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 232139841817b1b7fd16911b0ddd26d7c4377690
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453239"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="f61fe-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="f61fe-103">RangeFormat: autofitColumns</span></span>

<span data-ttu-id="f61fe-104">根据列中的当前数据更改当前范围的列宽，以达到最佳宽度。</span><span class="sxs-lookup"><span data-stu-id="f61fe-104">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="f61fe-105">权限</span><span class="sxs-lookup"><span data-stu-id="f61fe-105">Permissions</span></span>
<span data-ttu-id="f61fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f61fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f61fe-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f61fe-108">Permission type</span></span>      | <span data-ttu-id="f61fe-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f61fe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f61fe-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f61fe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f61fe-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f61fe-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f61fe-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f61fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f61fe-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f61fe-113">Not supported.</span></span>    |
|<span data-ttu-id="f61fe-114">Application</span><span class="sxs-lookup"><span data-stu-id="f61fe-114">Application</span></span> | <span data-ttu-id="f61fe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f61fe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f61fe-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f61fe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="f61fe-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f61fe-117">Request headers</span></span>
| <span data-ttu-id="f61fe-118">名称</span><span class="sxs-lookup"><span data-stu-id="f61fe-118">Name</span></span>       | <span data-ttu-id="f61fe-119">说明</span><span class="sxs-lookup"><span data-stu-id="f61fe-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f61fe-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f61fe-120">Authorization</span></span>  | <span data-ttu-id="f61fe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f61fe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f61fe-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f61fe-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f61fe-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f61fe-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f61fe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f61fe-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f61fe-127">响应</span><span class="sxs-lookup"><span data-stu-id="f61fe-127">Response</span></span>

<span data-ttu-id="f61fe-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f61fe-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f61fe-130">示例</span><span class="sxs-lookup"><span data-stu-id="f61fe-130">Example</span></span>
<span data-ttu-id="f61fe-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f61fe-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f61fe-132">请求</span><span class="sxs-lookup"><span data-stu-id="f61fe-132">Request</span></span>
<span data-ttu-id="f61fe-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f61fe-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```

##### <a name="response"></a><span data-ttu-id="f61fe-134">响应</span><span class="sxs-lookup"><span data-stu-id="f61fe-134">Response</span></span>
<span data-ttu-id="f61fe-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f61fe-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
