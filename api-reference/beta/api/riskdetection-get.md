---
title: 获取 riskDetection
description: 检索**riskdetection**对象的属性。
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f87245d2f07600afd612273fdf3a28a36db44b78
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863535"
---
# <a name="get-riskdetection"></a><span data-ttu-id="ac68a-103">获取 riskDetection</span><span class="sxs-lookup"><span data-stu-id="ac68a-103">Get riskDetection</span></span>

<span data-ttu-id="ac68a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac68a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac68a-105">检索**riskDetection**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ac68a-105">Retrieve the properties of a **riskDetection** object.</span></span>

>[!NOTE]
><span data-ttu-id="ac68a-106">您必须具有 Azure AD 高级 P1 或 P2 许可证，才能使用风险检测 API。</span><span class="sxs-lookup"><span data-stu-id="ac68a-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac68a-107">权限</span><span class="sxs-lookup"><span data-stu-id="ac68a-107">Permissions</span></span>
<span data-ttu-id="ac68a-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ac68a-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ac68a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac68a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac68a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac68a-110">Permission type</span></span>      | <span data-ttu-id="ac68a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac68a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac68a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac68a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ac68a-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac68a-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="ac68a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac68a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac68a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac68a-115">Not supported.</span></span>    |
|<span data-ttu-id="ac68a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac68a-116">Application</span></span> | <span data-ttu-id="ac68a-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac68a-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac68a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac68a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections/{id}
GET /identityProtection/riskDetections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ac68a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac68a-119">Request headers</span></span>
| <span data-ttu-id="ac68a-120">名称</span><span class="sxs-lookup"><span data-stu-id="ac68a-120">Name</span></span>      |<span data-ttu-id="ac68a-121">说明</span><span class="sxs-lookup"><span data-stu-id="ac68a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ac68a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac68a-122">Authorization</span></span>  | <span data-ttu-id="ac68a-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="ac68a-123">Bearer {token}.</span></span> <span data-ttu-id="ac68a-124">Required.</span><span class="sxs-lookup"><span data-stu-id="ac68a-124">Required.</span></span> |
| <span data-ttu-id="ac68a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac68a-125">Content-Type</span></span> | <span data-ttu-id="ac68a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac68a-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac68a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac68a-127">Request body</span></span>
<span data-ttu-id="ac68a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac68a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac68a-129">响应</span><span class="sxs-lookup"><span data-stu-id="ac68a-129">Response</span></span>

<span data-ttu-id="ac68a-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[riskDetection](../resources/riskdetection.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ac68a-130">If successful, this method returns a `200 OK` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac68a-131">示例</span><span class="sxs-lookup"><span data-stu-id="ac68a-131">Examples</span></span>
### <a name="example-1-get-risk-detections"></a><span data-ttu-id="ac68a-132">示例1：获取风险检测</span><span class="sxs-lookup"><span data-stu-id="ac68a-132">Example 1: Get risk detections</span></span>
#### <a name="request"></a><span data-ttu-id="ac68a-133">请求</span><span class="sxs-lookup"><span data-stu-id="ac68a-133">Request</span></span>
<span data-ttu-id="ac68a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac68a-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac68a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac68a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="ac68a-136">C#</span><span class="sxs-lookup"><span data-stu-id="ac68a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac68a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac68a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac68a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac68a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ac68a-139">响应</span><span class="sxs-lookup"><span data-stu-id="ac68a-139">Response</span></span>
<span data-ttu-id="ac68a-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ac68a-140">Here is an example of the response.</span></span>
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
### <a name="example-2-get-risk-detections-for-specific-user"></a><span data-ttu-id="ac68a-141">示例2：获取特定用户的风险检测项</span><span class="sxs-lookup"><span data-stu-id="ac68a-141">Example 2: Get risk detections for specific user</span></span>
#### <a name="request"></a><span data-ttu-id="ac68a-142">请求</span><span class="sxs-lookup"><span data-stu-id="ac68a-142">Request</span></span>
<span data-ttu-id="ac68a-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac68a-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac68a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac68a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="ac68a-145">C#</span><span class="sxs-lookup"><span data-stu-id="ac68a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac68a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac68a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac68a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac68a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ac68a-148">响应</span><span class="sxs-lookup"><span data-stu-id="ac68a-148">Response</span></span>
<span data-ttu-id="ac68a-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ac68a-149">Here is an example of the response.</span></span>
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

