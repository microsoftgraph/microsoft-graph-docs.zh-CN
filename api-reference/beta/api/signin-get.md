---
title: 获取 signIn
doc_type: apiPageType
description: 获取一个 signIn 对象，该对象包含租户的所有Azure Active Directory登录。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: d9cf2f0e6a03a490c1818712bf230120ff37311f
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129487"
---
# <a name="get-signin"></a><span data-ttu-id="d130a-103">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="d130a-103">Get signIn</span></span>

<span data-ttu-id="d130a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d130a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d130a-105">获取包含租户的特定用户登录事件的 [signIn](../resources/signin.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d130a-105">Get a [signIn](../resources/signin.md) object that contains a specific user sign-in event for your tenant.</span></span> <span data-ttu-id="d130a-106">这包括要求用户输入用户名或密码以及会话令牌的登录。</span><span class="sxs-lookup"><span data-stu-id="d130a-106">This includes sign-ins where a user is asked to enter a username or password, and session tokens.</span></span>

## <a name="permissions"></a><span data-ttu-id="d130a-107">权限</span><span class="sxs-lookup"><span data-stu-id="d130a-107">Permissions</span></span>

<span data-ttu-id="d130a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d130a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d130a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d130a-110">Permission type</span></span>      | <span data-ttu-id="d130a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d130a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="d130a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d130a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d130a-113">AuditLog.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d130a-113">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="d130a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d130a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d130a-115">不支持</span><span class="sxs-lookup"><span data-stu-id="d130a-115">Not supported</span></span> |
| <span data-ttu-id="d130a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d130a-116">Application</span></span> | <span data-ttu-id="d130a-117">AuditLog.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d130a-117">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="d130a-118">应用必须 [正确注册到](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) Azure AD。</span><span class="sxs-lookup"><span data-stu-id="d130a-118">Apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

<span data-ttu-id="d130a-119">除了委派的权限，登录用户还需要属于以下目录角色之一，以便他们阅读登录报告。</span><span class="sxs-lookup"><span data-stu-id="d130a-119">In addition to the delegated permissions, the signed-in user needs to belong to one of the following directory roles that allow them to read sign-in reports.</span></span> <span data-ttu-id="d130a-120">若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：</span><span class="sxs-lookup"><span data-stu-id="d130a-120">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="d130a-121">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d130a-121">Global Administrator</span></span>
+ <span data-ttu-id="d130a-122">全局读取者</span><span class="sxs-lookup"><span data-stu-id="d130a-122">Global Reader</span></span>
+ <span data-ttu-id="d130a-123">报告读取者</span><span class="sxs-lookup"><span data-stu-id="d130a-123">Reports Reader</span></span>
+ <span data-ttu-id="d130a-124">安全管理员</span><span class="sxs-lookup"><span data-stu-id="d130a-124">Security Administrator</span></span>
+ <span data-ttu-id="d130a-125">安全操作员</span><span class="sxs-lookup"><span data-stu-id="d130a-125">Security Operator</span></span>
+ <span data-ttu-id="d130a-126">安全读取者</span><span class="sxs-lookup"><span data-stu-id="d130a-126">Security Reader</span></span>

## <a name="http-request"></a><span data-ttu-id="d130a-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d130a-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d130a-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d130a-128">Optional query parameters</span></span>

<span data-ttu-id="d130a-129">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d130a-129">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="d130a-130">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="d130a-130">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d130a-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="d130a-131">Request headers</span></span>

| <span data-ttu-id="d130a-132">名称</span><span class="sxs-lookup"><span data-stu-id="d130a-132">Name</span></span>      |<span data-ttu-id="d130a-133">说明</span><span class="sxs-lookup"><span data-stu-id="d130a-133">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d130a-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="d130a-134">Authorization</span></span> | <span data-ttu-id="d130a-135">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d130a-135">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d130a-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="d130a-136">Request body</span></span>

<span data-ttu-id="d130a-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d130a-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d130a-138">响应</span><span class="sxs-lookup"><span data-stu-id="d130a-138">Response</span></span>

<span data-ttu-id="d130a-139">如果成功，此方法在响应正文中返回 响应代码 `200 OK` 和 [signIn](../resources/signin.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d130a-139">If successful, this method returns a `200 OK` response code and a [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d130a-140">示例</span><span class="sxs-lookup"><span data-stu-id="d130a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d130a-141">请求</span><span class="sxs-lookup"><span data-stu-id="d130a-141">Request</span></span>

<span data-ttu-id="d130a-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d130a-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d130a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d130a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/66ea54eb-blah-4ee5-be62-ff5a759b0100
```
# <a name="c"></a>[<span data-ttu-id="d130a-144">C#</span><span class="sxs-lookup"><span data-stu-id="d130a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d130a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d130a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d130a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d130a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d130a-147">Java</span><span class="sxs-lookup"><span data-stu-id="d130a-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d130a-148">响应</span><span class="sxs-lookup"><span data-stu-id="d130a-148">Response</span></span>

<span data-ttu-id="d130a-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d130a-149">The following is an example of the response.</span></span>
><span data-ttu-id="d130a-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d130a-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->


```http
HTTP/1.1 200 OK
Content-type: application/json

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
      "authenticationStepDateTime": "2018-11-06T18:48:03.8313489Z",
      "authenticationMethod": "FIDO2",
      "authenticationMethodDetail": "1G54395783",
      "succeeded": true,
      "authenticationStepResultDetail": "methodSucceeded",
      "authenticationStepRequirement": "Primary authentication"
    },
    {
      "authenticationStepDateTime": "2018-11-06T18:48:12.94725647Z",
      "authenticationMethod": "Claim in access token",
      "authenticationMethodDetail": null,
      "succeeded": true,
      "authenticationStepResultDetail": "methodSucceeded",
      "authenticationStepRequirement": "MFA"
    }
  ],
  "authenticationRequirementPolicies": []
}
```
