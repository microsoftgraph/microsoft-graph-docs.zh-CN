---
title: 获取 signIn
description: 介绍从 Microsoft (API) signIn Graph get 方法。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 6c5e3f215409e065ce6548e59827beb8ae1eafdf
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129460"
---
# <a name="get-signin"></a><span data-ttu-id="9e190-103">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="9e190-103">Get signIn</span></span>

<span data-ttu-id="9e190-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e190-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e190-105">检索租户的特定 Azure AD 用户登录事件。</span><span class="sxs-lookup"><span data-stu-id="9e190-105">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="9e190-106">本质上是交互式的登录 (其中用户名/密码作为身份验证令牌) 且成功的联合登录当前包含在登录日志中。</span><span class="sxs-lookup"><span data-stu-id="9e190-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e190-107">权限</span><span class="sxs-lookup"><span data-stu-id="9e190-107">Permissions</span></span>

<span data-ttu-id="9e190-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="9e190-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="9e190-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e190-110">Permission type</span></span>      | <span data-ttu-id="9e190-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e190-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e190-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e190-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9e190-113">AuditLog.Read.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e190-113">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="9e190-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e190-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e190-115">不支持</span><span class="sxs-lookup"><span data-stu-id="9e190-115">Not supported</span></span>   |
|<span data-ttu-id="9e190-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e190-116">Application</span></span> | <span data-ttu-id="9e190-117">AuditLog.Read.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e190-117">AuditLog.Read.All and Directory.Read.All</span></span> |

<span data-ttu-id="9e190-118">应用必须 [正确注册到](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) Azure AD。</span><span class="sxs-lookup"><span data-stu-id="9e190-118">Apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

<span data-ttu-id="9e190-119">除了委派的权限，登录用户还需要属于以下目录角色之一，以便他们阅读登录报告。</span><span class="sxs-lookup"><span data-stu-id="9e190-119">In addition to the delegated permissions, the signed-in user needs to belong to one of the following directory roles that allow them to read sign-in reports.</span></span> <span data-ttu-id="9e190-120">若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：</span><span class="sxs-lookup"><span data-stu-id="9e190-120">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="9e190-121">全局管理员</span><span class="sxs-lookup"><span data-stu-id="9e190-121">Global Administrator</span></span>
+ <span data-ttu-id="9e190-122">全局读取者</span><span class="sxs-lookup"><span data-stu-id="9e190-122">Global Reader</span></span>
+ <span data-ttu-id="9e190-123">报告读取者</span><span class="sxs-lookup"><span data-stu-id="9e190-123">Reports Reader</span></span>
+ <span data-ttu-id="9e190-124">安全管理员</span><span class="sxs-lookup"><span data-stu-id="9e190-124">Security Administrator</span></span>
+ <span data-ttu-id="9e190-125">安全操作员</span><span class="sxs-lookup"><span data-stu-id="9e190-125">Security Operator</span></span>
+ <span data-ttu-id="9e190-126">安全读取者</span><span class="sxs-lookup"><span data-stu-id="9e190-126">Security Reader</span></span>

## <a name="http-request"></a><span data-ttu-id="9e190-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e190-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e190-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9e190-128">Optional query parameters</span></span>

<span data-ttu-id="9e190-129">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9e190-129">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="9e190-130">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="9e190-130">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e190-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e190-131">Request headers</span></span>

| <span data-ttu-id="9e190-132">名称</span><span class="sxs-lookup"><span data-stu-id="9e190-132">Name</span></span>      |<span data-ttu-id="9e190-133">说明</span><span class="sxs-lookup"><span data-stu-id="9e190-133">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e190-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e190-134">Authorization</span></span>  | <span data-ttu-id="9e190-135">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9e190-135">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e190-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e190-136">Request body</span></span>

<span data-ttu-id="9e190-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9e190-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e190-138">响应</span><span class="sxs-lookup"><span data-stu-id="9e190-138">Response</span></span>

<span data-ttu-id="9e190-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e190-139">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e190-140">示例</span><span class="sxs-lookup"><span data-stu-id="9e190-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e190-141">请求</span><span class="sxs-lookup"><span data-stu-id="9e190-141">Request</span></span>

<span data-ttu-id="9e190-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e190-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9e190-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e190-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns/66ea54eb-6301-4ee5-be62-ff5a759b0100
```
# <a name="c"></a>[<span data-ttu-id="9e190-144">C#</span><span class="sxs-lookup"><span data-stu-id="9e190-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e190-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e190-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e190-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e190-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e190-147">Java</span><span class="sxs-lookup"><span data-stu-id="9e190-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9e190-148">响应</span><span class="sxs-lookup"><span data-stu-id="9e190-148">Response</span></span>

<span data-ttu-id="9e190-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9e190-149">Here is an example of the response.</span></span>
><span data-ttu-id="9e190-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9e190-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "value": [
        {
            "id": "66ea54eb-6301-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test Contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-ae82-4189-b4e2-a37c6808512d",
            "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "correlationId": "d79f5bee-5860-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "isInteractive": true,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
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
                    "result": "notEnabled"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled"
                },
              ]
        }
    ]
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

