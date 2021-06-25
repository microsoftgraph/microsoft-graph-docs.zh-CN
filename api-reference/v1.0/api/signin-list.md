---
title: 列出 signIn
description: 介绍 Microsoft (API) signIn 资源Graph方法。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 5bbd66efa246a0c3bbfdabe4a083a74443486ad2
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129451"
---
# <a name="list-signins"></a><span data-ttu-id="16a6d-103">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="16a6d-103">List signIns</span></span>

<span data-ttu-id="16a6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16a6d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16a6d-105">检索租户的 Azure AD 用户登录信息。</span><span class="sxs-lookup"><span data-stu-id="16a6d-105">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="16a6d-106">本质上是交互式的登录 (其中用户名/密码作为身份验证令牌) 且成功的联合登录当前包含在登录日志中。</span><span class="sxs-lookup"><span data-stu-id="16a6d-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="16a6d-107">最大和默认页面大小为 1，000 个对象，默认情况下，首先返回最新的登录。</span><span class="sxs-lookup"><span data-stu-id="16a6d-107">The maximum and default page size is 1,000 objects and by default, the most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="16a6d-108">权限</span><span class="sxs-lookup"><span data-stu-id="16a6d-108">Permissions</span></span>

<span data-ttu-id="16a6d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="16a6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="16a6d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="16a6d-111">Permission type</span></span>      | <span data-ttu-id="16a6d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16a6d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16a6d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16a6d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="16a6d-114">AuditLog.Read.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="16a6d-114">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="16a6d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16a6d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16a6d-116">不支持</span><span class="sxs-lookup"><span data-stu-id="16a6d-116">Not supported</span></span>   |
|<span data-ttu-id="16a6d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="16a6d-117">Application</span></span> | <span data-ttu-id="16a6d-118">AuditLog.Read.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="16a6d-118">AuditLog.Read.All and Directory.Read.All</span></span>  |

<span data-ttu-id="16a6d-119">应用必须 [正确注册到](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) Azure AD。</span><span class="sxs-lookup"><span data-stu-id="16a6d-119">Apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

<span data-ttu-id="16a6d-120">除了委派的权限，登录用户还需要属于以下目录角色之一，以便他们阅读登录报告。</span><span class="sxs-lookup"><span data-stu-id="16a6d-120">In addition to the delegated permissions, the signed-in user needs to belong to one of the following directory roles that allow them to read sign-in reports.</span></span> <span data-ttu-id="16a6d-121">若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：</span><span class="sxs-lookup"><span data-stu-id="16a6d-121">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="16a6d-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="16a6d-122">Global Administrator</span></span>
+ <span data-ttu-id="16a6d-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="16a6d-123">Global Reader</span></span>
+ <span data-ttu-id="16a6d-124">报告读取者</span><span class="sxs-lookup"><span data-stu-id="16a6d-124">Reports Reader</span></span>
+ <span data-ttu-id="16a6d-125">安全管理员</span><span class="sxs-lookup"><span data-stu-id="16a6d-125">Security Administrator</span></span>
+ <span data-ttu-id="16a6d-126">安全操作员</span><span class="sxs-lookup"><span data-stu-id="16a6d-126">Security Operator</span></span>
+ <span data-ttu-id="16a6d-127">安全读取者</span><span class="sxs-lookup"><span data-stu-id="16a6d-127">Security Reader</span></span>

## <a name="http-request"></a><span data-ttu-id="16a6d-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16a6d-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16a6d-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="16a6d-129">Optional query parameters</span></span>

<span data-ttu-id="16a6d-130">此方法支持 `$top` 、 `$skiptoken` 和 `$filter` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="16a6d-130">This method supports the `$top`, `$skiptoken`, and `$filter` OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="16a6d-131">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="16a6d-131">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="response"></a><span data-ttu-id="16a6d-132">响应</span><span class="sxs-lookup"><span data-stu-id="16a6d-132">Response</span></span>

<span data-ttu-id="16a6d-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="16a6d-133">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span> <span data-ttu-id="16a6d-134">对象的集合根据 **createdDateTime** 按降序列出。</span><span class="sxs-lookup"><span data-stu-id="16a6d-134">The collection of objects is listed in descending order based on **createdDateTime**.</span></span>

## <a name="examples"></a><span data-ttu-id="16a6d-135">示例</span><span class="sxs-lookup"><span data-stu-id="16a6d-135">Examples</span></span>

### <a name="example-1-list-all-sign-ins"></a><span data-ttu-id="16a6d-136">示例 1：列出所有登录</span><span class="sxs-lookup"><span data-stu-id="16a6d-136">Example 1: List all sign-ins</span></span>

#### <a name="request"></a><span data-ttu-id="16a6d-137">请求</span><span class="sxs-lookup"><span data-stu-id="16a6d-137">Request</span></span>

<span data-ttu-id="16a6d-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16a6d-138">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="16a6d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="16a6d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="16a6d-140">C#</span><span class="sxs-lookup"><span data-stu-id="16a6d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16a6d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16a6d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16a6d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16a6d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16a6d-143">Java</span><span class="sxs-lookup"><span data-stu-id="16a6d-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="16a6d-144">响应</span><span class="sxs-lookup"><span data-stu-id="16a6d-144">Response</span></span>

<span data-ttu-id="16a6d-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16a6d-145">Here is an example of the response.</span></span>
><span data-ttu-id="16a6d-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16a6d-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/auditLogs/signIns?$top=1&$skiptoken=9177f2e3532fcd4c4d225f68f7b9bdf7_1",
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

### <a name="example-2-retrieve-the-first-10-sign-ins-to-apps-with-the-appdisplayname-that-starts-with-graph"></a><span data-ttu-id="16a6d-147">示例 2：检索 appDisplayName 以"Graph"开头的应用的前 10 Graph</span><span class="sxs-lookup"><span data-stu-id="16a6d-147">Example 2: Retrieve the first 10 sign-ins to apps with the appDisplayName that starts with 'Graph'</span></span>

#### <a name="request"></a><span data-ttu-id="16a6d-148">请求</span><span class="sxs-lookup"><span data-stu-id="16a6d-148">Request</span></span>

<span data-ttu-id="16a6d-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16a6d-149">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns?&$filter=startsWith(appDisplayName,'Graph')&top=10
```

#### <a name="response"></a><span data-ttu-id="16a6d-150">响应</span><span class="sxs-lookup"><span data-stu-id="16a6d-150">Response</span></span>

<span data-ttu-id="16a6d-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16a6d-151">Here is an example of the response.</span></span> <span data-ttu-id="16a6d-152">该响应包含 `@odata.nextLink` 一个属性，其中包含可用于检索接下来的 10 个结果的 URL。</span><span class="sxs-lookup"><span data-stu-id="16a6d-152">The response includes a `@odata.nextLink` property which contains a URL that can be used to retrieve the next 10 results.</span></span>
><span data-ttu-id="16a6d-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16a6d-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/auditLogs/signins?$filter=startsWith(appDisplayName%2c%27Graph%27)&$top=10&$skiptoken=70f66c0893886b49370ffdb44cd8d137b1a12b9ba02f34a16f33c5e0f7c42fc7",
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
  "description": "List signIns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

