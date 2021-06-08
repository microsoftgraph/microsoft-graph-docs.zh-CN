---
title: workbookApplication： calculate
description: 重新计算 Excel 中当前打开的所有工作簿。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a63de9bf28697b328f6a398201208fae7e207975
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787082"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="6688e-103">workbookApplication： calculate</span><span class="sxs-lookup"><span data-stu-id="6688e-103">workbookApplication: calculate</span></span>

<span data-ttu-id="6688e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6688e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6688e-105">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="6688e-105">Recalculate all currently opened workbooks in Excel.</span></span>

## <a name="permissions"></a><span data-ttu-id="6688e-106">权限</span><span class="sxs-lookup"><span data-stu-id="6688e-106">Permissions</span></span>
<span data-ttu-id="6688e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6688e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6688e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6688e-109">Permission type</span></span>      | <span data-ttu-id="6688e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6688e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6688e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6688e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6688e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6688e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6688e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6688e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6688e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6688e-114">Not supported.</span></span>    |
|<span data-ttu-id="6688e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6688e-115">Application</span></span> | <span data-ttu-id="6688e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6688e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6688e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6688e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/application/calculate
POST /me/drive/root:/{item-path}:/workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="6688e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6688e-118">Request headers</span></span>
| <span data-ttu-id="6688e-119">名称</span><span class="sxs-lookup"><span data-stu-id="6688e-119">Name</span></span>       | <span data-ttu-id="6688e-120">说明</span><span class="sxs-lookup"><span data-stu-id="6688e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6688e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6688e-121">Authorization</span></span>  | <span data-ttu-id="6688e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6688e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6688e-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="6688e-124">Content-type</span></span> | <span data-ttu-id="6688e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6688e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6688e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6688e-127">Request body</span></span>
<span data-ttu-id="6688e-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6688e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6688e-129">参数</span><span class="sxs-lookup"><span data-stu-id="6688e-129">Parameter</span></span>    | <span data-ttu-id="6688e-130">类型</span><span class="sxs-lookup"><span data-stu-id="6688e-130">Type</span></span>   |<span data-ttu-id="6688e-131">说明</span><span class="sxs-lookup"><span data-stu-id="6688e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6688e-132">calculationType</span><span class="sxs-lookup"><span data-stu-id="6688e-132">calculationType</span></span>|<span data-ttu-id="6688e-133">string</span><span class="sxs-lookup"><span data-stu-id="6688e-133">string</span></span>|<span data-ttu-id="6688e-134">指定要使用的计算类型。</span><span class="sxs-lookup"><span data-stu-id="6688e-134">Specifies the calculation type to use.</span></span>  <span data-ttu-id="6688e-135">可取值为：`Recalculate`、`Full`、`FullRebuild`。</span><span class="sxs-lookup"><span data-stu-id="6688e-135">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="6688e-136">响应</span><span class="sxs-lookup"><span data-stu-id="6688e-136">Response</span></span>

<span data-ttu-id="6688e-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6688e-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6688e-139">示例</span><span class="sxs-lookup"><span data-stu-id="6688e-139">Example</span></span>
<span data-ttu-id="6688e-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6688e-140">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="6688e-141">请求</span><span class="sxs-lookup"><span data-stu-id="6688e-141">Request</span></span>
<span data-ttu-id="6688e-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6688e-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6688e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6688e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookApplication_calculate"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6688e-144">C#</span><span class="sxs-lookup"><span data-stu-id="6688e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6688e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6688e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6688e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6688e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6688e-147">Java</span><span class="sxs-lookup"><span data-stu-id="6688e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookapplication-calculate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6688e-148">响应</span><span class="sxs-lookup"><span data-stu-id="6688e-148">Response</span></span>
<span data-ttu-id="6688e-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6688e-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
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

