---
title: 'TableSort: apply'
description: 执行排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f2279109f83758958cb00940604854c4edeecd45
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523440"
---
# <a name="tablesort-apply"></a><span data-ttu-id="e241a-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="e241a-103">TableSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e241a-104">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="e241a-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="e241a-105">权限</span><span class="sxs-lookup"><span data-stu-id="e241a-105">Permissions</span></span>
<span data-ttu-id="e241a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e241a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e241a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e241a-108">Permission type</span></span>      | <span data-ttu-id="e241a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e241a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e241a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e241a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e241a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e241a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e241a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e241a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e241a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e241a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e241a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e241a-114">Application</span></span> | <span data-ttu-id="e241a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e241a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e241a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e241a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="e241a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e241a-117">Request headers</span></span>
| <span data-ttu-id="e241a-118">名称</span><span class="sxs-lookup"><span data-stu-id="e241a-118">Name</span></span>       | <span data-ttu-id="e241a-119">说明</span><span class="sxs-lookup"><span data-stu-id="e241a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e241a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e241a-120">Authorization</span></span>  | <span data-ttu-id="e241a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e241a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e241a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e241a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e241a-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e241a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e241a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e241a-126">Request body</span></span>
<span data-ttu-id="e241a-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e241a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e241a-128">参数</span><span class="sxs-lookup"><span data-stu-id="e241a-128">Parameter</span></span>    | <span data-ttu-id="e241a-129">类型</span><span class="sxs-lookup"><span data-stu-id="e241a-129">Type</span></span>   |<span data-ttu-id="e241a-130">说明</span><span class="sxs-lookup"><span data-stu-id="e241a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e241a-131">fields</span><span class="sxs-lookup"><span data-stu-id="e241a-131">fields</span></span>|<span data-ttu-id="e241a-132">SortField</span><span class="sxs-lookup"><span data-stu-id="e241a-132">SortField</span></span>|<span data-ttu-id="e241a-133">作为排序依据的条件列表。</span><span class="sxs-lookup"><span data-stu-id="e241a-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="e241a-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="e241a-134">matchCase</span></span>|<span data-ttu-id="e241a-135">布尔</span><span class="sxs-lookup"><span data-stu-id="e241a-135">boolean</span></span>|<span data-ttu-id="e241a-p104">可选。是否让大小写对字符串排序产生影响。</span><span class="sxs-lookup"><span data-stu-id="e241a-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="e241a-138">方法</span><span class="sxs-lookup"><span data-stu-id="e241a-138">method</span></span>|<span data-ttu-id="e241a-139">string</span><span class="sxs-lookup"><span data-stu-id="e241a-139">string</span></span>|<span data-ttu-id="e241a-p105">可选。用于中文字符的排序方法。可能的值是：`PinYin`、`StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="e241a-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="e241a-143">响应</span><span class="sxs-lookup"><span data-stu-id="e241a-143">Response</span></span>

<span data-ttu-id="e241a-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e241a-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e241a-146">示例</span><span class="sxs-lookup"><span data-stu-id="e241a-146">Example</span></span>
<span data-ttu-id="e241a-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e241a-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e241a-148">请求</span><span class="sxs-lookup"><span data-stu-id="e241a-148">Request</span></span>
<span data-ttu-id="e241a-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e241a-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="e241a-150">响应</span><span class="sxs-lookup"><span data-stu-id="e241a-150">Response</span></span>
<span data-ttu-id="e241a-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e241a-151">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablesort-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
