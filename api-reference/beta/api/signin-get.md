---
title: 获取 signIn
description: 检索租户的特定 Azure AD 用户登录事件。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b1a6aad8847bfaf2b30439c86c841a85005a3d2
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657369"
---
# <a name="get-signin"></a><span data-ttu-id="808b6-103">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="808b6-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="808b6-104">检索租户的特定 Azure AD 用户登录事件。</span><span class="sxs-lookup"><span data-stu-id="808b6-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="808b6-105">登录日志中目前包含交互式性质的登录名（其中用户名/密码作为授权令牌的一部分传递）和已成功联合的登录名。</span><span class="sxs-lookup"><span data-stu-id="808b6-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="808b6-106">权限</span><span class="sxs-lookup"><span data-stu-id="808b6-106">Permissions</span></span>

<span data-ttu-id="808b6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="808b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="808b6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="808b6-109">Permission type</span></span>      | <span data-ttu-id="808b6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="808b6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="808b6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="808b6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="808b6-112">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="808b6-112">AuditLog.Read.All</span></span> |
|<span data-ttu-id="808b6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="808b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="808b6-114">不支持</span><span class="sxs-lookup"><span data-stu-id="808b6-114">Not supported</span></span>   |
|<span data-ttu-id="808b6-115">应用</span><span class="sxs-lookup"><span data-stu-id="808b6-115">Application</span></span> | <span data-ttu-id="808b6-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="808b6-116">AuditLog.Read.All</span></span> | 

<span data-ttu-id="808b6-117">此外，应用还必须向 Azure AD [正确注册](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="808b6-117">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="808b6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="808b6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="808b6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="808b6-119">Optional query parameters</span></span>

<span data-ttu-id="808b6-120">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="808b6-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="808b6-121">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="808b6-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="808b6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="808b6-122">Request headers</span></span>

| <span data-ttu-id="808b6-123">名称</span><span class="sxs-lookup"><span data-stu-id="808b6-123">Name</span></span>      |<span data-ttu-id="808b6-124">说明</span><span class="sxs-lookup"><span data-stu-id="808b6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="808b6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="808b6-125">Authorization</span></span>  | <span data-ttu-id="808b6-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="808b6-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="808b6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="808b6-127">Request body</span></span>

<span data-ttu-id="808b6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="808b6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="808b6-129">响应</span><span class="sxs-lookup"><span data-stu-id="808b6-129">Response</span></span>

<span data-ttu-id="808b6-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="808b6-130">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="808b6-131">示例</span><span class="sxs-lookup"><span data-stu-id="808b6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="808b6-132">请求</span><span class="sxs-lookup"><span data-stu-id="808b6-132">Request</span></span>

<span data-ttu-id="808b6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="808b6-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```

### <a name="response"></a><span data-ttu-id="808b6-134">响应</span><span class="sxs-lookup"><span data-stu-id="808b6-134">Response</span></span>

<span data-ttu-id="808b6-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="808b6-135">Here is an example of the response.</span></span> 

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="808b6-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="808b6-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="808b6-137">C#</span><span class="sxs-lookup"><span data-stu-id="808b6-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signin-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="808b6-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="808b6-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signin-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
