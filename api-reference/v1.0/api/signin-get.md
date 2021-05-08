---
title: 获取 signIn
description: 介绍从 Microsoft (API) signIn Graph get 方法。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 007047fe0fe9364f99af31ee0447967da7618060
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238398"
---
# <a name="get-signin"></a><span data-ttu-id="f2838-103">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="f2838-103">Get signIn</span></span>

<span data-ttu-id="f2838-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2838-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2838-105">检索租户的特定 Azure AD 用户登录事件。</span><span class="sxs-lookup"><span data-stu-id="f2838-105">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="f2838-106">本质上是交互式的登录 (其中用户名/密码作为身份验证令牌) 且成功的联合登录当前包含在登录日志中。</span><span class="sxs-lookup"><span data-stu-id="f2838-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2838-107">权限</span><span class="sxs-lookup"><span data-stu-id="f2838-107">Permissions</span></span>

<span data-ttu-id="f2838-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="f2838-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="f2838-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2838-110">Permission type</span></span>      | <span data-ttu-id="f2838-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2838-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2838-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2838-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2838-113">AuditLog.Read.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2838-113">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="f2838-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2838-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2838-115">不支持</span><span class="sxs-lookup"><span data-stu-id="f2838-115">Not supported</span></span>   |
|<span data-ttu-id="f2838-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2838-116">Application</span></span> | <span data-ttu-id="f2838-117">AuditLog.Read.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2838-117">AuditLog.Read.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2838-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2838-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2838-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f2838-119">Optional query parameters</span></span>

<span data-ttu-id="f2838-120">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f2838-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="f2838-121">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="f2838-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2838-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2838-122">Request headers</span></span>

| <span data-ttu-id="f2838-123">名称</span><span class="sxs-lookup"><span data-stu-id="f2838-123">Name</span></span>      |<span data-ttu-id="f2838-124">说明</span><span class="sxs-lookup"><span data-stu-id="f2838-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f2838-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2838-125">Authorization</span></span>  | <span data-ttu-id="f2838-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f2838-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2838-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2838-127">Request body</span></span>

<span data-ttu-id="f2838-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f2838-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2838-129">响应</span><span class="sxs-lookup"><span data-stu-id="f2838-129">Response</span></span>

<span data-ttu-id="f2838-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2838-130">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2838-131">示例</span><span class="sxs-lookup"><span data-stu-id="f2838-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2838-132">请求</span><span class="sxs-lookup"><span data-stu-id="f2838-132">Request</span></span>

<span data-ttu-id="f2838-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2838-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns/66ea54eb-6301-4ee5-be62-ff5a759b0100
```

### <a name="response"></a><span data-ttu-id="f2838-134">响应</span><span class="sxs-lookup"><span data-stu-id="f2838-134">Response</span></span>

<span data-ttu-id="f2838-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f2838-135">Here is an example of the response.</span></span>
><span data-ttu-id="f2838-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f2838-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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

