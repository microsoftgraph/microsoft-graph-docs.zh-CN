---
title: 'WorksheetProtection: protect'
description: 保护工作表。如果工作表处于受保护状态，则会引发它。
author: lumine2008
ms.openlocfilehash: 28aa911e9eaee53272432bda78ed01073d899166
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303472"
---
# <a name="worksheetprotection-protect"></a><span data-ttu-id="e30c1-104">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="e30c1-104">WorksheetProtection: protect</span></span>

> <span data-ttu-id="e30c1-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e30c1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e30c1-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e30c1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e30c1-p103">保护工作表。如果工作表处于受保护状态，则会引发它。</span><span class="sxs-lookup"><span data-stu-id="e30c1-p103">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="e30c1-109">权限</span><span class="sxs-lookup"><span data-stu-id="e30c1-109">Permissions</span></span>
<span data-ttu-id="e30c1-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e30c1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e30c1-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e30c1-112">Permission type</span></span>      | <span data-ttu-id="e30c1-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e30c1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e30c1-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e30c1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e30c1-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e30c1-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e30c1-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e30c1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e30c1-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e30c1-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e30c1-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e30c1-118">Application</span></span> | <span data-ttu-id="e30c1-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e30c1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e30c1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e30c1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="e30c1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e30c1-121">Request headers</span></span>
| <span data-ttu-id="e30c1-122">Name</span><span class="sxs-lookup"><span data-stu-id="e30c1-122">Name</span></span>       | <span data-ttu-id="e30c1-123">说明</span><span class="sxs-lookup"><span data-stu-id="e30c1-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e30c1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e30c1-124">Authorization</span></span>  | <span data-ttu-id="e30c1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e30c1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e30c1-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e30c1-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="e30c1-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e30c1-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e30c1-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e30c1-130">Request body</span></span>
<span data-ttu-id="e30c1-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e30c1-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e30c1-132">参数</span><span class="sxs-lookup"><span data-stu-id="e30c1-132">Parameter</span></span>    | <span data-ttu-id="e30c1-133">Type</span><span class="sxs-lookup"><span data-stu-id="e30c1-133">Type</span></span>   |<span data-ttu-id="e30c1-134">说明</span><span class="sxs-lookup"><span data-stu-id="e30c1-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e30c1-135">options</span><span class="sxs-lookup"><span data-stu-id="e30c1-135">options</span></span>|<span data-ttu-id="e30c1-136">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="e30c1-136">WorksheetProtectionOptions</span></span>|<span data-ttu-id="e30c1-p107">可选。工作表保护选项。</span><span class="sxs-lookup"><span data-stu-id="e30c1-p107">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="e30c1-139">响应</span><span class="sxs-lookup"><span data-stu-id="e30c1-139">Response</span></span>

<span data-ttu-id="e30c1-p108">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e30c1-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e30c1-142">示例</span><span class="sxs-lookup"><span data-stu-id="e30c1-142">Example</span></span>
<span data-ttu-id="e30c1-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e30c1-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e30c1-144">请求</span><span class="sxs-lookup"><span data-stu-id="e30c1-144">Request</span></span>
<span data-ttu-id="e30c1-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e30c1-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="e30c1-146">响应</span><span class="sxs-lookup"><span data-stu-id="e30c1-146">Response</span></span>
<span data-ttu-id="e30c1-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e30c1-147">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
