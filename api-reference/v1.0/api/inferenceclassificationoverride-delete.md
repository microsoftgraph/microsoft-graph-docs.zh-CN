---
title: 删除 inferenceClassificationOverride
description: 删除由其 ID 指定的替代。
localization_priority: Normal
ms.openlocfilehash: ae4043f0f118519de860c12431f0c6a80289a08f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277110"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="53fbe-103">删除 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="53fbe-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="53fbe-104">删除由其 ID 指定的替代。</span><span class="sxs-lookup"><span data-stu-id="53fbe-104">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="53fbe-105">权限</span><span class="sxs-lookup"><span data-stu-id="53fbe-105">Permissions</span></span>
<span data-ttu-id="53fbe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53fbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53fbe-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="53fbe-108">Permission type</span></span>      | <span data-ttu-id="53fbe-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53fbe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53fbe-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53fbe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53fbe-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53fbe-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="53fbe-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53fbe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53fbe-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53fbe-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="53fbe-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="53fbe-114">Application</span></span> | <span data-ttu-id="53fbe-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53fbe-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="53fbe-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53fbe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="53fbe-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="53fbe-117">Request headers</span></span>
| <span data-ttu-id="53fbe-118">名称</span><span class="sxs-lookup"><span data-stu-id="53fbe-118">Name</span></span>       | <span data-ttu-id="53fbe-119">类型</span><span class="sxs-lookup"><span data-stu-id="53fbe-119">Type</span></span> | <span data-ttu-id="53fbe-120">说明</span><span class="sxs-lookup"><span data-stu-id="53fbe-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53fbe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53fbe-121">Authorization</span></span>  | <span data-ttu-id="53fbe-122">string</span><span class="sxs-lookup"><span data-stu-id="53fbe-122">string</span></span>  | <span data-ttu-id="53fbe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53fbe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53fbe-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="53fbe-125">Request body</span></span>
<span data-ttu-id="53fbe-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53fbe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53fbe-127">响应</span><span class="sxs-lookup"><span data-stu-id="53fbe-127">Response</span></span>

<span data-ttu-id="53fbe-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="53fbe-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53fbe-130">示例</span><span class="sxs-lookup"><span data-stu-id="53fbe-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53fbe-131">请求</span><span class="sxs-lookup"><span data-stu-id="53fbe-131">Request</span></span>
<span data-ttu-id="53fbe-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53fbe-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="53fbe-133">响应</span><span class="sxs-lookup"><span data-stu-id="53fbe-133">Response</span></span>
<span data-ttu-id="53fbe-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53fbe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="53fbe-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="53fbe-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="53fbe-138">C#</span><span class="sxs-lookup"><span data-stu-id="53fbe-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53fbe-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="53fbe-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="53fbe-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="53fbe-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
