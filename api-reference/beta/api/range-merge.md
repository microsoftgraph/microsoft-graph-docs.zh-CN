---
title: 'Range: merge'
description: 将范围单元格合并到工作表的一个区域中。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 151163604bc7eada167daebdb325857cc6e87ce4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990521"
---
# <a name="range-merge"></a><span data-ttu-id="2f31b-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="2f31b-103">Range: merge</span></span>

> <span data-ttu-id="2f31b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2f31b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f31b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2f31b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f31b-106">将范围单元格合并到工作表的一个区域中。</span><span class="sxs-lookup"><span data-stu-id="2f31b-106">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f31b-107">权限</span><span class="sxs-lookup"><span data-stu-id="2f31b-107">Permissions</span></span>
<span data-ttu-id="2f31b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f31b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f31b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f31b-110">Permission type</span></span>      | <span data-ttu-id="2f31b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f31b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f31b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f31b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2f31b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f31b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2f31b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f31b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f31b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f31b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2f31b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f31b-116">Application</span></span> | <span data-ttu-id="2f31b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f31b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f31b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f31b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="2f31b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f31b-119">Request headers</span></span>
| <span data-ttu-id="2f31b-120">名称</span><span class="sxs-lookup"><span data-stu-id="2f31b-120">Name</span></span>       | <span data-ttu-id="2f31b-121">说明</span><span class="sxs-lookup"><span data-stu-id="2f31b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2f31b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f31b-122">Authorization</span></span>  | <span data-ttu-id="2f31b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f31b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f31b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2f31b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2f31b-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2f31b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f31b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f31b-128">Request body</span></span>
<span data-ttu-id="2f31b-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2f31b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f31b-130">参数</span><span class="sxs-lookup"><span data-stu-id="2f31b-130">Parameter</span></span>    | <span data-ttu-id="2f31b-131">类型</span><span class="sxs-lookup"><span data-stu-id="2f31b-131">Type</span></span>   |<span data-ttu-id="2f31b-132">说明</span><span class="sxs-lookup"><span data-stu-id="2f31b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f31b-133">横向</span><span class="sxs-lookup"><span data-stu-id="2f31b-133">across</span></span>|<span data-ttu-id="2f31b-134">boolean</span><span class="sxs-lookup"><span data-stu-id="2f31b-134">boolean</span></span>|<span data-ttu-id="2f31b-p105">可选。如果为 True，则将指定区域中每一行的单元格合并为一个单独的合并单元格。默认值是 false。</span><span class="sxs-lookup"><span data-stu-id="2f31b-p105">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="2f31b-138">响应</span><span class="sxs-lookup"><span data-stu-id="2f31b-138">Response</span></span>

<span data-ttu-id="2f31b-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2f31b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f31b-141">示例</span><span class="sxs-lookup"><span data-stu-id="2f31b-141">Example</span></span>
<span data-ttu-id="2f31b-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2f31b-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2f31b-143">请求</span><span class="sxs-lookup"><span data-stu-id="2f31b-143">Request</span></span>
<span data-ttu-id="2f31b-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f31b-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2f31b-145">响应</span><span class="sxs-lookup"><span data-stu-id="2f31b-145">Response</span></span>
<span data-ttu-id="2f31b-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2f31b-146">Here is an example of the response.</span></span> 
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
