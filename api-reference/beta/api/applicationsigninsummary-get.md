---
title: 获取 applicationSignInSummary
description: 检索**applicationSigninSummary**对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 408a148973d37297f2bbd0bf48a0eee64a914d0f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439551"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="1b990-103">获取 applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="1b990-103">Get applicationSignInSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b990-104">检索[applicationSigninSummary](../resources/applicationsigninsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b990-104">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b990-105">权限</span><span class="sxs-lookup"><span data-stu-id="1b990-105">Permissions</span></span>
<span data-ttu-id="1b990-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1b990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="1b990-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b990-108">Permission type</span></span>      | <span data-ttu-id="1b990-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b990-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b990-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b990-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1b990-111">Report. All</span><span class="sxs-lookup"><span data-stu-id="1b990-111">Report.Read.All</span></span> |
|<span data-ttu-id="1b990-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b990-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b990-113">不支持</span><span class="sxs-lookup"><span data-stu-id="1b990-113">Not supported</span></span>   |
|<span data-ttu-id="1b990-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b990-114">Application</span></span> | <span data-ttu-id="1b990-115">Report. All</span><span class="sxs-lookup"><span data-stu-id="1b990-115">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1b990-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b990-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="1b990-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="1b990-117">Function parameters</span></span>

| <span data-ttu-id="1b990-118">参数</span><span class="sxs-lookup"><span data-stu-id="1b990-118">Parameter</span></span> | <span data-ttu-id="1b990-119">说明</span><span class="sxs-lookup"><span data-stu-id="1b990-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="1b990-120">period</span><span class="sxs-lookup"><span data-stu-id="1b990-120">period</span></span> | <span data-ttu-id="1b990-121">`D7` (最近七天) 或`D30` (最近30天);其他值会生成错误。</span><span class="sxs-lookup"><span data-stu-id="1b990-121">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1b990-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b990-122">Request headers</span></span>
| <span data-ttu-id="1b990-123">名称</span><span class="sxs-lookup"><span data-stu-id="1b990-123">Name</span></span>      |<span data-ttu-id="1b990-124">说明</span><span class="sxs-lookup"><span data-stu-id="1b990-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b990-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b990-125">Authorization</span></span> | <span data-ttu-id="1b990-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1b990-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b990-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b990-127">Request body</span></span>
<span data-ttu-id="1b990-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1b990-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b990-129">响应</span><span class="sxs-lookup"><span data-stu-id="1b990-129">Response</span></span>
<span data-ttu-id="1b990-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[applicationSignInSummary](../resources/applicationsigninsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b990-130">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b990-131">示例</span><span class="sxs-lookup"><span data-stu-id="1b990-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1b990-132">请求</span><span class="sxs-lookup"><span data-stu-id="1b990-132">Request</span></span>
<span data-ttu-id="1b990-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b990-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1b990-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1b990-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b990-135">C#</span><span class="sxs-lookup"><span data-stu-id="1b990-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsigninsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b990-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="1b990-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsigninsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b990-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="1b990-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsigninsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1b990-138">响应</span><span class="sxs-lookup"><span data-stu-id="1b990-138">Response</span></span>
<span data-ttu-id="1b990-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1b990-139">The following is an example of the response.</span></span> 

><span data-ttu-id="1b990-140">**注意:** 在此处显示的响应对象将缩短 mmight 以提高可读性。</span><span class="sxs-lookup"><span data-stu-id="1b990-140">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="1b990-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1b990-141">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
