---
title: workbookApplication：计算
description: 重新计算 Excel 中当前打开的所有工作簿。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d05767d03e10e0fb7785442fef6696b273f52424
ms.sourcegitcommit: 2f3e7325b5bc1f0cdc12a8acdf34d31cea3b8bdb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/07/2019
ms.locfileid: "38023182"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="a2b3e-103">workbookApplication：计算</span><span class="sxs-lookup"><span data-stu-id="a2b3e-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2b3e-104">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="a2b3e-104">Recalculate all currently opened workbooks in Excel.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2b3e-105">权限</span><span class="sxs-lookup"><span data-stu-id="a2b3e-105">Permissions</span></span>
<span data-ttu-id="a2b3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2b3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2b3e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2b3e-108">Permission type</span></span>      | <span data-ttu-id="a2b3e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2b3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2b3e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2b3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a2b3e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2b3e-111">Files.ReadWrite</span></span>     |
|<span data-ttu-id="a2b3e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2b3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2b3e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2b3e-113">Not supported.</span></span>    |
|<span data-ttu-id="a2b3e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2b3e-114">Application</span></span> | <span data-ttu-id="a2b3e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2b3e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2b3e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2b3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="a2b3e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2b3e-117">Request headers</span></span>
| <span data-ttu-id="a2b3e-118">名称</span><span class="sxs-lookup"><span data-stu-id="a2b3e-118">Name</span></span>       | <span data-ttu-id="a2b3e-119">说明</span><span class="sxs-lookup"><span data-stu-id="a2b3e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a2b3e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2b3e-120">Authorization</span></span>  | <span data-ttu-id="a2b3e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2b3e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2b3e-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="a2b3e-123">Content-type</span></span> | <span data-ttu-id="a2b3e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a2b3e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2b3e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2b3e-126">Request body</span></span>
<span data-ttu-id="a2b3e-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a2b3e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a2b3e-128">参数</span><span class="sxs-lookup"><span data-stu-id="a2b3e-128">Parameter</span></span>    | <span data-ttu-id="a2b3e-129">类型</span><span class="sxs-lookup"><span data-stu-id="a2b3e-129">Type</span></span>   |<span data-ttu-id="a2b3e-130">说明</span><span class="sxs-lookup"><span data-stu-id="a2b3e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2b3e-131">calculationType</span><span class="sxs-lookup"><span data-stu-id="a2b3e-131">calculationType</span></span>|<span data-ttu-id="a2b3e-132">string</span><span class="sxs-lookup"><span data-stu-id="a2b3e-132">string</span></span>|<span data-ttu-id="a2b3e-133">指定要使用的计算类型。</span><span class="sxs-lookup"><span data-stu-id="a2b3e-133">Specifies the calculation type to use.</span></span>  <span data-ttu-id="a2b3e-134">可取值为：`Recalculate`、`Full`、`FullRebuild`。</span><span class="sxs-lookup"><span data-stu-id="a2b3e-134">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="a2b3e-135">响应</span><span class="sxs-lookup"><span data-stu-id="a2b3e-135">Response</span></span>

<span data-ttu-id="a2b3e-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a2b3e-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b3e-138">示例</span><span class="sxs-lookup"><span data-stu-id="a2b3e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2b3e-139">请求</span><span class="sxs-lookup"><span data-stu-id="a2b3e-139">Request</span></span>
<span data-ttu-id="a2b3e-140">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="a2b3e-140">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a2b3e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2b3e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookApplication_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a2b3e-142">C#</span><span class="sxs-lookup"><span data-stu-id="a2b3e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2b3e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2b3e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a2b3e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2b3e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a2b3e-145">响应</span><span class="sxs-lookup"><span data-stu-id="a2b3e-145">Response</span></span>
<span data-ttu-id="a2b3e-146">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a2b3e-146">The following example shows the response.</span></span>

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
  "description": "workbookApplication: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
