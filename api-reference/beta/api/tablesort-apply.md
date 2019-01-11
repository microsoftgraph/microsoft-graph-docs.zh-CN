---
title: 'TableSort: apply'
description: 执行排序操作。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 2dc8d9c0619e434d3799ae03e0ef54354c868852
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844098"
---
# <a name="tablesort-apply"></a><span data-ttu-id="b7e66-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="b7e66-103">TableSort: apply</span></span>

> <span data-ttu-id="b7e66-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b7e66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7e66-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b7e66-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7e66-106">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="b7e66-106">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7e66-107">权限</span><span class="sxs-lookup"><span data-stu-id="b7e66-107">Permissions</span></span>
<span data-ttu-id="b7e66-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7e66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7e66-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7e66-110">Permission type</span></span>      | <span data-ttu-id="b7e66-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7e66-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7e66-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7e66-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b7e66-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7e66-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7e66-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7e66-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7e66-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7e66-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7e66-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7e66-116">Application</span></span> | <span data-ttu-id="b7e66-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7e66-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7e66-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7e66-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="b7e66-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7e66-119">Request headers</span></span>
| <span data-ttu-id="b7e66-120">名称</span><span class="sxs-lookup"><span data-stu-id="b7e66-120">Name</span></span>       | <span data-ttu-id="b7e66-121">说明</span><span class="sxs-lookup"><span data-stu-id="b7e66-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7e66-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7e66-122">Authorization</span></span>  | <span data-ttu-id="b7e66-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7e66-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7e66-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b7e66-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b7e66-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="b7e66-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7e66-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7e66-128">Request body</span></span>
<span data-ttu-id="b7e66-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b7e66-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b7e66-130">参数</span><span class="sxs-lookup"><span data-stu-id="b7e66-130">Parameter</span></span>    | <span data-ttu-id="b7e66-131">类型</span><span class="sxs-lookup"><span data-stu-id="b7e66-131">Type</span></span>   |<span data-ttu-id="b7e66-132">说明</span><span class="sxs-lookup"><span data-stu-id="b7e66-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7e66-133">fields</span><span class="sxs-lookup"><span data-stu-id="b7e66-133">fields</span></span>|<span data-ttu-id="b7e66-134">SortField</span><span class="sxs-lookup"><span data-stu-id="b7e66-134">SortField</span></span>|<span data-ttu-id="b7e66-135">作为排序依据的条件列表。</span><span class="sxs-lookup"><span data-stu-id="b7e66-135">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="b7e66-136">matchCase</span><span class="sxs-lookup"><span data-stu-id="b7e66-136">matchCase</span></span>|<span data-ttu-id="b7e66-137">boolean</span><span class="sxs-lookup"><span data-stu-id="b7e66-137">boolean</span></span>|<span data-ttu-id="b7e66-p105">可选。是否让大小写对字符串排序产生影响。</span><span class="sxs-lookup"><span data-stu-id="b7e66-p105">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="b7e66-140">方法</span><span class="sxs-lookup"><span data-stu-id="b7e66-140">method</span></span>|<span data-ttu-id="b7e66-141">string</span><span class="sxs-lookup"><span data-stu-id="b7e66-141">string</span></span>|<span data-ttu-id="b7e66-p106">可选。用于中文字符的排序方法。可能的值是：`PinYin`、`StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="b7e66-p106">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="b7e66-145">响应</span><span class="sxs-lookup"><span data-stu-id="b7e66-145">Response</span></span>

<span data-ttu-id="b7e66-p107">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b7e66-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7e66-148">示例</span><span class="sxs-lookup"><span data-stu-id="b7e66-148">Example</span></span>
<span data-ttu-id="b7e66-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b7e66-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7e66-150">请求</span><span class="sxs-lookup"><span data-stu-id="b7e66-150">Request</span></span>
<span data-ttu-id="b7e66-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7e66-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b7e66-152">响应</span><span class="sxs-lookup"><span data-stu-id="b7e66-152">Response</span></span>
<span data-ttu-id="b7e66-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b7e66-153">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
