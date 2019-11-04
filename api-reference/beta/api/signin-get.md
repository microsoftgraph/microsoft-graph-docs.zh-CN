---
title: 获取 signIn
doc_type: apiPageType
description: 获取一个登录对象，其中包含 Azure Active Directory 租户的所有登录。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ed96154c2104dc0b06ee24f01080203a8bb61b15
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938370"
---
# <a name="get-signin"></a><span data-ttu-id="63f0e-103">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="63f0e-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63f0e-104">获取一个[登录](../resources/signin.md)对象，其中包含租户的特定用户登录事件。</span><span class="sxs-lookup"><span data-stu-id="63f0e-104">Get a [signIn](../resources/signin.md) object that contains a specific user sign-in event for your tenant.</span></span> <span data-ttu-id="63f0e-105">这包括要求用户输入用户名或密码以及会话令牌的登录。</span><span class="sxs-lookup"><span data-stu-id="63f0e-105">This includes sign-ins where a user is asked to enter a username or password, and session tokens.</span></span>

## <a name="permissions"></a><span data-ttu-id="63f0e-106">权限</span><span class="sxs-lookup"><span data-stu-id="63f0e-106">Permissions</span></span>

<span data-ttu-id="63f0e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63f0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63f0e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="63f0e-109">Permission type</span></span>      | <span data-ttu-id="63f0e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63f0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="63f0e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63f0e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63f0e-112">AuditLog、目录、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="63f0e-112">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="63f0e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63f0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63f0e-114">不支持</span><span class="sxs-lookup"><span data-stu-id="63f0e-114">Not supported</span></span> |
| <span data-ttu-id="63f0e-115">应用</span><span class="sxs-lookup"><span data-stu-id="63f0e-115">Application</span></span> | <span data-ttu-id="63f0e-116">AuditLog、目录、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="63f0e-116">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="63f0e-117">此外，应用还必须向 Azure AD [正确注册](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="63f0e-117">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="63f0e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63f0e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63f0e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="63f0e-119">Optional query parameters</span></span>

<span data-ttu-id="63f0e-120">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="63f0e-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="63f0e-121">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="63f0e-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="63f0e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="63f0e-122">Request headers</span></span>

| <span data-ttu-id="63f0e-123">名称</span><span class="sxs-lookup"><span data-stu-id="63f0e-123">Name</span></span>      |<span data-ttu-id="63f0e-124">说明</span><span class="sxs-lookup"><span data-stu-id="63f0e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="63f0e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="63f0e-125">Authorization</span></span> | <span data-ttu-id="63f0e-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="63f0e-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="63f0e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="63f0e-127">Request body</span></span>

<span data-ttu-id="63f0e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63f0e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63f0e-129">响应</span><span class="sxs-lookup"><span data-stu-id="63f0e-129">Response</span></span>

<span data-ttu-id="63f0e-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[登录](../resources/signin.md)对象。</span><span class="sxs-lookup"><span data-stu-id="63f0e-130">If successful, this method returns a `200 OK` response code and a [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63f0e-131">示例</span><span class="sxs-lookup"><span data-stu-id="63f0e-131">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="63f0e-132">示例1：用户使用 MFA 登录，这是由条件访问策略触发的。</span><span class="sxs-lookup"><span data-stu-id="63f0e-132">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="63f0e-133">主要身份验证是通过 FIDO。</span><span class="sxs-lookup"><span data-stu-id="63f0e-133">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="63f0e-134">请求</span><span class="sxs-lookup"><span data-stu-id="63f0e-134">Request</span></span>

<span data-ttu-id="63f0e-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63f0e-135">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="63f0e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="63f0e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="63f0e-137">C#</span><span class="sxs-lookup"><span data-stu-id="63f0e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63f0e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63f0e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63f0e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63f0e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="63f0e-140">响应</span><span class="sxs-lookup"><span data-stu-id="63f0e-140">Response</span></span>

<span data-ttu-id="63f0e-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63f0e-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->


```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [ 
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"FIDO2",
          "authenticationMethodDetail":"1G54395783",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        },
        {
          "authenticationStepDateTime":"2018-11-06T18:48:12.94725647Z",
          "authenticationMethod":"Claim in access token",
          "authenticationMethodDetail":null,
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"MFA"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"applied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```

### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="63f0e-142">示例2：用户仅使用主身份验证进行登录。</span><span class="sxs-lookup"><span data-stu-id="63f0e-142">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="63f0e-143">主要身份验证通过云密码。</span><span class="sxs-lookup"><span data-stu-id="63f0e-143">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="63f0e-144">请求</span><span class="sxs-lookup"><span data-stu-id="63f0e-144">Request</span></span>

<span data-ttu-id="63f0e-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63f0e-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```

#### <a name="response"></a><span data-ttu-id="63f0e-146">响应</span><span class="sxs-lookup"><span data-stu-id="63f0e-146">Response</span></span>

<span data-ttu-id="63f0e-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63f0e-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"Password",
          "authenticationMethodDetail":"Cloud password",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"notApplied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```
