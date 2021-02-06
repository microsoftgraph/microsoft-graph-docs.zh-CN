---
title: 获取 applicationSignInDetailedSummary
description: 检索 applicationSignInDetailSummary 对象的属性和关系。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 17f4a087d548ae06b69430c3ca442ead5ac38625
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128976"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="d6257-103">获取 applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="d6257-103">Get applicationSignInDetailedSummary</span></span>

<span data-ttu-id="d6257-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6257-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6257-105">检索 [applicationSignInDetailSummary 对象的属性和](../resources/applicationsignindetailedsummary.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d6257-105">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6257-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6257-106">Permissions</span></span>
<span data-ttu-id="d6257-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d6257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="d6257-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6257-109">Permission type</span></span>                        | <span data-ttu-id="d6257-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6257-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6257-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6257-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6257-112">Report.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6257-112">Report.Read.All</span></span> |
|<span data-ttu-id="d6257-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6257-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6257-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6257-114">Not supported.</span></span> |
|<span data-ttu-id="d6257-115">Application</span><span class="sxs-lookup"><span data-stu-id="d6257-115">Application</span></span>                            | <span data-ttu-id="d6257-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6257-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6257-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6257-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6257-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d6257-118">Optional query parameters</span></span>

<span data-ttu-id="d6257-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d6257-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6257-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6257-120">Request headers</span></span>

| <span data-ttu-id="d6257-121">名称</span><span class="sxs-lookup"><span data-stu-id="d6257-121">Name</span></span>      |<span data-ttu-id="d6257-122">说明</span><span class="sxs-lookup"><span data-stu-id="d6257-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d6257-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6257-123">Authorization</span></span> | <span data-ttu-id="d6257-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d6257-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6257-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6257-125">Request body</span></span>
<span data-ttu-id="d6257-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6257-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6257-127">响应</span><span class="sxs-lookup"><span data-stu-id="d6257-127">Response</span></span>
<span data-ttu-id="d6257-128">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6257-128">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6257-129">示例</span><span class="sxs-lookup"><span data-stu-id="d6257-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6257-130">请求</span><span class="sxs-lookup"><span data-stu-id="d6257-130">Request</span></span>
<span data-ttu-id="d6257-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d6257-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6257-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6257-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/{id}
```
# <a name="c"></a>[<span data-ttu-id="d6257-133">C#</span><span class="sxs-lookup"><span data-stu-id="d6257-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsignindetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6257-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6257-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsignindetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6257-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6257-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsignindetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6257-136">Java</span><span class="sxs-lookup"><span data-stu-id="d6257-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationsignindetailedsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d6257-137">响应</span><span class="sxs-lookup"><span data-stu-id="d6257-137">Response</span></span>
<span data-ttu-id="d6257-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d6257-138">The following is an example of the response.</span></span> 

><span data-ttu-id="d6257-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d6257-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


