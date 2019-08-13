---
title: 'workbookApplication: 计算'
description: 重新计算 Excel 中当前打开的所有工作簿。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a89bd864f0c145acf37a0caef64a42ebddd51eff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361961"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="4bac6-103">workbookApplication: 计算</span><span class="sxs-lookup"><span data-stu-id="4bac6-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bac6-104">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="4bac6-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bac6-105">权限</span><span class="sxs-lookup"><span data-stu-id="4bac6-105">Permissions</span></span>
<span data-ttu-id="4bac6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bac6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bac6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bac6-108">Permission type</span></span>      | <span data-ttu-id="4bac6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4bac6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bac6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bac6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4bac6-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bac6-111">Not supported.</span></span>    |
|<span data-ttu-id="4bac6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bac6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bac6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bac6-113">Not supported.</span></span>    |
|<span data-ttu-id="4bac6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bac6-114">Application</span></span> | <span data-ttu-id="4bac6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bac6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bac6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bac6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="4bac6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bac6-117">Request headers</span></span>
| <span data-ttu-id="4bac6-118">名称</span><span class="sxs-lookup"><span data-stu-id="4bac6-118">Name</span></span>       | <span data-ttu-id="4bac6-119">说明</span><span class="sxs-lookup"><span data-stu-id="4bac6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4bac6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bac6-120">Authorization</span></span>  | <span data-ttu-id="4bac6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4bac6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bac6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bac6-123">Request body</span></span>
<span data-ttu-id="4bac6-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4bac6-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4bac6-125">参数</span><span class="sxs-lookup"><span data-stu-id="4bac6-125">Parameter</span></span>    | <span data-ttu-id="4bac6-126">类型</span><span class="sxs-lookup"><span data-stu-id="4bac6-126">Type</span></span>   |<span data-ttu-id="4bac6-127">说明</span><span class="sxs-lookup"><span data-stu-id="4bac6-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bac6-128">calculationType</span><span class="sxs-lookup"><span data-stu-id="4bac6-128">calculationType</span></span>|<span data-ttu-id="4bac6-129">string</span><span class="sxs-lookup"><span data-stu-id="4bac6-129">string</span></span>|<span data-ttu-id="4bac6-130">指定要使用的计算类型。</span><span class="sxs-lookup"><span data-stu-id="4bac6-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="4bac6-131">可取值为：`Recalculate`、`Full`、`FullRebuild`。</span><span class="sxs-lookup"><span data-stu-id="4bac6-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="4bac6-132">响应</span><span class="sxs-lookup"><span data-stu-id="4bac6-132">Response</span></span>

<span data-ttu-id="4bac6-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4bac6-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bac6-135">示例</span><span class="sxs-lookup"><span data-stu-id="4bac6-135">Example</span></span>
<span data-ttu-id="4bac6-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4bac6-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4bac6-137">请求</span><span class="sxs-lookup"><span data-stu-id="4bac6-137">Request</span></span>
<span data-ttu-id="4bac6-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4bac6-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4bac6-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4bac6-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4bac6-140">C#</span><span class="sxs-lookup"><span data-stu-id="4bac6-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4bac6-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bac6-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4bac6-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="4bac6-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4bac6-143">Java</span><span class="sxs-lookup"><span data-stu-id="4bac6-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookapplication-calculate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4bac6-144">响应</span><span class="sxs-lookup"><span data-stu-id="4bac6-144">Response</span></span>
<span data-ttu-id="4bac6-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4bac6-145">Here is an example of the response.</span></span> 
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
