---
title: 获取 signIn
doc_type: apiPageType
description: 检索租户的特定 Azure AD 用户登录事件。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ae597257544645ddf705be0156a10febcf272e29
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722361"
---
# <a name="get-signin"></a><span data-ttu-id="39602-103">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="39602-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39602-104">检索租户的特定 Azure AD 用户登录事件。</span><span class="sxs-lookup"><span data-stu-id="39602-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="39602-105">登录日志中目前包含交互式性质的登录名（其中用户名/密码作为授权令牌的一部分传递）和已成功联合的登录名。</span><span class="sxs-lookup"><span data-stu-id="39602-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="39602-106">权限</span><span class="sxs-lookup"><span data-stu-id="39602-106">Permissions</span></span>

<span data-ttu-id="39602-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39602-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39602-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="39602-109">Permission type</span></span>      | <span data-ttu-id="39602-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39602-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39602-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39602-111">Delegated (work or school account)</span></span> | <span data-ttu-id="39602-112">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="39602-112">AuditLog.Read.All</span></span> |
|<span data-ttu-id="39602-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39602-113">Delegated (work or school account)</span></span> | <span data-ttu-id="39602-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="39602-114">Directory.Read.All</span></span> |
|<span data-ttu-id="39602-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39602-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39602-116">不支持</span><span class="sxs-lookup"><span data-stu-id="39602-116">Not supported</span></span>   |
|<span data-ttu-id="39602-117">应用</span><span class="sxs-lookup"><span data-stu-id="39602-117">Application</span></span> | <span data-ttu-id="39602-118">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="39602-118">AuditLog.Read.All</span></span> | 
|<span data-ttu-id="39602-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="39602-119">Application</span></span> | <span data-ttu-id="39602-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="39602-120">Directory.Read.All</span></span> | 


<span data-ttu-id="39602-121">此外，应用还必须向 Azure AD [正确注册](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="39602-121">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="39602-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39602-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39602-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="39602-123">Optional query parameters</span></span>

<span data-ttu-id="39602-124">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="39602-124">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="39602-125">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="39602-125">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="39602-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="39602-126">Request headers</span></span>

| <span data-ttu-id="39602-127">名称</span><span class="sxs-lookup"><span data-stu-id="39602-127">Name</span></span>      |<span data-ttu-id="39602-128">说明</span><span class="sxs-lookup"><span data-stu-id="39602-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39602-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="39602-129">Authorization</span></span>  | <span data-ttu-id="39602-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="39602-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="39602-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="39602-131">Request body</span></span>

<span data-ttu-id="39602-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="39602-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39602-133">响应</span><span class="sxs-lookup"><span data-stu-id="39602-133">Response</span></span>

<span data-ttu-id="39602-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39602-134">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39602-135">示例</span><span class="sxs-lookup"><span data-stu-id="39602-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="39602-136">请求</span><span class="sxs-lookup"><span data-stu-id="39602-136">Request</span></span>

<span data-ttu-id="39602-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39602-137">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="39602-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="39602-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="39602-139">C#</span><span class="sxs-lookup"><span data-stu-id="39602-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="39602-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39602-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="39602-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="39602-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="39602-142">响应</span><span class="sxs-lookup"><span data-stu-id="39602-142">Response</span></span>

<span data-ttu-id="39602-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="39602-143">Here is an example of the response.</span></span> 

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
            "additionalDetails": "SignIn Success & CA Success"
        },
        "clientAppUsed": null,
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v3.14.1592.7",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
