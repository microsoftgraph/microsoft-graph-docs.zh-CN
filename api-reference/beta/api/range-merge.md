---
title: 'Range: merge'
description: 将范围单元格合并到工作表的一个区域中。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ef2ace7b963402b2be3dfd92c11c27029aeeed3c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337028"
---
# <a name="range-merge"></a><span data-ttu-id="0c989-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="0c989-103">Range: merge</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c989-104">将范围单元格合并到工作表的一个区域中。</span><span class="sxs-lookup"><span data-stu-id="0c989-104">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c989-105">权限</span><span class="sxs-lookup"><span data-stu-id="0c989-105">Permissions</span></span>
<span data-ttu-id="0c989-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c989-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c989-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c989-108">Permission type</span></span>      | <span data-ttu-id="0c989-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c989-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c989-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c989-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c989-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c989-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0c989-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c989-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c989-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c989-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0c989-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c989-114">Application</span></span> | <span data-ttu-id="0c989-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c989-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c989-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c989-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="0c989-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c989-117">Request headers</span></span>
| <span data-ttu-id="0c989-118">名称</span><span class="sxs-lookup"><span data-stu-id="0c989-118">Name</span></span>       | <span data-ttu-id="0c989-119">说明</span><span class="sxs-lookup"><span data-stu-id="0c989-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c989-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c989-120">Authorization</span></span>  | <span data-ttu-id="0c989-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c989-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c989-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0c989-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0c989-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0c989-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c989-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c989-126">Request body</span></span>
<span data-ttu-id="0c989-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0c989-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c989-128">参数</span><span class="sxs-lookup"><span data-stu-id="0c989-128">Parameter</span></span>    | <span data-ttu-id="0c989-129">类型</span><span class="sxs-lookup"><span data-stu-id="0c989-129">Type</span></span>   |<span data-ttu-id="0c989-130">说明</span><span class="sxs-lookup"><span data-stu-id="0c989-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c989-131">横向</span><span class="sxs-lookup"><span data-stu-id="0c989-131">across</span></span>|<span data-ttu-id="0c989-132">布尔</span><span class="sxs-lookup"><span data-stu-id="0c989-132">boolean</span></span>|<span data-ttu-id="0c989-p104">可选。如果为 True，则将指定区域中每一行的单元格合并为一个单独的合并单元格。默认值是 false。</span><span class="sxs-lookup"><span data-stu-id="0c989-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="0c989-136">响应</span><span class="sxs-lookup"><span data-stu-id="0c989-136">Response</span></span>

<span data-ttu-id="0c989-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0c989-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c989-139">示例</span><span class="sxs-lookup"><span data-stu-id="0c989-139">Example</span></span>
<span data-ttu-id="0c989-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="0c989-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0c989-141">请求</span><span class="sxs-lookup"><span data-stu-id="0c989-141">Request</span></span>
<span data-ttu-id="0c989-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0c989-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="0c989-143">响应</span><span class="sxs-lookup"><span data-stu-id="0c989-143">Response</span></span>
<span data-ttu-id="0c989-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0c989-144">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
