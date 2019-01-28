---
title: 获取 signIn
description: 检索租户的 Azure AD 用户登录名。 登录日志中目前包含交互式性质的登录名（其中用户名/密码作为授权令牌的一部分传递）和已成功联合的登录名。
localization_priority: Priority
ms.openlocfilehash: 79bebfda40b15a5524aecfc99e5b6d83a168b28e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576610"
---
# <a name="get-signin"></a><span data-ttu-id="45cd8-104">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="45cd8-104">Get signIn</span></span>
<span data-ttu-id="45cd8-105">检索租户的 Azure AD 用户登录名。</span><span class="sxs-lookup"><span data-stu-id="45cd8-105">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="45cd8-106">登录日志中目前包含交互式性质的登录名（其中用户名/密码作为授权令牌的一部分传递）和已成功联合的登录名。</span><span class="sxs-lookup"><span data-stu-id="45cd8-106">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="45cd8-107">权限</span><span class="sxs-lookup"><span data-stu-id="45cd8-107">Permissions</span></span>
<span data-ttu-id="45cd8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45cd8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45cd8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="45cd8-110">Permission type</span></span>      | <span data-ttu-id="45cd8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45cd8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45cd8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45cd8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="45cd8-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="45cd8-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="45cd8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45cd8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45cd8-115">不支持</span><span class="sxs-lookup"><span data-stu-id="45cd8-115">Not supported</span></span>   |
|<span data-ttu-id="45cd8-116">应用</span><span class="sxs-lookup"><span data-stu-id="45cd8-116">Application</span></span> | <span data-ttu-id="45cd8-117">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="45cd8-117">AuditLog.Read.All</span></span> | 

<span data-ttu-id="45cd8-118">此外，应用还必须向 Azure AD [正确注册](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="45cd8-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="45cd8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45cd8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="45cd8-120">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="45cd8-120">Optional query parameters</span></span>
<span data-ttu-id="45cd8-121">此方法支持以下 OData 查询参数，它们有助于自定义响应。</span><span class="sxs-lookup"><span data-stu-id="45cd8-121">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="45cd8-122">请参看 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)，了解如何使用这些参数。</span><span class="sxs-lookup"><span data-stu-id="45cd8-122">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45cd8-123">请求头</span><span class="sxs-lookup"><span data-stu-id="45cd8-123">Request headers</span></span>
| <span data-ttu-id="45cd8-124">名称</span><span class="sxs-lookup"><span data-stu-id="45cd8-124">Name</span></span>      |<span data-ttu-id="45cd8-125">说明</span><span class="sxs-lookup"><span data-stu-id="45cd8-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="45cd8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="45cd8-126">Authorization</span></span>  | <span data-ttu-id="45cd8-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="45cd8-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="45cd8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="45cd8-128">Request body</span></span>
<span data-ttu-id="45cd8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45cd8-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="45cd8-130">响应</span><span class="sxs-lookup"><span data-stu-id="45cd8-130">Response</span></span>
<span data-ttu-id="45cd8-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45cd8-131">If successful, this method returns a `200 OK` response code and a [windowsPhone81CompliancePolicy](../resources/signin.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45cd8-132">示例</span><span class="sxs-lookup"><span data-stu-id="45cd8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45cd8-133">请求</span><span class="sxs-lookup"><span data-stu-id="45cd8-133">Request</span></span>
<span data-ttu-id="45cd8-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45cd8-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
##### <a name="response"></a><span data-ttu-id="45cd8-135">响应</span><span class="sxs-lookup"><span data-stu-id="45cd8-135">Response</span></span>
<span data-ttu-id="45cd8-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="45cd8-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211
```
```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id": "id",
        "createdDateTime": "2018-01-09T21:17:21.5077253Z",
        "userDisplayName": "Jamie Doe",
        "userPrincipalName": "jdoe@contoso.com",
        "userId": "bbb3b4b5-e6e6-f7f5-f7f5-090805040302",
        "appId": "d3590ed6-52b3-4102-aeff-aad2292ab01c",
        "appDisplayName": "Azure",
        "ipAddress": "127.0.0.1",
        "status": {
            "errorCode": 0,
            "failureReason": null,
            "additionalDetails": "SignIn Success & CA Sucess"
        },
        "clientAppUsed": null,
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v1.0.2016.0",
            "isCompliant": true,
            "isManaged": true,
            "trustType": ""
        },
        "location": {
            "city": "Redmond",
            "state": "WA",
            "countryOrRegion": "USA",
            "geoCoordinates": {
                "altitude": 41.589,
                "latitude": 41.589,
                "longitude": -93.6151
            }
        },
        "mfaDetail": {
            "mfaAuthMethod": "Phone Auth",
            "mfaAuthDetail": null
        },
        "correlationId": "17c47d3c-593d-4d08-ac20-813892b87e42",
        "conditionalAccessApplied": true,
        "conditionalAccessPolicies": [{
            "id": "26490ed6-52b3-4102-aeff-aad2292abacf",
            "displayName": "capPolicy",
            "enforcedAccessControls": ["MFA", "TOU"],
            "enforcedSessionControls": ["CloudAppSecurity"],
            "result": "success"
        }],
        "isRisky": false,
        "riskLevel": "low"
    }]
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
