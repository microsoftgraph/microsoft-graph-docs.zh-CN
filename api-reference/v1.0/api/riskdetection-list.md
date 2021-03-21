---
title: 列出 riskDetections
description: 获取 riskDetection 对象及其属性的列表。
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9688d9d5b54958a33705a71bb8637923b5163ce5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959527"
---
# <a name="list-riskdetections"></a><span data-ttu-id="90441-103">列出 riskDetections</span><span class="sxs-lookup"><span data-stu-id="90441-103">List riskDetections</span></span>
<span data-ttu-id="90441-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90441-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90441-105">获取 [riskDetection 对象](../resources/riskdetection.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="90441-105">Get a list of the [riskDetection](../resources/riskdetection.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="90441-106">必须具有 Azure AD Premium P1 或 P2 许可证才能使用风险检测 API。</span><span class="sxs-lookup"><span data-stu-id="90441-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="90441-107">权限</span><span class="sxs-lookup"><span data-stu-id="90441-107">Permissions</span></span>
<span data-ttu-id="90441-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="90441-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="90441-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="90441-110">Permission type</span></span>      | <span data-ttu-id="90441-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90441-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90441-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90441-112">Delegated (work or school account)</span></span> | <span data-ttu-id="90441-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="90441-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="90441-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90441-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90441-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="90441-115">Not supported.</span></span>    |
|<span data-ttu-id="90441-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="90441-116">Application</span></span> | <span data-ttu-id="90441-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="90441-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90441-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90441-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90441-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="90441-119">Optional query parameters</span></span>
<span data-ttu-id="90441-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="90441-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="90441-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="90441-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="90441-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="90441-122">Request headers</span></span>
|<span data-ttu-id="90441-123">名称</span><span class="sxs-lookup"><span data-stu-id="90441-123">Name</span></span>|<span data-ttu-id="90441-124">说明</span><span class="sxs-lookup"><span data-stu-id="90441-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="90441-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="90441-125">Authorization</span></span>|<span data-ttu-id="90441-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90441-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90441-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="90441-128">Request body</span></span>
<span data-ttu-id="90441-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90441-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90441-130">响应</span><span class="sxs-lookup"><span data-stu-id="90441-130">Response</span></span>

<span data-ttu-id="90441-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [riskDetection](../resources/riskdetection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="90441-131">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90441-132">示例</span><span class="sxs-lookup"><span data-stu-id="90441-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90441-133">请求</span><span class="sxs-lookup"><span data-stu-id="90441-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskdetection_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections
```


### <a name="response"></a><span data-ttu-id="90441-134">响应</span><span class="sxs-lookup"><span data-stu-id="90441-134">Response</span></span>
<span data-ttu-id="90441-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="90441-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskDetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
  {
    "@odata.type": "#microsoft.graph.riskDetection",
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
    "userDisplayName": "Olivia Lack",
    "userPrincipalName": "olack@adatum.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
  ]
}
```


