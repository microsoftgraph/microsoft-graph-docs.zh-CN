---
title: 'WorksheetCollection: add'
description: 对其.activate()。
author: lumine2008
ms.openlocfilehash: 560a66c4beb589fbb736f0aa27784827740c0440
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363576"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="181d6-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="181d6-103">WorksheetCollection: add</span></span>

> <span data-ttu-id="181d6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="181d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="181d6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="181d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="181d6-p102">向工作簿添加新工作表。工作表将添加到现有工作表的末尾。如果您想要激活新添加的工作表，请对其调用 ".activate()。</span><span class="sxs-lookup"><span data-stu-id="181d6-p102">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="181d6-109">权限</span><span class="sxs-lookup"><span data-stu-id="181d6-109">Permissions</span></span>
<span data-ttu-id="181d6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="181d6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="181d6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="181d6-112">Permission type</span></span>      | <span data-ttu-id="181d6-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="181d6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="181d6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="181d6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="181d6-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="181d6-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="181d6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="181d6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="181d6-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="181d6-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="181d6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="181d6-118">Application</span></span> | <span data-ttu-id="181d6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="181d6-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="181d6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="181d6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="181d6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="181d6-121">Request headers</span></span>
| <span data-ttu-id="181d6-122">Name</span><span class="sxs-lookup"><span data-stu-id="181d6-122">Name</span></span>       | <span data-ttu-id="181d6-123">说明</span><span class="sxs-lookup"><span data-stu-id="181d6-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="181d6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="181d6-124">Authorization</span></span>  | <span data-ttu-id="181d6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="181d6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="181d6-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="181d6-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="181d6-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="181d6-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="181d6-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="181d6-130">Request body</span></span>
<span data-ttu-id="181d6-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="181d6-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="181d6-132">参数</span><span class="sxs-lookup"><span data-stu-id="181d6-132">Parameter</span></span>    | <span data-ttu-id="181d6-133">Type</span><span class="sxs-lookup"><span data-stu-id="181d6-133">Type</span></span>   |<span data-ttu-id="181d6-134">说明</span><span class="sxs-lookup"><span data-stu-id="181d6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="181d6-135">name</span><span class="sxs-lookup"><span data-stu-id="181d6-135">name</span></span>|<span data-ttu-id="181d6-136">string</span><span class="sxs-lookup"><span data-stu-id="181d6-136">string</span></span>|<span data-ttu-id="181d6-p106">可选。要添加的工作表的名称。如果指定，名称应唯一。如果未指定，Excel 将确定新工作表的名称。</span><span class="sxs-lookup"><span data-stu-id="181d6-p106">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="181d6-141">响应</span><span class="sxs-lookup"><span data-stu-id="181d6-141">Response</span></span>

<span data-ttu-id="181d6-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Worksheet](../resources/worksheet.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="181d6-142">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="181d6-143">示例</span><span class="sxs-lookup"><span data-stu-id="181d6-143">Example</span></span>
<span data-ttu-id="181d6-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="181d6-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="181d6-145">请求</span><span class="sxs-lookup"><span data-stu-id="181d6-145">Request</span></span>
<span data-ttu-id="181d6-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="181d6-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="181d6-147">响应</span><span class="sxs-lookup"><span data-stu-id="181d6-147">Response</span></span>
<span data-ttu-id="181d6-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="181d6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->