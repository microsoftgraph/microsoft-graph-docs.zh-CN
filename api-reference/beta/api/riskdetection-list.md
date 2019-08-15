---
title: 列出 riskDetection
description: 检索**riskDetection**对象的集合的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3497f19e4a1348cd42ae9ba272eca551ee676cb2
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410897"
---
# <a name="list-riskdetection"></a><span data-ttu-id="5ab84-103">列出 riskDetection</span><span class="sxs-lookup"><span data-stu-id="5ab84-103">List riskDetection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ab84-104">检索**riskDetection**对象的集合的属性。</span><span class="sxs-lookup"><span data-stu-id="5ab84-104">Retrieve the properties of a collection of **riskDetection** objects.</span></span>

>[!NOTE]
><span data-ttu-id="5ab84-105">您必须具有 Azure AD 高级 P2 许可证才能使用风险检测 API。</span><span class="sxs-lookup"><span data-stu-id="5ab84-105">You must have an Azure AD Premium P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ab84-106">权限</span><span class="sxs-lookup"><span data-stu-id="5ab84-106">Permissions</span></span>

<span data-ttu-id="5ab84-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ab84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ab84-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ab84-109">Permission type</span></span>      | <span data-ttu-id="5ab84-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ab84-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ab84-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ab84-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ab84-112">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ab84-112">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="5ab84-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ab84-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ab84-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ab84-114">Not supported.</span></span>    |
|<span data-ttu-id="5ab84-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ab84-115">Application</span></span> | <span data-ttu-id="5ab84-116">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ab84-116">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ab84-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ab84-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ab84-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5ab84-118">Optional query parameters</span></span>

<span data-ttu-id="5ab84-119">此方法支持`$filter`和`$select`自定义查询响应。</span><span class="sxs-lookup"><span data-stu-id="5ab84-119">This method supports `$filter` and `$select` to customize the query response.</span></span> <span data-ttu-id="5ab84-120">请参阅本主题后面的示例。</span><span class="sxs-lookup"><span data-stu-id="5ab84-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="5ab84-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ab84-121">Request headers</span></span>

| <span data-ttu-id="5ab84-122">名称</span><span class="sxs-lookup"><span data-stu-id="5ab84-122">Name</span></span>      |<span data-ttu-id="5ab84-123">说明</span><span class="sxs-lookup"><span data-stu-id="5ab84-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ab84-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ab84-124">Authorization</span></span>  | <span data-ttu-id="5ab84-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ab84-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ab84-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ab84-127">Content-Type</span></span> | <span data-ttu-id="5ab84-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5ab84-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ab84-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ab84-129">Request body</span></span>

<span data-ttu-id="5ab84-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ab84-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ab84-131">响应</span><span class="sxs-lookup"><span data-stu-id="5ab84-131">Response</span></span>

<span data-ttu-id="5ab84-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[riskDetection](../resources/riskdetection.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="5ab84-132">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ab84-133">示例</span><span class="sxs-lookup"><span data-stu-id="5ab84-133">Examples</span></span>

### <a name="example-1-list-risk-detections"></a><span data-ttu-id="5ab84-134">示例 1: 列出风险检测项</span><span class="sxs-lookup"><span data-stu-id="5ab84-134">Example 1: List risk detections</span></span>

#### <a name="request"></a><span data-ttu-id="5ab84-135">请求</span><span class="sxs-lookup"><span data-stu-id="5ab84-135">Request</span></span>

<span data-ttu-id="5ab84-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ab84-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5ab84-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5ab84-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection"
}-->

```http
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5ab84-138">C#</span><span class="sxs-lookup"><span data-stu-id="5ab84-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ab84-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ab84-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5ab84-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="5ab84-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5ab84-141">响应</span><span class="sxs-lookup"><span data-stu-id="5ab84-141">Response</span></span>

<span data-ttu-id="5ab84-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5ab84-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
    "id": "6a5874ca-abcd-9d82-5ad39bd71600",
    "requestId": "6a5874ca-abcd-9d82-5ad39bd71600",
    "correlationId": "abcd74ca-9823-4b1c-9d82-5ad39bd71600",
    "riskType": "unfamiliarFeatures",
    "riskState": "remediated",
    "riskLevel": "medium",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "source": "activeDirectory",
    "detectionTimingType": "realtime",
    "activity": "signin",
    "tokenIssuerType": "Azure Active Directory",
    "ipAddress": "123.456.7.89",
    "location": {
        "city": "Seattle",
        "state": "Washington",
        "countryOrRegion": "US",
        "geoCoordinates": null
    },
    "activityDateTime": "2018-09-05T00:09:18.7822851Z",
    "detectedDateTime": "2018-09-05T00:11:27.773602Z",
    "lastUpdatedDateTime": "2018-09-05T00:11:27.773602Z",
    "userId": "abcdefab-af90-4edf-ac4c-742ff06735d0",
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

### <a name="example-2-list-risk-detections-and-filter-the-results"></a><span data-ttu-id="5ab84-143">示例 2: 列出风险检测并筛选结果</span><span class="sxs-lookup"><span data-stu-id="5ab84-143">Example 2: List risk detections and filter the results</span></span>

#### <a name="request"></a><span data-ttu-id="5ab84-144">请求</span><span class="sxs-lookup"><span data-stu-id="5ab84-144">Request</span></span>

<span data-ttu-id="5ab84-145">下面的示例演示如何使用`$filter`来获取风险级别为 "中" 或风险事件类型为 "unfamilarFeatures" 的风险检测集, 这表明登录处于不熟悉或异常的位置。</span><span class="sxs-lookup"><span data-stu-id="5ab84-145">The following example shows how to use `$filter` to get the collection of risk detections where the risk level is medium or the risk event type is unfamilarFeatures, which indicates the sign-in was in an unfamiliar or anomalous location.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5ab84-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5ab84-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskDetections"
} -->

```http
GET https://graph.microsoft.com/beta/riskDetections?$filter=riskType eq 'unfamiliarFeatures' or riskLevel eq 'medium'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5ab84-147">C#</span><span class="sxs-lookup"><span data-stu-id="5ab84-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskdetections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ab84-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ab84-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskdetections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5ab84-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="5ab84-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskdetections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5ab84-150">响应</span><span class="sxs-lookup"><span data-stu-id="5ab84-150">Response</span></span>

<span data-ttu-id="5ab84-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5ab84-151">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
    "id": "1d68fc3d60d012ff80ad4b16818bf304df1bde295fdf1db31fa5389ba9532cd1",
    "requestId": "3295073e-04b1-4871-9d15-c1f871b41100",
    "correlationId": "f141d8e5-93e9-4fd0-9eb0-c40e5f8fc092",
    "riskType": "unfamiliarFeatures",
    "riskState": "atRisk",
    "riskLevel": "medium",
    "riskDetail": "none",
    "source": "Identity Protection",
    "detectionTimingType": "realtime",
    "activity": "signin",
    "tokenIssuerType": "Azure Active Directory",
    "ipAddress": "123.456.7.89",
    "location": {
        "city": "Seattle",
        "state": "Washington",
        "countryOrRegion": "US",
        "geoCoordinates": null
    },
    "activityDateTime": "2018-09-05T00:09:18.7822851Z",
    "detectedDateTime": "2018-09-05T00:11:27.773602Z",
    "lastUpdatedDateTime": "2018-09-05T00:11:27.773602Z",
    "userId": "abcdefab-af90-4edf-ac4c-742ff06735d0",
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskDetections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
