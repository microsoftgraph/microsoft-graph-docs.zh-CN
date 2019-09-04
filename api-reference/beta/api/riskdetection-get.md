---
title: 获取 riskDetection
description: 检索**riskdetection**对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 22bf8450edf700f18aaf9c1831ea9a4265c84da7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724783"
---
# <a name="get-riskdetection"></a><span data-ttu-id="300e4-103">获取 riskDetection</span><span class="sxs-lookup"><span data-stu-id="300e4-103">Get riskDetection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="300e4-104">检索**riskDetection**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="300e4-104">Retrieve the properties of a **riskDetection** object.</span></span>

>[!NOTE]
><span data-ttu-id="300e4-105">您必须具有 Azure AD 高级 P2 许可证才能使用风险检测 API。</span><span class="sxs-lookup"><span data-stu-id="300e4-105">You must have an Azure AD Premium P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="300e4-106">权限</span><span class="sxs-lookup"><span data-stu-id="300e4-106">Permissions</span></span>
<span data-ttu-id="300e4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="300e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="300e4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="300e4-109">Permission type</span></span>      | <span data-ttu-id="300e4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="300e4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="300e4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="300e4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="300e4-112">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="300e4-112">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="300e4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="300e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="300e4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="300e4-114">Not supported.</span></span>    |
|<span data-ttu-id="300e4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="300e4-115">Application</span></span> | <span data-ttu-id="300e4-116">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="300e4-116">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="300e4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="300e4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="300e4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="300e4-118">Request headers</span></span>
| <span data-ttu-id="300e4-119">名称</span><span class="sxs-lookup"><span data-stu-id="300e4-119">Name</span></span>      |<span data-ttu-id="300e4-120">说明</span><span class="sxs-lookup"><span data-stu-id="300e4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="300e4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="300e4-121">Authorization</span></span>  | <span data-ttu-id="300e4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="300e4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="300e4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="300e4-124">Content-Type</span></span> | <span data-ttu-id="300e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="300e4-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="300e4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="300e4-126">Request body</span></span>
<span data-ttu-id="300e4-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="300e4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="300e4-128">响应</span><span class="sxs-lookup"><span data-stu-id="300e4-128">Response</span></span>

<span data-ttu-id="300e4-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[riskDetection](../resources/riskdetection.md)对象。</span><span class="sxs-lookup"><span data-stu-id="300e4-129">If successful, this method returns a `200 OK` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="300e4-130">示例</span><span class="sxs-lookup"><span data-stu-id="300e4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="300e4-131">请求</span><span class="sxs-lookup"><span data-stu-id="300e4-131">Request</span></span>
<span data-ttu-id="300e4-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="300e4-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="300e4-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="300e4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="300e4-134">C#</span><span class="sxs-lookup"><span data-stu-id="300e4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="300e4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="300e4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="300e4-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="300e4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="300e4-137">响应</span><span class="sxs-lookup"><span data-stu-id="300e4-137">Response</span></span>
<span data-ttu-id="300e4-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="300e4-138">Here is an example of the response.</span></span>
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

