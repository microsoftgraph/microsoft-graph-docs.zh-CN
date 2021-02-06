---
title: 获取 applicationSignInSummary
description: 检索 **applicationSigninSummary** 对象的属性和关系。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 9fad0f7122a1d82cb1f0dfc2ca7172f7f4029e85
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128972"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="adb81-103">获取 applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="adb81-103">Get applicationSignInSummary</span></span>

<span data-ttu-id="adb81-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adb81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adb81-105">检索 [applicationSigninSummary](../resources/applicationsigninsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="adb81-105">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="adb81-106">权限</span><span class="sxs-lookup"><span data-stu-id="adb81-106">Permissions</span></span>
<span data-ttu-id="adb81-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="adb81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="adb81-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="adb81-109">Permission type</span></span>      | <span data-ttu-id="adb81-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="adb81-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adb81-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adb81-111">Delegated (work or school account)</span></span> | <span data-ttu-id="adb81-112">Report.Read.All</span><span class="sxs-lookup"><span data-stu-id="adb81-112">Report.Read.All</span></span> |
|<span data-ttu-id="adb81-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adb81-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adb81-114">不支持</span><span class="sxs-lookup"><span data-stu-id="adb81-114">Not supported</span></span>   |
|<span data-ttu-id="adb81-115">Application</span><span class="sxs-lookup"><span data-stu-id="adb81-115">Application</span></span> | <span data-ttu-id="adb81-116">Report.Read.All</span><span class="sxs-lookup"><span data-stu-id="adb81-116">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="adb81-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adb81-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="adb81-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="adb81-118">Function parameters</span></span>

| <span data-ttu-id="adb81-119">参数</span><span class="sxs-lookup"><span data-stu-id="adb81-119">Parameter</span></span> | <span data-ttu-id="adb81-120">说明</span><span class="sxs-lookup"><span data-stu-id="adb81-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="adb81-121">period</span><span class="sxs-lookup"><span data-stu-id="adb81-121">period</span></span> | <span data-ttu-id="adb81-122">如果 (最近七天) ， (最近 30) 天;其他值 `D7` `D30` 将生成错误。</span><span class="sxs-lookup"><span data-stu-id="adb81-122">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="adb81-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="adb81-123">Request headers</span></span>
| <span data-ttu-id="adb81-124">名称</span><span class="sxs-lookup"><span data-stu-id="adb81-124">Name</span></span>      |<span data-ttu-id="adb81-125">说明</span><span class="sxs-lookup"><span data-stu-id="adb81-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="adb81-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="adb81-126">Authorization</span></span> | <span data-ttu-id="adb81-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="adb81-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="adb81-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="adb81-128">Request body</span></span>
<span data-ttu-id="adb81-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="adb81-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adb81-130">响应</span><span class="sxs-lookup"><span data-stu-id="adb81-130">Response</span></span>
<span data-ttu-id="adb81-131">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [applicationSignInSummary](../resources/applicationsigninsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="adb81-131">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adb81-132">示例</span><span class="sxs-lookup"><span data-stu-id="adb81-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="adb81-133">请求</span><span class="sxs-lookup"><span data-stu-id="adb81-133">Request</span></span>
<span data-ttu-id="adb81-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adb81-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="adb81-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="adb81-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="adb81-136">C#</span><span class="sxs-lookup"><span data-stu-id="adb81-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsigninsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adb81-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adb81-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsigninsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adb81-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adb81-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsigninsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adb81-139">Java</span><span class="sxs-lookup"><span data-stu-id="adb81-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationsigninsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="adb81-140">响应</span><span class="sxs-lookup"><span data-stu-id="adb81-140">Response</span></span>
<span data-ttu-id="adb81-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="adb81-141">The following is an example of the response.</span></span> 

><span data-ttu-id="adb81-142">**注意：** 为了可读性，缩短了此处 mmight 所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="adb81-142">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="adb81-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="adb81-143">All the properties will be returned from an actual call.</span></span>
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


