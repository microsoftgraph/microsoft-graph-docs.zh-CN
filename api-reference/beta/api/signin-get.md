---
title: 获取 signIn
description: 检索租户的特定 Azure AD 用户登录事件。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 13f95b67a76496f7695efb5d7ae11381c9647108
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271636"
---
# <a name="get-signin"></a><span data-ttu-id="1e56d-103">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="1e56d-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e56d-104">检索租户的特定 Azure AD 用户登录事件。</span><span class="sxs-lookup"><span data-stu-id="1e56d-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="1e56d-105">登录日志中目前包含交互式性质的登录名（其中用户名/密码作为授权令牌的一部分传递）和已成功联合的登录名。</span><span class="sxs-lookup"><span data-stu-id="1e56d-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="1e56d-106">权限</span><span class="sxs-lookup"><span data-stu-id="1e56d-106">Permissions</span></span>

<span data-ttu-id="1e56d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e56d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e56d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e56d-109">Permission type</span></span>      | <span data-ttu-id="1e56d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e56d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e56d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e56d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1e56d-112">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e56d-112">AuditLog.Read.All</span></span> |
|<span data-ttu-id="1e56d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e56d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e56d-114">不支持</span><span class="sxs-lookup"><span data-stu-id="1e56d-114">Not supported</span></span>   |
|<span data-ttu-id="1e56d-115">应用</span><span class="sxs-lookup"><span data-stu-id="1e56d-115">Application</span></span> | <span data-ttu-id="1e56d-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e56d-116">AuditLog.Read.All</span></span> | 

<span data-ttu-id="1e56d-117">此外，应用还必须向 Azure AD [正确注册](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="1e56d-117">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="1e56d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e56d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e56d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1e56d-119">Optional query parameters</span></span>

<span data-ttu-id="1e56d-120">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1e56d-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="1e56d-121">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="1e56d-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e56d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e56d-122">Request headers</span></span>

| <span data-ttu-id="1e56d-123">名称</span><span class="sxs-lookup"><span data-stu-id="1e56d-123">Name</span></span>      |<span data-ttu-id="1e56d-124">说明</span><span class="sxs-lookup"><span data-stu-id="1e56d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1e56d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e56d-125">Authorization</span></span>  | <span data-ttu-id="1e56d-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1e56d-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e56d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e56d-127">Request body</span></span>

<span data-ttu-id="1e56d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e56d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e56d-129">响应</span><span class="sxs-lookup"><span data-stu-id="1e56d-129">Response</span></span>

<span data-ttu-id="1e56d-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e56d-130">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e56d-131">示例</span><span class="sxs-lookup"><span data-stu-id="1e56d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e56d-132">请求</span><span class="sxs-lookup"><span data-stu-id="1e56d-132">Request</span></span>

<span data-ttu-id="1e56d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e56d-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```

### <a name="response"></a><span data-ttu-id="1e56d-134">响应</span><span class="sxs-lookup"><span data-stu-id="1e56d-134">Response</span></span>

<span data-ttu-id="1e56d-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1e56d-135">Here is an example of the response.</span></span> 

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1e56d-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1e56d-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1e56d-137">C#</span><span class="sxs-lookup"><span data-stu-id="1e56d-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signin-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e56d-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="1e56d-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signin-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1e56d-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="1e56d-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_signin-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
