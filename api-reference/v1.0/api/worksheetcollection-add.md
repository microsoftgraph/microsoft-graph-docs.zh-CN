---
title: 'WorksheetCollection: add'
description: 对其.activate()。
author: lumine2008
ms.openlocfilehash: fc22e4b45732c9ef197ad9b1172ec87c8becbfc5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346597"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="1bbdb-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="1bbdb-103">WorksheetCollection: add</span></span>

<span data-ttu-id="1bbdb-p101">向工作簿添加新工作表。工作表将添加到现有工作表的末尾。如果您想要激活新添加的工作表，请对其调用 ".activate()。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="1bbdb-107">权限</span><span class="sxs-lookup"><span data-stu-id="1bbdb-107">Permissions</span></span>
<span data-ttu-id="1bbdb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bbdb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bbdb-110">Permission type</span></span>      | <span data-ttu-id="1bbdb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1bbdb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bbdb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bbdb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1bbdb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1bbdb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1bbdb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bbdb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bbdb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-115">Not supported.</span></span>    |
|<span data-ttu-id="1bbdb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bbdb-116">Application</span></span> | <span data-ttu-id="1bbdb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bbdb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bbdb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="1bbdb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bbdb-119">Request headers</span></span>
| <span data-ttu-id="1bbdb-120">Name</span><span class="sxs-lookup"><span data-stu-id="1bbdb-120">Name</span></span>       | <span data-ttu-id="1bbdb-121">说明</span><span class="sxs-lookup"><span data-stu-id="1bbdb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1bbdb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bbdb-122">Authorization</span></span>  | <span data-ttu-id="1bbdb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1bbdb-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1bbdb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1bbdb-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bbdb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bbdb-128">Request body</span></span>
<span data-ttu-id="1bbdb-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1bbdb-130">参数</span><span class="sxs-lookup"><span data-stu-id="1bbdb-130">Parameter</span></span>    | <span data-ttu-id="1bbdb-131">Type</span><span class="sxs-lookup"><span data-stu-id="1bbdb-131">Type</span></span>   |<span data-ttu-id="1bbdb-132">说明</span><span class="sxs-lookup"><span data-stu-id="1bbdb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1bbdb-133">name</span><span class="sxs-lookup"><span data-stu-id="1bbdb-133">name</span></span>|<span data-ttu-id="1bbdb-134">string</span><span class="sxs-lookup"><span data-stu-id="1bbdb-134">string</span></span>|<span data-ttu-id="1bbdb-p105">可选。要添加的工作表的名称。如果指定，名称应唯一。如果未指定，Excel 将确定新工作表的名称。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="1bbdb-139">响应</span><span class="sxs-lookup"><span data-stu-id="1bbdb-139">Response</span></span>

<span data-ttu-id="1bbdb-140">如果成功，此方法返回`200 OK`响应代码和[WorkbookWorksheet](../resources/worksheet.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-140">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bbdb-141">示例</span><span class="sxs-lookup"><span data-stu-id="1bbdb-141">Example</span></span>
<span data-ttu-id="1bbdb-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1bbdb-143">请求</span><span class="sxs-lookup"><span data-stu-id="1bbdb-143">Request</span></span>
<span data-ttu-id="1bbdb-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="1bbdb-145">响应</span><span class="sxs-lookup"><span data-stu-id="1bbdb-145">Response</span></span>
<span data-ttu-id="1bbdb-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1bbdb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
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