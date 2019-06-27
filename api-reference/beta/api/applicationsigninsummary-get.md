---
title: 获取 applicationSignInSummary
description: 检索**applicationSigninSummary**对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb9dfa4f57226ed846fcf7e7b6668214ad4be7ca
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258392"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="d456f-103">获取 applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="d456f-103">Get applicationSignInSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d456f-104">检索[applicationSigninSummary](../resources/applicationsigninsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d456f-104">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d456f-105">权限</span><span class="sxs-lookup"><span data-stu-id="d456f-105">Permissions</span></span>
<span data-ttu-id="d456f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d456f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="d456f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d456f-108">Permission type</span></span>      | <span data-ttu-id="d456f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d456f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d456f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d456f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d456f-111">Report. All</span><span class="sxs-lookup"><span data-stu-id="d456f-111">Report.Read.All</span></span> |
|<span data-ttu-id="d456f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d456f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d456f-113">不支持</span><span class="sxs-lookup"><span data-stu-id="d456f-113">Not supported</span></span>   |
|<span data-ttu-id="d456f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d456f-114">Application</span></span> | <span data-ttu-id="d456f-115">Report. All</span><span class="sxs-lookup"><span data-stu-id="d456f-115">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d456f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d456f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="d456f-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="d456f-117">Function parameters</span></span>

| <span data-ttu-id="d456f-118">参数</span><span class="sxs-lookup"><span data-stu-id="d456f-118">Parameter</span></span> | <span data-ttu-id="d456f-119">说明</span><span class="sxs-lookup"><span data-stu-id="d456f-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="d456f-120">period</span><span class="sxs-lookup"><span data-stu-id="d456f-120">period</span></span> | <span data-ttu-id="d456f-121">`D7` (最近七天) 或`D30` (最近30天);其他值会生成错误。</span><span class="sxs-lookup"><span data-stu-id="d456f-121">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d456f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d456f-122">Request headers</span></span>
| <span data-ttu-id="d456f-123">名称</span><span class="sxs-lookup"><span data-stu-id="d456f-123">Name</span></span>      |<span data-ttu-id="d456f-124">说明</span><span class="sxs-lookup"><span data-stu-id="d456f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d456f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d456f-125">Authorization</span></span> | <span data-ttu-id="d456f-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d456f-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d456f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d456f-127">Request body</span></span>
<span data-ttu-id="d456f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d456f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d456f-129">响应</span><span class="sxs-lookup"><span data-stu-id="d456f-129">Response</span></span>
<span data-ttu-id="d456f-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[applicationSignInSummary](../resources/applicationsigninsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d456f-130">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d456f-131">示例</span><span class="sxs-lookup"><span data-stu-id="d456f-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d456f-132">请求</span><span class="sxs-lookup"><span data-stu-id="d456f-132">Request</span></span>
<span data-ttu-id="d456f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d456f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
### <a name="response"></a><span data-ttu-id="d456f-134">响应</span><span class="sxs-lookup"><span data-stu-id="d456f-134">Response</span></span>
<span data-ttu-id="d456f-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d456f-135">The following is an example of the response.</span></span> 

><span data-ttu-id="d456f-136">**注意:** 在此处显示的响应对象将缩短 mmight 以提高可读性。</span><span class="sxs-lookup"><span data-stu-id="d456f-136">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="d456f-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d456f-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "successfulSignInCount": 99,
  "failedSignInCount": 99,
  "successPercentage": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d456f-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d456f-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d456f-139">C#</span><span class="sxs-lookup"><span data-stu-id="d456f-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_applicationsigninsummary-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d456f-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="d456f-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_applicationsigninsummary-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d456f-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="d456f-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_applicationsigninsummary-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/applicationsigninsummary-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/applicationsigninsummary-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/applicationsigninsummary-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
