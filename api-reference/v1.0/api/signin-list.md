---
title: 列出 signIn
description: 介绍 Microsoft (API) signIn 资源Graph方法。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 8ee9f01bf2b7f590332abcd726e3d6d21b506125
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241126"
---
# <a name="list-signins"></a><span data-ttu-id="f276c-103">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="f276c-103">List signIns</span></span>

<span data-ttu-id="f276c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f276c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f276c-105">检索租户的 Azure AD 用户登录信息。</span><span class="sxs-lookup"><span data-stu-id="f276c-105">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="f276c-106">本质上是交互式的登录 (其中用户名/密码作为身份验证令牌) 且成功的联合登录当前包含在登录日志中。</span><span class="sxs-lookup"><span data-stu-id="f276c-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="f276c-107">最大和默认页面大小为 1，000 个对象，默认情况下，首先返回最新的登录。</span><span class="sxs-lookup"><span data-stu-id="f276c-107">The maximum and default page size is 1,000 objects and by default, the most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="f276c-108">权限</span><span class="sxs-lookup"><span data-stu-id="f276c-108">Permissions</span></span>

<span data-ttu-id="f276c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="f276c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="f276c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f276c-111">Permission type</span></span>      | <span data-ttu-id="f276c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f276c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f276c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f276c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f276c-114">AuditLog.Read.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f276c-114">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="f276c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f276c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f276c-116">不支持</span><span class="sxs-lookup"><span data-stu-id="f276c-116">Not supported</span></span>   |
|<span data-ttu-id="f276c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f276c-117">Application</span></span> | <span data-ttu-id="f276c-118">AuditLog.Read.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f276c-118">AuditLog.Read.All and Directory.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f276c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f276c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f276c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f276c-120">Optional query parameters</span></span>

<span data-ttu-id="f276c-121">此方法支持 `$top` 、 `$skiptoken` 和 `$filter` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f276c-121">This method supports the `$top`, `$skiptoken`, and `$filter` OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="f276c-122">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="f276c-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="response"></a><span data-ttu-id="f276c-123">响应</span><span class="sxs-lookup"><span data-stu-id="f276c-123">Response</span></span>

<span data-ttu-id="f276c-124">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f276c-124">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span> <span data-ttu-id="f276c-125">对象的集合根据 **createdDateTime** 按降序列出。</span><span class="sxs-lookup"><span data-stu-id="f276c-125">The collection of objects is listed in descending order based on **createdDateTime**.</span></span>

## <a name="examples"></a><span data-ttu-id="f276c-126">示例</span><span class="sxs-lookup"><span data-stu-id="f276c-126">Examples</span></span>

### <a name="example-1-list-all-sign-ins"></a><span data-ttu-id="f276c-127">示例 1：列出所有登录</span><span class="sxs-lookup"><span data-stu-id="f276c-127">Example 1: List all sign-ins</span></span>

#### <a name="request"></a><span data-ttu-id="f276c-128">请求</span><span class="sxs-lookup"><span data-stu-id="f276c-128">Request</span></span>

<span data-ttu-id="f276c-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f276c-129">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f276c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f276c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="f276c-131">C#</span><span class="sxs-lookup"><span data-stu-id="f276c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f276c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f276c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f276c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f276c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f276c-134">Java</span><span class="sxs-lookup"><span data-stu-id="f276c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f276c-135">响应</span><span class="sxs-lookup"><span data-stu-id="f276c-135">Response</span></span>

<span data-ttu-id="f276c-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f276c-136">Here is an example of the response.</span></span>
><span data-ttu-id="f276c-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f276c-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-retrieve-the-first-10-sign-ins-to-apps-with-the-appdisplayname-that-starts-with-graph"></a><span data-ttu-id="f276c-138">示例 2：检索 appDisplayName 以"Graph"开头的应用的前 10 Graph</span><span class="sxs-lookup"><span data-stu-id="f276c-138">Example 2: Retrieve the first 10 sign-ins to apps with the appDisplayName that starts with 'Graph'</span></span>

#### <a name="request"></a><span data-ttu-id="f276c-139">请求</span><span class="sxs-lookup"><span data-stu-id="f276c-139">Request</span></span>

<span data-ttu-id="f276c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f276c-140">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns?&$filter=startsWith(appDisplayName,'Graph')&top=10
```

#### <a name="response"></a><span data-ttu-id="f276c-141">响应</span><span class="sxs-lookup"><span data-stu-id="f276c-141">Response</span></span>

<span data-ttu-id="f276c-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f276c-142">Here is an example of the response.</span></span> <span data-ttu-id="f276c-143">该响应包含 `@odata.nextLink` 一个属性，其中包含可用于检索接下来的 10 个结果的 URL。</span><span class="sxs-lookup"><span data-stu-id="f276c-143">The response includes a `@odata.nextLink` property which contains a URL that can be used to retrieve the next 10 results.</span></span>
><span data-ttu-id="f276c-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f276c-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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

