---
title: 获取 riskDetection
description: 检索 **riskdetection 对象** 的属性。
localization_priority: Normal
author: cloudhandler
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 84093741d434686a9957ca657978406fe6156da7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954197"
---
# <a name="get-riskdetection"></a><span data-ttu-id="8636e-103">获取 riskDetection</span><span class="sxs-lookup"><span data-stu-id="8636e-103">Get riskDetection</span></span>

<span data-ttu-id="8636e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8636e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8636e-105">检索 **riskDetection 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="8636e-105">Retrieve the properties of a **riskDetection** object.</span></span>

>[!NOTE]
><span data-ttu-id="8636e-106">必须具有 Azure AD Premium P1 或 P2 许可证才能使用风险检测 API。</span><span class="sxs-lookup"><span data-stu-id="8636e-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="8636e-107">权限</span><span class="sxs-lookup"><span data-stu-id="8636e-107">Permissions</span></span>
<span data-ttu-id="8636e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8636e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8636e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8636e-110">Permission type</span></span>      | <span data-ttu-id="8636e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8636e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8636e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8636e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8636e-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="8636e-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="8636e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8636e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8636e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8636e-115">Not supported.</span></span>    |
|<span data-ttu-id="8636e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8636e-116">Application</span></span> | <span data-ttu-id="8636e-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="8636e-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8636e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8636e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections/{id}
GET /identityProtection/riskDetections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8636e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8636e-119">Request headers</span></span>
| <span data-ttu-id="8636e-120">名称</span><span class="sxs-lookup"><span data-stu-id="8636e-120">Name</span></span>      |<span data-ttu-id="8636e-121">说明</span><span class="sxs-lookup"><span data-stu-id="8636e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8636e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8636e-122">Authorization</span></span>  | <span data-ttu-id="8636e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8636e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8636e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8636e-125">Content-Type</span></span> | <span data-ttu-id="8636e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8636e-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8636e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8636e-127">Request body</span></span>
<span data-ttu-id="8636e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8636e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8636e-129">响应</span><span class="sxs-lookup"><span data-stu-id="8636e-129">Response</span></span>

<span data-ttu-id="8636e-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [riskDetection](../resources/riskdetection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8636e-130">If successful, this method returns a `200 OK` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8636e-131">示例</span><span class="sxs-lookup"><span data-stu-id="8636e-131">Examples</span></span>
### <a name="example-1-get-risk-detections"></a><span data-ttu-id="8636e-132">示例 1：获取风险检测</span><span class="sxs-lookup"><span data-stu-id="8636e-132">Example 1: Get risk detections</span></span>
#### <a name="request"></a><span data-ttu-id="8636e-133">请求</span><span class="sxs-lookup"><span data-stu-id="8636e-133">Request</span></span>
<span data-ttu-id="8636e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8636e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8636e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8636e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection_1",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="8636e-136">C#</span><span class="sxs-lookup"><span data-stu-id="8636e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8636e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8636e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8636e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8636e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8636e-139">Java</span><span class="sxs-lookup"><span data-stu-id="8636e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskdetection-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8636e-140">响应</span><span class="sxs-lookup"><span data-stu-id="8636e-140">Response</span></span>
<span data-ttu-id="8636e-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8636e-141">Here is an example of the response.</span></span>
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
### <a name="example-2-get-risk-detections-for-specific-user"></a><span data-ttu-id="8636e-142">示例 2：获取特定用户的风险检测</span><span class="sxs-lookup"><span data-stu-id="8636e-142">Example 2: Get risk detections for specific user</span></span>
#### <a name="request"></a><span data-ttu-id="8636e-143">请求</span><span class="sxs-lookup"><span data-stu-id="8636e-143">Request</span></span>
<span data-ttu-id="8636e-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8636e-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8636e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="8636e-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection_2",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="8636e-146">C#</span><span class="sxs-lookup"><span data-stu-id="8636e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8636e-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8636e-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8636e-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8636e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8636e-149">Java</span><span class="sxs-lookup"><span data-stu-id="8636e-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskdetection-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8636e-150">响应</span><span class="sxs-lookup"><span data-stu-id="8636e-150">Response</span></span>
<span data-ttu-id="8636e-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8636e-151">Here is an example of the response.</span></span>
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



