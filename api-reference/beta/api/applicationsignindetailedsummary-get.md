---
title: 获取 applicationSignInDetailedSummary
description: 检索 applicationSignInDetailSummary 对象的属性和关系。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c209b42d9b18ec0fc935c588a42e98a9c62c42e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996715"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="d6f97-103">获取 applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="d6f97-103">Get applicationSignInDetailedSummary</span></span>

<span data-ttu-id="d6f97-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6f97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6f97-105">检索 [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d6f97-105">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6f97-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6f97-106">Permissions</span></span>
<span data-ttu-id="d6f97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d6f97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="d6f97-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6f97-109">Permission type</span></span>                        | <span data-ttu-id="d6f97-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6f97-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6f97-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6f97-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6f97-112">Report. All</span><span class="sxs-lookup"><span data-stu-id="d6f97-112">Report.Read.All</span></span> |
|<span data-ttu-id="d6f97-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6f97-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6f97-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6f97-114">Not supported.</span></span> |
|<span data-ttu-id="d6f97-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6f97-115">Application</span></span>                            | <span data-ttu-id="d6f97-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6f97-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6f97-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6f97-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6f97-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d6f97-118">Optional query parameters</span></span>

<span data-ttu-id="d6f97-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d6f97-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6f97-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6f97-120">Request headers</span></span>

| <span data-ttu-id="d6f97-121">名称</span><span class="sxs-lookup"><span data-stu-id="d6f97-121">Name</span></span>      |<span data-ttu-id="d6f97-122">说明</span><span class="sxs-lookup"><span data-stu-id="d6f97-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d6f97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6f97-123">Authorization</span></span> | <span data-ttu-id="d6f97-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d6f97-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6f97-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6f97-125">Request body</span></span>
<span data-ttu-id="d6f97-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6f97-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6f97-127">响应</span><span class="sxs-lookup"><span data-stu-id="d6f97-127">Response</span></span>
<span data-ttu-id="d6f97-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6f97-128">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6f97-129">示例</span><span class="sxs-lookup"><span data-stu-id="d6f97-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6f97-130">请求</span><span class="sxs-lookup"><span data-stu-id="d6f97-130">Request</span></span>
<span data-ttu-id="d6f97-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d6f97-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6f97-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6f97-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/{id}
```
# <a name="c"></a>[<span data-ttu-id="d6f97-133">C#</span><span class="sxs-lookup"><span data-stu-id="d6f97-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsignindetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6f97-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6f97-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsignindetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6f97-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6f97-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsignindetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d6f97-136">响应</span><span class="sxs-lookup"><span data-stu-id="d6f97-136">Response</span></span>
<span data-ttu-id="d6f97-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d6f97-137">The following is an example of the response.</span></span> 

><span data-ttu-id="d6f97-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d6f97-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


