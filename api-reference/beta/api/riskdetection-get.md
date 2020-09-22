---
title: 获取 riskDetection
description: 检索 **riskdetection** 对象的属性。
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 80b1099fa2641973bfe842311f0086fd09fffcd4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052927"
---
# <a name="get-riskdetection"></a><span data-ttu-id="3d200-103">获取 riskDetection</span><span class="sxs-lookup"><span data-stu-id="3d200-103">Get riskDetection</span></span>

<span data-ttu-id="3d200-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d200-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d200-105">检索 **riskDetection** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3d200-105">Retrieve the properties of a **riskDetection** object.</span></span>

>[!NOTE]
><span data-ttu-id="3d200-106">您必须具有 Azure AD 高级 P1 或 P2 许可证，才能使用风险检测 API。</span><span class="sxs-lookup"><span data-stu-id="3d200-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d200-107">权限</span><span class="sxs-lookup"><span data-stu-id="3d200-107">Permissions</span></span>
<span data-ttu-id="3d200-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d200-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d200-110">Permission type</span></span>      | <span data-ttu-id="3d200-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3d200-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d200-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d200-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3d200-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d200-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="3d200-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d200-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d200-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d200-115">Not supported.</span></span>    |
|<span data-ttu-id="3d200-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d200-116">Application</span></span> | <span data-ttu-id="3d200-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d200-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d200-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d200-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections/{id}
GET /identityProtection/riskDetections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3d200-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d200-119">Request headers</span></span>
| <span data-ttu-id="3d200-120">名称</span><span class="sxs-lookup"><span data-stu-id="3d200-120">Name</span></span>      |<span data-ttu-id="3d200-121">说明</span><span class="sxs-lookup"><span data-stu-id="3d200-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3d200-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d200-122">Authorization</span></span>  | <span data-ttu-id="3d200-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3d200-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d200-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d200-125">Content-Type</span></span> | <span data-ttu-id="3d200-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d200-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d200-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d200-127">Request body</span></span>
<span data-ttu-id="3d200-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3d200-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d200-129">响应</span><span class="sxs-lookup"><span data-stu-id="3d200-129">Response</span></span>

<span data-ttu-id="3d200-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [riskDetection](../resources/riskdetection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d200-130">If successful, this method returns a `200 OK` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3d200-131">示例</span><span class="sxs-lookup"><span data-stu-id="3d200-131">Examples</span></span>
### <a name="example-1-get-risk-detections"></a><span data-ttu-id="3d200-132">示例1：获取风险检测</span><span class="sxs-lookup"><span data-stu-id="3d200-132">Example 1: Get risk detections</span></span>
#### <a name="request"></a><span data-ttu-id="3d200-133">请求</span><span class="sxs-lookup"><span data-stu-id="3d200-133">Request</span></span>
<span data-ttu-id="3d200-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d200-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3d200-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d200-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="3d200-136">C#</span><span class="sxs-lookup"><span data-stu-id="3d200-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d200-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d200-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d200-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d200-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3d200-139">响应</span><span class="sxs-lookup"><span data-stu-id="3d200-139">Response</span></span>
<span data-ttu-id="3d200-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3d200-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
    "userDisplayName": "Olivia Lack",
    "userPrincipalName": "olack@adatum.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
}
```
### <a name="example-2-get-risk-detections-for-specific-user"></a><span data-ttu-id="3d200-141">示例2：获取特定用户的风险检测项</span><span class="sxs-lookup"><span data-stu-id="3d200-141">Example 2: Get risk detections for specific user</span></span>
#### <a name="request"></a><span data-ttu-id="3d200-142">请求</span><span class="sxs-lookup"><span data-stu-id="3d200-142">Request</span></span>
<span data-ttu-id="3d200-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d200-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3d200-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d200-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="3d200-145">C#</span><span class="sxs-lookup"><span data-stu-id="3d200-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d200-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d200-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d200-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d200-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3d200-148">响应</span><span class="sxs-lookup"><span data-stu-id="3d200-148">Response</span></span>
<span data-ttu-id="3d200-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3d200-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
    "userDisplayName": "Olivia Lack",
    "userPrincipalName": "olack@adatum.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskDetection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



