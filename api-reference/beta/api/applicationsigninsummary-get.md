---
title: 获取 applicationSignInSummary
description: 检索 **applicationSigninSummary** 对象的属性和关系。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cbc72087d34473345d359ba6b57653226ea03e64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996680"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="6b13d-103">获取 applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="6b13d-103">Get applicationSignInSummary</span></span>

<span data-ttu-id="6b13d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b13d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b13d-105">检索 [applicationSigninSummary](../resources/applicationsigninsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6b13d-105">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b13d-106">权限</span><span class="sxs-lookup"><span data-stu-id="6b13d-106">Permissions</span></span>
<span data-ttu-id="6b13d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6b13d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="6b13d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b13d-109">Permission type</span></span>      | <span data-ttu-id="6b13d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b13d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b13d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b13d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b13d-112">Report. All</span><span class="sxs-lookup"><span data-stu-id="6b13d-112">Report.Read.All</span></span> |
|<span data-ttu-id="6b13d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b13d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b13d-114">不支持</span><span class="sxs-lookup"><span data-stu-id="6b13d-114">Not supported</span></span>   |
|<span data-ttu-id="6b13d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b13d-115">Application</span></span> | <span data-ttu-id="6b13d-116">Report. All</span><span class="sxs-lookup"><span data-stu-id="6b13d-116">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6b13d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b13d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="6b13d-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="6b13d-118">Function parameters</span></span>

| <span data-ttu-id="6b13d-119">参数</span><span class="sxs-lookup"><span data-stu-id="6b13d-119">Parameter</span></span> | <span data-ttu-id="6b13d-120">说明</span><span class="sxs-lookup"><span data-stu-id="6b13d-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="6b13d-121">period</span><span class="sxs-lookup"><span data-stu-id="6b13d-121">period</span></span> | <span data-ttu-id="6b13d-122">`D7` (最近七天) 或 `D30` (最近30天) ; 其他值会产生错误。</span><span class="sxs-lookup"><span data-stu-id="6b13d-122">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6b13d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b13d-123">Request headers</span></span>
| <span data-ttu-id="6b13d-124">名称</span><span class="sxs-lookup"><span data-stu-id="6b13d-124">Name</span></span>      |<span data-ttu-id="6b13d-125">说明</span><span class="sxs-lookup"><span data-stu-id="6b13d-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6b13d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b13d-126">Authorization</span></span> | <span data-ttu-id="6b13d-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6b13d-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b13d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b13d-128">Request body</span></span>
<span data-ttu-id="6b13d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b13d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b13d-130">响应</span><span class="sxs-lookup"><span data-stu-id="6b13d-130">Response</span></span>
<span data-ttu-id="6b13d-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [applicationSignInSummary](../resources/applicationsigninsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b13d-131">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b13d-132">示例</span><span class="sxs-lookup"><span data-stu-id="6b13d-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6b13d-133">请求</span><span class="sxs-lookup"><span data-stu-id="6b13d-133">Request</span></span>
<span data-ttu-id="6b13d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6b13d-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b13d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b13d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="6b13d-136">C#</span><span class="sxs-lookup"><span data-stu-id="6b13d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsigninsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b13d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b13d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsigninsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b13d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b13d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsigninsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6b13d-139">响应</span><span class="sxs-lookup"><span data-stu-id="6b13d-139">Response</span></span>
<span data-ttu-id="6b13d-140">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="6b13d-140">The following is an example of the response.</span></span> 

><span data-ttu-id="6b13d-141">**注意：** 在此处显示的响应对象将缩短 mmight 以提高可读性。</span><span class="sxs-lookup"><span data-stu-id="6b13d-141">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="6b13d-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6b13d-142">All the properties will be returned from an actual call.</span></span>
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


