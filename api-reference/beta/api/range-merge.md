---
title: 'Range: merge'
description: 将范围单元格合并到工作表的一个区域中。
author: lumine2008
ms.openlocfilehash: 628acea9c86ff7cf8b460fb5db2abb7157c85146
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317337"
---
# <a name="range-merge"></a><span data-ttu-id="e0419-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="e0419-103">Range: merge</span></span>

> <span data-ttu-id="e0419-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e0419-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0419-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e0419-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0419-106">将范围单元格合并到工作表的一个区域中。</span><span class="sxs-lookup"><span data-stu-id="e0419-106">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0419-107">权限</span><span class="sxs-lookup"><span data-stu-id="e0419-107">Permissions</span></span>
<span data-ttu-id="e0419-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0419-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0419-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0419-110">Permission type</span></span>      | <span data-ttu-id="e0419-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0419-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0419-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0419-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e0419-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0419-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0419-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0419-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0419-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0419-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0419-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0419-116">Application</span></span> | <span data-ttu-id="e0419-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0419-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0419-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0419-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="e0419-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0419-119">Request headers</span></span>
| <span data-ttu-id="e0419-120">Name</span><span class="sxs-lookup"><span data-stu-id="e0419-120">Name</span></span>       | <span data-ttu-id="e0419-121">说明</span><span class="sxs-lookup"><span data-stu-id="e0419-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e0419-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0419-122">Authorization</span></span>  | <span data-ttu-id="e0419-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0419-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0419-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e0419-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e0419-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e0419-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0419-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0419-128">Request body</span></span>
<span data-ttu-id="e0419-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e0419-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e0419-130">参数</span><span class="sxs-lookup"><span data-stu-id="e0419-130">Parameter</span></span>    | <span data-ttu-id="e0419-131">Type</span><span class="sxs-lookup"><span data-stu-id="e0419-131">Type</span></span>   |<span data-ttu-id="e0419-132">说明</span><span class="sxs-lookup"><span data-stu-id="e0419-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0419-133">横向</span><span class="sxs-lookup"><span data-stu-id="e0419-133">across</span></span>|<span data-ttu-id="e0419-134">boolean</span><span class="sxs-lookup"><span data-stu-id="e0419-134">boolean</span></span>|<span data-ttu-id="e0419-p105">可选。如果为 True，则将指定区域中每一行的单元格合并为一个单独的合并单元格。默认值是 false。</span><span class="sxs-lookup"><span data-stu-id="e0419-p105">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="e0419-138">响应</span><span class="sxs-lookup"><span data-stu-id="e0419-138">Response</span></span>

<span data-ttu-id="e0419-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e0419-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0419-141">示例</span><span class="sxs-lookup"><span data-stu-id="e0419-141">Example</span></span>
<span data-ttu-id="e0419-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e0419-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e0419-143">请求</span><span class="sxs-lookup"><span data-stu-id="e0419-143">Request</span></span>
<span data-ttu-id="e0419-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0419-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="e0419-145">响应</span><span class="sxs-lookup"><span data-stu-id="e0419-145">Response</span></span>
<span data-ttu-id="e0419-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0419-146">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->