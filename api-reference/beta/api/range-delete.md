---
title: 'Range: delete'
description: 删除与范围相关的单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9fbd9fab13e94d33f5254911730d3640414b01f3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546406"
---
# <a name="range-delete"></a><span data-ttu-id="6b91c-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="6b91c-103">Range: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b91c-104">删除与范围相关的单元格。</span><span class="sxs-lookup"><span data-stu-id="6b91c-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b91c-105">权限</span><span class="sxs-lookup"><span data-stu-id="6b91c-105">Permissions</span></span>
<span data-ttu-id="6b91c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b91c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b91c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b91c-108">Permission type</span></span>      | <span data-ttu-id="6b91c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b91c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b91c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b91c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6b91c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b91c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6b91c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b91c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b91c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b91c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6b91c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b91c-114">Application</span></span> | <span data-ttu-id="6b91c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b91c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b91c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b91c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="6b91c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b91c-117">Request headers</span></span>
| <span data-ttu-id="6b91c-118">名称</span><span class="sxs-lookup"><span data-stu-id="6b91c-118">Name</span></span>       | <span data-ttu-id="6b91c-119">说明</span><span class="sxs-lookup"><span data-stu-id="6b91c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6b91c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b91c-120">Authorization</span></span>  | <span data-ttu-id="6b91c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b91c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6b91c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6b91c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6b91c-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6b91c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b91c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b91c-126">Request body</span></span>
<span data-ttu-id="6b91c-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6b91c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6b91c-128">参数</span><span class="sxs-lookup"><span data-stu-id="6b91c-128">Parameter</span></span>    | <span data-ttu-id="6b91c-129">类型</span><span class="sxs-lookup"><span data-stu-id="6b91c-129">Type</span></span>   |<span data-ttu-id="6b91c-130">说明</span><span class="sxs-lookup"><span data-stu-id="6b91c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b91c-131">Shift</span><span class="sxs-lookup"><span data-stu-id="6b91c-131">shift</span></span>|<span data-ttu-id="6b91c-132">string</span><span class="sxs-lookup"><span data-stu-id="6b91c-132">string</span></span>|<span data-ttu-id="6b91c-p104">指定移动单元格的方式。可能的值是：`Up`、`Left`。</span><span class="sxs-lookup"><span data-stu-id="6b91c-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="6b91c-135">响应</span><span class="sxs-lookup"><span data-stu-id="6b91c-135">Response</span></span>

<span data-ttu-id="6b91c-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6b91c-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b91c-138">示例</span><span class="sxs-lookup"><span data-stu-id="6b91c-138">Example</span></span>
<span data-ttu-id="6b91c-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6b91c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6b91c-140">请求</span><span class="sxs-lookup"><span data-stu-id="6b91c-140">Request</span></span>
<span data-ttu-id="6b91c-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b91c-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="6b91c-142">响应</span><span class="sxs-lookup"><span data-stu-id="6b91c-142">Response</span></span>
<span data-ttu-id="6b91c-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6b91c-143">Here is an example of the response.</span></span> 
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
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
