---
title: 列出 riskDetection
description: 检索 **riskDetection 对象集合** 的属性。
localization_priority: Normal
author: cloudhandler
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e7e0bb9eba36a3b6fdbd6ae03db718dc210d5424
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955524"
---
# <a name="list-riskdetection"></a><span data-ttu-id="39f2b-103">列出 riskDetection</span><span class="sxs-lookup"><span data-stu-id="39f2b-103">List riskDetection</span></span>

<span data-ttu-id="39f2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39f2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39f2b-105">检索 **riskDetection 对象集合** 的属性。</span><span class="sxs-lookup"><span data-stu-id="39f2b-105">Retrieve the properties of a collection of **riskDetection** objects.</span></span>

>[!NOTE]
><span data-ttu-id="39f2b-106">必须具有 Azure AD Premium P1 或 P2 许可证才能使用风险检测 API。</span><span class="sxs-lookup"><span data-stu-id="39f2b-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="39f2b-107">权限</span><span class="sxs-lookup"><span data-stu-id="39f2b-107">Permissions</span></span>

<span data-ttu-id="39f2b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39f2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39f2b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="39f2b-110">Permission type</span></span>      | <span data-ttu-id="39f2b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39f2b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39f2b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39f2b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="39f2b-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="39f2b-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="39f2b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39f2b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39f2b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="39f2b-115">Not supported.</span></span>    |
|<span data-ttu-id="39f2b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="39f2b-116">Application</span></span> | <span data-ttu-id="39f2b-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="39f2b-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39f2b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39f2b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections
GET /identityProtection/riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39f2b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="39f2b-119">Optional query parameters</span></span>

<span data-ttu-id="39f2b-120">此方法支持 `$filter` 并 `$select` 自定义查询响应。</span><span class="sxs-lookup"><span data-stu-id="39f2b-120">This method supports `$filter` and `$select` to customize the query response.</span></span> <span data-ttu-id="39f2b-121">请参阅本主题稍后介绍的示例。</span><span class="sxs-lookup"><span data-stu-id="39f2b-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="39f2b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="39f2b-122">Request headers</span></span>

| <span data-ttu-id="39f2b-123">名称</span><span class="sxs-lookup"><span data-stu-id="39f2b-123">Name</span></span>      |<span data-ttu-id="39f2b-124">说明</span><span class="sxs-lookup"><span data-stu-id="39f2b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39f2b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="39f2b-125">Authorization</span></span>  | <span data-ttu-id="39f2b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39f2b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39f2b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39f2b-128">Content-Type</span></span> | <span data-ttu-id="39f2b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="39f2b-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="39f2b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="39f2b-130">Request body</span></span>

<span data-ttu-id="39f2b-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="39f2b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39f2b-132">响应</span><span class="sxs-lookup"><span data-stu-id="39f2b-132">Response</span></span>

<span data-ttu-id="39f2b-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [riskDetection](../resources/riskdetection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="39f2b-133">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39f2b-134">示例</span><span class="sxs-lookup"><span data-stu-id="39f2b-134">Examples</span></span>


### <a name="example-1-list-risk-detections"></a><span data-ttu-id="39f2b-135">示例 1：列出风险检测</span><span class="sxs-lookup"><span data-stu-id="39f2b-135">Example 1: List risk detections</span></span>

#### <a name="request"></a><span data-ttu-id="39f2b-136">请求</span><span class="sxs-lookup"><span data-stu-id="39f2b-136">Request</span></span>

<span data-ttu-id="39f2b-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39f2b-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39f2b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="39f2b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="39f2b-139">C#</span><span class="sxs-lookup"><span data-stu-id="39f2b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39f2b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39f2b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39f2b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39f2b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39f2b-142">Java</span><span class="sxs-lookup"><span data-stu-id="39f2b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskdetection-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39f2b-143">响应</span><span class="sxs-lookup"><span data-stu-id="39f2b-143">Response</span></span>

<span data-ttu-id="39f2b-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="39f2b-144">Here is an example of the response.</span></span>
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
    "riskEventType": "unfamiliarFeatures",
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

### <a name="example-2-list-risk-detections-for-a-specific-user"></a><span data-ttu-id="39f2b-145">示例 2：列出特定用户的风险检测</span><span class="sxs-lookup"><span data-stu-id="39f2b-145">Example 2: List risk detections for a specific user</span></span>

#### <a name="request"></a><span data-ttu-id="39f2b-146">请求</span><span class="sxs-lookup"><span data-stu-id="39f2b-146">Request</span></span>

<span data-ttu-id="39f2b-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39f2b-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39f2b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="39f2b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="39f2b-149">C#</span><span class="sxs-lookup"><span data-stu-id="39f2b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39f2b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39f2b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39f2b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39f2b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39f2b-152">Java</span><span class="sxs-lookup"><span data-stu-id="39f2b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskdetection-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39f2b-153">响应</span><span class="sxs-lookup"><span data-stu-id="39f2b-153">Response</span></span>

<span data-ttu-id="39f2b-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="39f2b-154">Here is an example of the response.</span></span>
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
    "riskEventType": "unfamiliarFeatures",
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

### <a name="example-3-list-risk-detections-and-filter-the-results"></a><span data-ttu-id="39f2b-155">示例 3：列出风险检测并筛选结果</span><span class="sxs-lookup"><span data-stu-id="39f2b-155">Example 3: List risk detections and filter the results</span></span>

#### <a name="request"></a><span data-ttu-id="39f2b-156">请求</span><span class="sxs-lookup"><span data-stu-id="39f2b-156">Request</span></span>

<span data-ttu-id="39f2b-157">以下示例演示如何使用 获取风险级别为中等或风险事件类型为不固定Features 的风险检测集合，这表示登录位于不熟悉或异常的位置。 `$filter`</span><span class="sxs-lookup"><span data-stu-id="39f2b-157">The following example shows how to use `$filter` to get the collection of risk detections where the risk level is medium or the risk event type is unfamilarFeatures, which indicates the sign-in was in an unfamiliar or anomalous location.</span></span>


# <a name="http"></a>[<span data-ttu-id="39f2b-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="39f2b-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskDetections"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections?$filter=riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'
```
# <a name="c"></a>[<span data-ttu-id="39f2b-159">C#</span><span class="sxs-lookup"><span data-stu-id="39f2b-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskdetections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39f2b-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39f2b-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskdetections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39f2b-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39f2b-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskdetections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39f2b-162">Java</span><span class="sxs-lookup"><span data-stu-id="39f2b-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskdetections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39f2b-163">响应</span><span class="sxs-lookup"><span data-stu-id="39f2b-163">Response</span></span>

<span data-ttu-id="39f2b-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="39f2b-164">Here is an example of the response.</span></span>
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
    "riskEventType": "unfamiliarFeatures",
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


