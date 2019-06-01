---
title: 列出 signIn
description: 描述 Microsoft Graph API (REST) 中 signIn 资源（实体）的列表方法，有助于审核目录（租户）活动（beta 版本）。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8e17b6d6d4a8a80de26d59da5e17e7f5655a04ef
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657362"
---
# <a name="list-signins"></a><span data-ttu-id="27f01-103">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="27f01-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27f01-104">检索租户的 Azure AD 用户登录信息。</span><span class="sxs-lookup"><span data-stu-id="27f01-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="27f01-105">登录日志中目前包含交互式性质的登录名（其中用户名/密码作为授权令牌的一部分传递）和已成功联合的登录名。</span><span class="sxs-lookup"><span data-stu-id="27f01-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="27f01-106">首先返回最新 signIn。</span><span class="sxs-lookup"><span data-stu-id="27f01-106">The most recent signIns are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="27f01-107">权限</span><span class="sxs-lookup"><span data-stu-id="27f01-107">Permissions</span></span>

<span data-ttu-id="27f01-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27f01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27f01-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="27f01-110">Permission type</span></span>      | <span data-ttu-id="27f01-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27f01-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27f01-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27f01-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27f01-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="27f01-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="27f01-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27f01-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27f01-115">不支持</span><span class="sxs-lookup"><span data-stu-id="27f01-115">Not supported</span></span>   |
|<span data-ttu-id="27f01-116">应用</span><span class="sxs-lookup"><span data-stu-id="27f01-116">Application</span></span> | <span data-ttu-id="27f01-117">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="27f01-117">AuditLog.Read.All</span></span> | 

<span data-ttu-id="27f01-118">此外，应用还必须向 Azure AD [正确注册](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="27f01-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="27f01-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27f01-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="27f01-120">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="27f01-120">Optional query parameters</span></span>
<span data-ttu-id="27f01-121">此方法支持以下 OData 查询参数，它们有助于自定义响应。</span><span class="sxs-lookup"><span data-stu-id="27f01-121">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="27f01-122">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="27f01-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="27f01-123">名称</span><span class="sxs-lookup"><span data-stu-id="27f01-123">Name</span></span>     |<span data-ttu-id="27f01-124">说明</span><span class="sxs-lookup"><span data-stu-id="27f01-124">Description</span></span>                            |<span data-ttu-id="27f01-125">示例</span><span class="sxs-lookup"><span data-stu-id="27f01-125">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="27f01-126">$filter</span><span class="sxs-lookup"><span data-stu-id="27f01-126">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="27f01-127">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="27f01-127">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="27f01-128">$top</span><span class="sxs-lookup"><span data-stu-id="27f01-128">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="27f01-129">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="27f01-129">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="27f01-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="27f01-130">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="27f01-131">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="27f01-131">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="27f01-132">$filter 参数支持的属性列表</span><span class="sxs-lookup"><span data-stu-id="27f01-132">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="27f01-133">属性名</span><span class="sxs-lookup"><span data-stu-id="27f01-133">Attribute Name</span></span> |<span data-ttu-id="27f01-134">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="27f01-134">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="27f01-135">id</span><span class="sxs-lookup"><span data-stu-id="27f01-135">id</span></span>|<span data-ttu-id="27f01-136">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-136">eq</span></span>|
|<span data-ttu-id="27f01-137">userId</span><span class="sxs-lookup"><span data-stu-id="27f01-137">userId</span></span>|<span data-ttu-id="27f01-138">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-138">eq</span></span>|
|<span data-ttu-id="27f01-139">appId</span><span class="sxs-lookup"><span data-stu-id="27f01-139">appId</span></span>|<span data-ttu-id="27f01-140">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-140">eq</span></span>|
|<span data-ttu-id="27f01-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27f01-141">createdDateTime</span></span>| <span data-ttu-id="27f01-142">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="27f01-142">eq, le, ge</span></span>|
|<span data-ttu-id="27f01-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="27f01-143">userDisplayName</span></span>| <span data-ttu-id="27f01-144">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="27f01-144">eq, startswith</span></span>|
|<span data-ttu-id="27f01-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="27f01-145">userPrincipalName</span></span>| <span data-ttu-id="27f01-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="27f01-146">eq, startswith</span></span>|
|<span data-ttu-id="27f01-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="27f01-147">appDisplayName</span></span>| <span data-ttu-id="27f01-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="27f01-148">eq, startswith</span></span>|
|<span data-ttu-id="27f01-149">ipAddress</span><span class="sxs-lookup"><span data-stu-id="27f01-149">ipAddress</span></span>| <span data-ttu-id="27f01-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="27f01-150">eq, startswith</span></span>|
|<span data-ttu-id="27f01-151">location/city</span><span class="sxs-lookup"><span data-stu-id="27f01-151">location/city</span></span>| <span data-ttu-id="27f01-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="27f01-152">eq, startswith</span></span>|
|<span data-ttu-id="27f01-153">location/state</span><span class="sxs-lookup"><span data-stu-id="27f01-153">location/state</span></span>| <span data-ttu-id="27f01-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="27f01-154">eq, startswith</span></span>|
|<span data-ttu-id="27f01-155">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="27f01-155">location/countryOrRegion</span></span>| <span data-ttu-id="27f01-156">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="27f01-156">eq, startswith</span></span>|
|<span data-ttu-id="27f01-157">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="27f01-157">status/errorCode</span></span>|<span data-ttu-id="27f01-158">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-158">eq</span></span>|
|<span data-ttu-id="27f01-159">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="27f01-159">initiatedBy/user/id</span></span>|<span data-ttu-id="27f01-160">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-160">eq</span></span>|
|<span data-ttu-id="27f01-161">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="27f01-161">initiatedBy/user/displayName</span></span>| <span data-ttu-id="27f01-162">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-162">eq</span></span>|
|<span data-ttu-id="27f01-163">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="27f01-163">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="27f01-164">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="27f01-164">eq, startswith</span></span>|
|<span data-ttu-id="27f01-165">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="27f01-165">clientAppUsed</span></span>| <span data-ttu-id="27f01-166">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-166">eq</span></span>|
|<span data-ttu-id="27f01-167">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="27f01-167">conditionalAccessStatus</span></span> | <span data-ttu-id="27f01-168">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-168">eq</span></span>|
|<span data-ttu-id="27f01-169">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="27f01-169">deviceDetail/browser</span></span>| <span data-ttu-id="27f01-170">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="27f01-170">eq, startswith</span></span>|
|<span data-ttu-id="27f01-171">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="27f01-171">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="27f01-172">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="27f01-172">eq, startswith</span></span>|
|<span data-ttu-id="27f01-173">correlationId</span><span class="sxs-lookup"><span data-stu-id="27f01-173">correlationId</span></span>| <span data-ttu-id="27f01-174">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-174">eq</span></span>|
|<span data-ttu-id="27f01-175">riskDetail</span><span class="sxs-lookup"><span data-stu-id="27f01-175">riskDetail</span></span>| <span data-ttu-id="27f01-176">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-176">eq</span></span>|
|<span data-ttu-id="27f01-177">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="27f01-177">riskLevelAggregated</span></span>| <span data-ttu-id="27f01-178">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-178">eq</span></span>|
|<span data-ttu-id="27f01-179">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="27f01-179">riskLevelDuringSignIn</span></span>| <span data-ttu-id="27f01-180">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-180">eq</span></span>|
|<span data-ttu-id="27f01-181">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="27f01-181">riskEventTypes</span></span>| <span data-ttu-id="27f01-182">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-182">eq</span></span>|
|<span data-ttu-id="27f01-183">riskState</span><span class="sxs-lookup"><span data-stu-id="27f01-183">riskState</span></span>| <span data-ttu-id="27f01-184">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-184">eq</span></span>|
|<span data-ttu-id="27f01-185">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="27f01-185">originalRequestId</span></span>| <span data-ttu-id="27f01-186">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-186">eq</span></span>|
|<span data-ttu-id="27f01-187">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="27f01-187">tokenIssuerName</span></span>| <span data-ttu-id="27f01-188">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-188">eq</span></span>|
|<span data-ttu-id="27f01-189">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="27f01-189">tokenIssuerType</span></span>| <span data-ttu-id="27f01-190">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-190">eq</span></span>|
|<span data-ttu-id="27f01-191">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="27f01-191">resourceDisplayName</span></span>| <span data-ttu-id="27f01-192">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-192">eq</span></span>|
|<span data-ttu-id="27f01-193">resourceId</span><span class="sxs-lookup"><span data-stu-id="27f01-193">resourceId</span></span>| <span data-ttu-id="27f01-194">eq</span><span class="sxs-lookup"><span data-stu-id="27f01-194">eq</span></span>|


## <a name="response"></a><span data-ttu-id="27f01-195">响应</span><span class="sxs-lookup"><span data-stu-id="27f01-195">Response</span></span>
<span data-ttu-id="27f01-196">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="27f01-196">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27f01-197">示例</span><span class="sxs-lookup"><span data-stu-id="27f01-197">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27f01-198">请求</span><span class="sxs-lookup"><span data-stu-id="27f01-198">Request</span></span>
<span data-ttu-id="27f01-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27f01-199">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="27f01-200">响应</span><span class="sxs-lookup"><span data-stu-id="27f01-200">Response</span></span>
<span data-ttu-id="27f01-201">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="27f01-201">Here is an example of the response.</span></span> 

><span data-ttu-id="27f01-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="27f01-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 264
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="27f01-204">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="27f01-204">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="27f01-205">C#</span><span class="sxs-lookup"><span data-stu-id="27f01-205">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signins-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27f01-206">Javascript</span><span class="sxs-lookup"><span data-stu-id="27f01-206">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signins-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id":"b01b1726-0147-425e-a7f7-21f252050400",
        "createdDateTime":"2018-11-06T18:48:33.8527147Z",
        "userDisplayName":"Jon Doe",
         "userPrincipalName":"admin@aad171.ccsctp.net",
         "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
        "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
         "appDisplayName":"Azure Portal",
         "ipAddress":"207.254.19.10",
         "clientAppUsed":"Browser",
        "mfaDetail":null,
         "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
         "conditionalAccessStatus":"notApplied",
        "originalRequestId":null,
        "isInteractive":true,
        "tokenIssuerName":null,
        "tokenIssuerType":"AzureAD",
        "processingTimeInMilliseconds":0,
        "riskDetail":"none",
        "riskLevelAggregated":"none",
        "riskLevelDuringSignIn":"none",
        "riskState":"none",
        "riskEventTypes":[

        ],
        "resourceDisplayName":"windows azure service management api",
        "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
        "authenticationMethodsUsed":[

        ],
        "status":{
            "errorCode":50140,
            "failureReason":"This error occurred due to 'Keep me signed in' interrupt when the user was signing-in.",
            "additionalDetails":null
        },
        "deviceDetail":{
            "deviceId":null,
            "displayName":null,
            "operatingSystem":"Windows 7",
            "browser":"Chrome 63.0.3239",
            "isCompliant":null,
            "isManaged":null,
            "trustType":null
        },
        "location":{
            "city":"Lithia Springs",
            "state":"Georgia",
            "countryOrRegion":"US",
            "geoCoordinates":{
                "altitude":null,
                "latitude":33.7930908203125,
                "longitude":-84.445358276367188
            }
        },
        "appliedConditionalAccessPolicies":[
            {
            "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
            "displayName":"New Name here4",
            "enforcedGrantControls":[
                "Mfa",
                "RequireCompliantDevice"
            ],
            "enforcedSessionControls":[

            ],
            "result":"notApplied"
            },
            {
            "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
            "displayName":"PipelineTest4",
            "enforcedGrantControls":[

            ],
            "enforcedSessionControls":[

            ],
            "result":"notEnabled"
            }
        ],
        "authenticationProcessingDetails":[

        ],
        "networkLocationDetails":[

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
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
