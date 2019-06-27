---
title: 获取 signIn
description: 介绍 Microsoft Graph API 中登录资源 (实体) 的 get 方法。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67ca5b333228b6b78cdb5854f7ee897b0afbdbe7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279266"
---
# <a name="get-signin"></a><span data-ttu-id="605da-103">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="605da-103">Get signIn</span></span>

<span data-ttu-id="605da-104">检索租户的特定 Azure AD 用户登录事件。</span><span class="sxs-lookup"><span data-stu-id="605da-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="605da-105">在性质 (用户名/密码作为身份验证令牌的一部分传递) 和成功的联合登录中当前包括在登录日志中的登录登录。</span><span class="sxs-lookup"><span data-stu-id="605da-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="605da-106">权限</span><span class="sxs-lookup"><span data-stu-id="605da-106">Permissions</span></span>

<span data-ttu-id="605da-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="605da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="605da-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="605da-109">Permission type</span></span>      | <span data-ttu-id="605da-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="605da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="605da-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="605da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="605da-112">AuditLog 和所有目录。全部读取. 所有</span><span class="sxs-lookup"><span data-stu-id="605da-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="605da-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="605da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="605da-114">不支持</span><span class="sxs-lookup"><span data-stu-id="605da-114">Not supported</span></span>   |
|<span data-ttu-id="605da-115">应用</span><span class="sxs-lookup"><span data-stu-id="605da-115">Application</span></span> | <span data-ttu-id="605da-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="605da-116">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="605da-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="605da-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="605da-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="605da-118">Optional query parameters</span></span>

<span data-ttu-id="605da-119">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="605da-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="605da-120">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="605da-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="605da-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="605da-121">Request headers</span></span>

| <span data-ttu-id="605da-122">名称</span><span class="sxs-lookup"><span data-stu-id="605da-122">Name</span></span>      |<span data-ttu-id="605da-123">说明</span><span class="sxs-lookup"><span data-stu-id="605da-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="605da-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="605da-124">Authorization</span></span>  | <span data-ttu-id="605da-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="605da-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="605da-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="605da-126">Request body</span></span>

<span data-ttu-id="605da-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="605da-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="605da-128">响应</span><span class="sxs-lookup"><span data-stu-id="605da-128">Response</span></span>

<span data-ttu-id="605da-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="605da-129">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="605da-130">示例</span><span class="sxs-lookup"><span data-stu-id="605da-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="605da-131">请求</span><span class="sxs-lookup"><span data-stu-id="605da-131">Request</span></span>

<span data-ttu-id="605da-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="605da-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->

```http
GET https://graph.microsoft.com/v1.0/auditLogs/signIns/{id}
```

### <a name="response"></a><span data-ttu-id="605da-133">响应</span><span class="sxs-lookup"><span data-stu-id="605da-133">Response</span></span>

<span data-ttu-id="605da-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="605da-134">Here is an example of the response.</span></span>
><span data-ttu-id="605da-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="605da-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="605da-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="605da-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="605da-138">C#</span><span class="sxs-lookup"><span data-stu-id="605da-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signin-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="605da-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="605da-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signin-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="605da-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="605da-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_signin-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "id": "id",
    "appId": "d3590ed6-52b3-4102-aeff-aad2292ab01c",
    "appDisplayName": "Azure",
    "createdDateTime": "2018-01-09T21:17:21.5077253Z",
    "clientAppUsed": null,
    "conditionalAccessApplied": true,
    "conditionalAccessPolicies": [{
        "id": "26490ed6-52b3-4102-aeff-aad2292abacf",
        "displayName": "capPolicy",
        "enforcedAccessControls": ["MFA", "TOU"],
        "enforcedSessionControls": ["CloudAppSecurity"],
        "result": "success"
    }],
    "correlationId": "17444d3c-563d-4b08-ac20-815892b87e42",
    "deviceDetail": {
        "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
        "displayName": "DeviceName",
        "operatingSystem": "Windows 10",
        "browser": "Rich Client v3.14.1592.7",
        "isCompliant": true,
        "isManaged": true,
        "trustType": ""
    },
    "ipAddress": "127.0.0.1",
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
    "status": {
        "errorCode": 0,
        "failureReason": null,
        "additionalDetails": "SignIn Success & CA Success"
    },
    "userDisplayName": "Jamie Doe",
    "userPrincipalName": "jdoe@wingtiptoys.com",
    "userId": "bbb3b4b5-e6e6-f7f5-f7f5-090805040302"
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
    "Error: /api-reference/v1.0/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
