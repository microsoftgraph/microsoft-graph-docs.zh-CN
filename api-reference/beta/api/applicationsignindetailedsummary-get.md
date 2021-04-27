---
title: 获取 applicationSignInDetailedSummary
description: 检索 applicationSignInDetailSummary 对象的属性和关系。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 5bb2acdcc76b26aac6ebd851359a4c85a0441015
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048069"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="ea808-103">获取 applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="ea808-103">Get applicationSignInDetailedSummary</span></span>

<span data-ttu-id="ea808-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea808-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea808-105">检索 [applicationSignInDetailSummary 对象的属性和](../resources/applicationsignindetailedsummary.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="ea808-105">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea808-106">权限</span><span class="sxs-lookup"><span data-stu-id="ea808-106">Permissions</span></span>
<span data-ttu-id="ea808-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ea808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="ea808-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea808-109">Permission type</span></span>                        | <span data-ttu-id="ea808-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea808-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea808-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea808-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea808-112">Report.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea808-112">Report.Read.All</span></span> |
|<span data-ttu-id="ea808-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea808-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea808-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea808-114">Not supported.</span></span> |
|<span data-ttu-id="ea808-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea808-115">Application</span></span>                            | <span data-ttu-id="ea808-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea808-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea808-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea808-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea808-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ea808-118">Optional query parameters</span></span>

<span data-ttu-id="ea808-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ea808-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea808-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea808-120">Request headers</span></span>

| <span data-ttu-id="ea808-121">名称</span><span class="sxs-lookup"><span data-stu-id="ea808-121">Name</span></span>      |<span data-ttu-id="ea808-122">说明</span><span class="sxs-lookup"><span data-stu-id="ea808-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ea808-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea808-123">Authorization</span></span> | <span data-ttu-id="ea808-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ea808-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea808-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea808-125">Request body</span></span>
<span data-ttu-id="ea808-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea808-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea808-127">响应</span><span class="sxs-lookup"><span data-stu-id="ea808-127">Response</span></span>
<span data-ttu-id="ea808-128">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea808-128">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea808-129">示例</span><span class="sxs-lookup"><span data-stu-id="ea808-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea808-130">请求</span><span class="sxs-lookup"><span data-stu-id="ea808-130">Request</span></span>
<span data-ttu-id="ea808-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ea808-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea808-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea808-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/{id}
```
# <a name="c"></a>[<span data-ttu-id="ea808-133">C#</span><span class="sxs-lookup"><span data-stu-id="ea808-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsignindetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea808-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea808-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsignindetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea808-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea808-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsignindetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea808-136">Java</span><span class="sxs-lookup"><span data-stu-id="ea808-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationsignindetailedsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ea808-137">响应</span><span class="sxs-lookup"><span data-stu-id="ea808-137">Response</span></span>
<span data-ttu-id="ea808-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ea808-138">The following is an example of the response.</span></span> 

><span data-ttu-id="ea808-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ea808-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 295

{
  "id": "id-value",
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "status": {
    "errorCode": 99,
    "failureReason": "failureReason-value",
    "additionalDetails": "additionalDetails-value"
  },
  "signInCount": 99,
  "aggregatedEventDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInDetailedSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


