---
title: 获取 applicationSignInSummary
description: 检索**applicationSigninSummary**对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3b1c87d3481d25f820f625532a6d421eada46114
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441422"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="f172f-103">获取 applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="f172f-103">Get applicationSignInSummary</span></span>

<span data-ttu-id="f172f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f172f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f172f-105">检索[applicationSigninSummary](../resources/applicationsigninsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f172f-105">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f172f-106">权限</span><span class="sxs-lookup"><span data-stu-id="f172f-106">Permissions</span></span>
<span data-ttu-id="f172f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f172f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="f172f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f172f-109">Permission type</span></span>      | <span data-ttu-id="f172f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f172f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f172f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f172f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f172f-112">Report. All</span><span class="sxs-lookup"><span data-stu-id="f172f-112">Report.Read.All</span></span> |
|<span data-ttu-id="f172f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f172f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f172f-114">不支持</span><span class="sxs-lookup"><span data-stu-id="f172f-114">Not supported</span></span>   |
|<span data-ttu-id="f172f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f172f-115">Application</span></span> | <span data-ttu-id="f172f-116">Report. All</span><span class="sxs-lookup"><span data-stu-id="f172f-116">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f172f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f172f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="f172f-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="f172f-118">Function parameters</span></span>

| <span data-ttu-id="f172f-119">参数</span><span class="sxs-lookup"><span data-stu-id="f172f-119">Parameter</span></span> | <span data-ttu-id="f172f-120">说明</span><span class="sxs-lookup"><span data-stu-id="f172f-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="f172f-121">period</span><span class="sxs-lookup"><span data-stu-id="f172f-121">period</span></span> | <span data-ttu-id="f172f-122">`D7` （最近七天）或`D30` （最近30天）;其他值会生成错误。</span><span class="sxs-lookup"><span data-stu-id="f172f-122">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f172f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f172f-123">Request headers</span></span>
| <span data-ttu-id="f172f-124">名称</span><span class="sxs-lookup"><span data-stu-id="f172f-124">Name</span></span>      |<span data-ttu-id="f172f-125">说明</span><span class="sxs-lookup"><span data-stu-id="f172f-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f172f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f172f-126">Authorization</span></span> | <span data-ttu-id="f172f-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f172f-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f172f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f172f-128">Request body</span></span>
<span data-ttu-id="f172f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f172f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f172f-130">响应</span><span class="sxs-lookup"><span data-stu-id="f172f-130">Response</span></span>
<span data-ttu-id="f172f-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[applicationSignInSummary](../resources/applicationsigninsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f172f-131">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f172f-132">示例</span><span class="sxs-lookup"><span data-stu-id="f172f-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f172f-133">请求</span><span class="sxs-lookup"><span data-stu-id="f172f-133">Request</span></span>
<span data-ttu-id="f172f-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f172f-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f172f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f172f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="f172f-136">C#</span><span class="sxs-lookup"><span data-stu-id="f172f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsigninsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f172f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f172f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsigninsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f172f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f172f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsigninsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f172f-139">响应</span><span class="sxs-lookup"><span data-stu-id="f172f-139">Response</span></span>
<span data-ttu-id="f172f-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f172f-140">The following is an example of the response.</span></span> 

><span data-ttu-id="f172f-141">**注意：** 在此处显示的响应对象将缩短 mmight 以提高可读性。</span><span class="sxs-lookup"><span data-stu-id="f172f-141">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="f172f-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f172f-142">All the properties will be returned from an actual call.</span></span>
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
