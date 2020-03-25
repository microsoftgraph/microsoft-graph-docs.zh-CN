---
title: 获取 signIn
doc_type: apiPageType
description: 获取一个登录对象，其中包含 Azure Active Directory 租户的所有登录。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4265807cc72794f3611fdda64d405138931b7df3
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947312"
---
# <a name="get-signin"></a><span data-ttu-id="16517-103">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="16517-103">Get signIn</span></span>

<span data-ttu-id="16517-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16517-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16517-105">获取一个[登录](../resources/signin.md)对象，其中包含租户的特定用户登录事件。</span><span class="sxs-lookup"><span data-stu-id="16517-105">Get a [signIn](../resources/signin.md) object that contains a specific user sign-in event for your tenant.</span></span> <span data-ttu-id="16517-106">这包括要求用户输入用户名或密码以及会话令牌的登录。</span><span class="sxs-lookup"><span data-stu-id="16517-106">This includes sign-ins where a user is asked to enter a username or password, and session tokens.</span></span>

## <a name="permissions"></a><span data-ttu-id="16517-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="16517-107">Permissions</span></span>

<span data-ttu-id="16517-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16517-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16517-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="16517-110">Permission type</span></span>      | <span data-ttu-id="16517-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16517-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="16517-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16517-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16517-113">AuditLog、目录、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="16517-113">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="16517-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16517-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16517-115">不支持</span><span class="sxs-lookup"><span data-stu-id="16517-115">Not supported</span></span> |
| <span data-ttu-id="16517-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="16517-116">Application</span></span> | <span data-ttu-id="16517-117">AuditLog、目录、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="16517-117">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="16517-118">此外，应用还必须向 Azure AD [正确注册](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="16517-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="16517-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16517-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16517-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="16517-120">Optional query parameters</span></span>

<span data-ttu-id="16517-121">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="16517-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="16517-122">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="16517-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="16517-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="16517-123">Request headers</span></span>

| <span data-ttu-id="16517-124">名称</span><span class="sxs-lookup"><span data-stu-id="16517-124">Name</span></span>      |<span data-ttu-id="16517-125">说明</span><span class="sxs-lookup"><span data-stu-id="16517-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16517-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="16517-126">Authorization</span></span> | <span data-ttu-id="16517-127">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="16517-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="16517-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="16517-128">Request body</span></span>

<span data-ttu-id="16517-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16517-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16517-130">响应</span><span class="sxs-lookup"><span data-stu-id="16517-130">Response</span></span>

<span data-ttu-id="16517-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[登录](../resources/signin.md)对象。</span><span class="sxs-lookup"><span data-stu-id="16517-131">If successful, this method returns a `200 OK` response code and a [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16517-132">示例</span><span class="sxs-lookup"><span data-stu-id="16517-132">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="16517-133">示例1：用户使用 MFA 登录，这是由条件访问策略触发的。</span><span class="sxs-lookup"><span data-stu-id="16517-133">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="16517-134">主要身份验证是通过 FIDO。</span><span class="sxs-lookup"><span data-stu-id="16517-134">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="16517-135">请求</span><span class="sxs-lookup"><span data-stu-id="16517-135">Request</span></span>

<span data-ttu-id="16517-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="16517-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="16517-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="16517-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="16517-138">C#</span><span class="sxs-lookup"><span data-stu-id="16517-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16517-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16517-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16517-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16517-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="16517-141">响应</span><span class="sxs-lookup"><span data-stu-id="16517-141">Response</span></span>

<span data-ttu-id="16517-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16517-142">The following is an example of the response.</span></span>

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
            "id": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-1111-5555-b4e2-a37c6808512d",
            "appId": "de8bc8b5-5555-6666-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "authenticationRequirement": "MultifactorAuthentication",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Safari/537.36 Edg/80.0.361.66",
            "correlationId": "d79f5bee-blah-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "originalRequestId": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "isInteractive": true,
            "tokenIssuerName": "",
            "tokenIssuerType": "AzureAD",
            "processingTimeInMilliseconds": 541,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "riskEventTypes_v2": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
            "authenticationMethodsUsed": [],
            "alternateSignInName": "testaccount2@contoso.com",
            "servicePrincipalName": null,
            "servicePrincipalId": "",
            "mfaDetail": null,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            },
            "deviceDetail": {
                "deviceId": "",
                "displayName": null,
                "operatingSystem": "Windows 10",
                "browser": "Edge 80.0.361",
                "isCompliant": null,
                "isManaged": null,
                "trustType": null
            },
            "location": {
                "city": "Redmond",
                "state": "Washington",
                "countryOrRegion": "US",
                "geoCoordinates": {
                    "altitude": null,
                    "latitude": 47.68050003051758,
                    "longitude": -122.12094116210938
                }
            },
            "appliedConditionalAccessPolicies": [
                {
                    "id": "de7e60eb-ed89-4d73-8205-2227def6b7c9",
                    "displayName": "SharePoint limited access for guest workers",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
               
            ],
            "authenticationProcessingDetails": [],
            "networkLocationDetails": [],
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
            "authenticationRequirementPolicies": []
        }
    ]
}
```

### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="16517-143">示例2：用户仅使用主身份验证进行登录。</span><span class="sxs-lookup"><span data-stu-id="16517-143">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="16517-144">主要身份验证通过云密码。</span><span class="sxs-lookup"><span data-stu-id="16517-144">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="16517-145">请求</span><span class="sxs-lookup"><span data-stu-id="16517-145">Request</span></span>

<span data-ttu-id="16517-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="16517-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="16517-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="16517-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="16517-148">C#</span><span class="sxs-lookup"><span data-stu-id="16517-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16517-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16517-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16517-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16517-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="16517-151">响应</span><span class="sxs-lookup"><span data-stu-id="16517-151">Response</span></span>

<span data-ttu-id="16517-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16517-152">The following is an example of the response.</span></span>

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
      "userPrincipalName":"jdoe@contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
       "authenticationRequirement": "singleFactorAuthentication",
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
