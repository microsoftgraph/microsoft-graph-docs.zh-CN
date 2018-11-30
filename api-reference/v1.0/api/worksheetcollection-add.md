---
title: 'WorksheetCollection: add'
description: 对其.activate()。
ms.openlocfilehash: 992524aae6dfca0619c043eb0ddb7a4100f50206
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009221"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="c87ce-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="c87ce-103">WorksheetCollection: add</span></span>

<span data-ttu-id="c87ce-p101">向工作簿添加新工作表。工作表将添加到现有工作表的末尾。如果您想要激活新添加的工作表，请对其调用 ".activate()。</span><span class="sxs-lookup"><span data-stu-id="c87ce-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="c87ce-107">权限</span><span class="sxs-lookup"><span data-stu-id="c87ce-107">Permissions</span></span>
<span data-ttu-id="c87ce-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c87ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c87ce-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c87ce-110">Permission type</span></span>      | <span data-ttu-id="c87ce-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c87ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c87ce-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c87ce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c87ce-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c87ce-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c87ce-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c87ce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c87ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c87ce-115">Not supported.</span></span>    |
|<span data-ttu-id="c87ce-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c87ce-116">Application</span></span> | <span data-ttu-id="c87ce-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c87ce-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c87ce-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c87ce-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="c87ce-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c87ce-119">Request headers</span></span>
| <span data-ttu-id="c87ce-120">名称</span><span class="sxs-lookup"><span data-stu-id="c87ce-120">Name</span></span>       | <span data-ttu-id="c87ce-121">说明</span><span class="sxs-lookup"><span data-stu-id="c87ce-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c87ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c87ce-122">Authorization</span></span>  | <span data-ttu-id="c87ce-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c87ce-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c87ce-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c87ce-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c87ce-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c87ce-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c87ce-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c87ce-128">Request body</span></span>
<span data-ttu-id="c87ce-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c87ce-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c87ce-130">参数</span><span class="sxs-lookup"><span data-stu-id="c87ce-130">Parameter</span></span>    | <span data-ttu-id="c87ce-131">类型</span><span class="sxs-lookup"><span data-stu-id="c87ce-131">Type</span></span>   |<span data-ttu-id="c87ce-132">说明</span><span class="sxs-lookup"><span data-stu-id="c87ce-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c87ce-133">name</span><span class="sxs-lookup"><span data-stu-id="c87ce-133">name</span></span>|<span data-ttu-id="c87ce-134">string</span><span class="sxs-lookup"><span data-stu-id="c87ce-134">string</span></span>|<span data-ttu-id="c87ce-p105">可选。要添加的工作表的名称。如果指定，名称应唯一。如果未指定，Excel 将确定新工作表的名称。</span><span class="sxs-lookup"><span data-stu-id="c87ce-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="c87ce-139">响应</span><span class="sxs-lookup"><span data-stu-id="c87ce-139">Response</span></span>

<span data-ttu-id="c87ce-140">如果成功，此方法返回`200 OK`响应代码和[WorkbookWorksheet](../resources/worksheet.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="c87ce-140">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c87ce-141">示例</span><span class="sxs-lookup"><span data-stu-id="c87ce-141">Example</span></span>
<span data-ttu-id="c87ce-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c87ce-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c87ce-143">请求</span><span class="sxs-lookup"><span data-stu-id="c87ce-143">Request</span></span>
<span data-ttu-id="c87ce-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c87ce-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c87ce-145">响应</span><span class="sxs-lookup"><span data-stu-id="c87ce-145">Response</span></span>
<span data-ttu-id="c87ce-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c87ce-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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