---
title: 获取 applicationSignInDetailedSummary
description: 检索 applicationSignInDetailSummary 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c847aefb1a7e9ab7b18821d2c002bbc96f3c1a7d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318675"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="f7b80-103">获取 applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="f7b80-103">Get applicationSignInDetailedSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7b80-104">检索[applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7b80-104">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7b80-105">权限</span><span class="sxs-lookup"><span data-stu-id="f7b80-105">Permissions</span></span>
<span data-ttu-id="f7b80-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f7b80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="f7b80-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7b80-108">Permission type</span></span>                        | <span data-ttu-id="f7b80-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7b80-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7b80-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7b80-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7b80-111">Report. All</span><span class="sxs-lookup"><span data-stu-id="f7b80-111">Report.Read.All</span></span> |
|<span data-ttu-id="f7b80-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7b80-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7b80-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7b80-113">Not supported.</span></span> |
|<span data-ttu-id="f7b80-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7b80-114">Application</span></span>                            | <span data-ttu-id="f7b80-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7b80-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7b80-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7b80-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7b80-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f7b80-117">Optional query parameters</span></span>

<span data-ttu-id="f7b80-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f7b80-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7b80-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7b80-119">Request headers</span></span>

| <span data-ttu-id="f7b80-120">名称</span><span class="sxs-lookup"><span data-stu-id="f7b80-120">Name</span></span>      |<span data-ttu-id="f7b80-121">说明</span><span class="sxs-lookup"><span data-stu-id="f7b80-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7b80-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7b80-122">Authorization</span></span> | <span data-ttu-id="f7b80-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f7b80-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7b80-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7b80-124">Request body</span></span>
<span data-ttu-id="f7b80-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7b80-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7b80-126">响应</span><span class="sxs-lookup"><span data-stu-id="f7b80-126">Response</span></span>
<span data-ttu-id="f7b80-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f7b80-127">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7b80-128">示例</span><span class="sxs-lookup"><span data-stu-id="f7b80-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7b80-129">请求</span><span class="sxs-lookup"><span data-stu-id="f7b80-129">Request</span></span>
<span data-ttu-id="f7b80-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7b80-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f7b80-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f7b80-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/<id>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7b80-132">C#</span><span class="sxs-lookup"><span data-stu-id="f7b80-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsignindetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7b80-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7b80-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsignindetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7b80-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="f7b80-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsignindetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f7b80-135">Java</span><span class="sxs-lookup"><span data-stu-id="f7b80-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationsignindetailedsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7b80-136">响应</span><span class="sxs-lookup"><span data-stu-id="f7b80-136">Response</span></span>
<span data-ttu-id="f7b80-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7b80-137">The following is an example of the response.</span></span> 

><span data-ttu-id="f7b80-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f7b80-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
