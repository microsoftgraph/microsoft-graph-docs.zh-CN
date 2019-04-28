---
title: 列出 signIn
description: 检索租户的 Azure AD 用户登录名。 登录日志中目前包含交互式性质的登录名（其中用户名/密码作为授权令牌的一部分传递）和已成功联合的登录名。  首先返回最新 signIn。
localization_priority: Priority
ms.openlocfilehash: 8596bd168a3e10cbea9e15e2f61d6bd668fd27b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545155"
---
# <a name="list-signins"></a><span data-ttu-id="37797-105">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="37797-105">List sign-ins</span></span>

<span data-ttu-id="37797-106">检索租户的 Azure AD 用户登录名。</span><span class="sxs-lookup"><span data-stu-id="37797-106">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="37797-107">登录日志中目前包含交互式性质的登录名（其中用户名/密码作为授权令牌的一部分传递）和已成功联合的登录名。</span><span class="sxs-lookup"><span data-stu-id="37797-107">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="37797-108">首先返回最新 signIn。</span><span class="sxs-lookup"><span data-stu-id="37797-108">The most recent signIns are returned first.</span></span>


## <a name="permissions"></a><span data-ttu-id="37797-109">权限</span><span class="sxs-lookup"><span data-stu-id="37797-109">Permissions</span></span>
<span data-ttu-id="37797-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37797-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37797-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="37797-112">Permission type</span></span>      | <span data-ttu-id="37797-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37797-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37797-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37797-114">Delegated (work or school account)</span></span> | <span data-ttu-id="37797-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="37797-115">AuditLog.Read.All</span></span> |
|<span data-ttu-id="37797-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37797-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37797-117">不支持</span><span class="sxs-lookup"><span data-stu-id="37797-117">Not supported</span></span>   |
|<span data-ttu-id="37797-118">应用</span><span class="sxs-lookup"><span data-stu-id="37797-118">Application</span></span> | <span data-ttu-id="37797-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="37797-119">AuditLog.Read.All</span></span> | 

<span data-ttu-id="37797-120">此外，应用还必须向 Azure AD [正确注册](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="37797-120">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="37797-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37797-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="37797-122">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="37797-122">Optional query parameters</span></span>
<span data-ttu-id="37797-123">此方法支持以下 OData 查询参数，它们有助于自定义响应。</span><span class="sxs-lookup"><span data-stu-id="37797-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="37797-124">请参看 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)，了解如何使用这些参数。</span><span class="sxs-lookup"><span data-stu-id="37797-124">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

|<span data-ttu-id="37797-125">名称</span><span class="sxs-lookup"><span data-stu-id="37797-125">Name</span></span>     |<span data-ttu-id="37797-126">说明</span><span class="sxs-lookup"><span data-stu-id="37797-126">Description</span></span>                            |<span data-ttu-id="37797-127">示例</span><span class="sxs-lookup"><span data-stu-id="37797-127">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="37797-128">$filter</span><span class="sxs-lookup"><span data-stu-id="37797-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="37797-129">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="37797-129">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="37797-130">$top</span><span class="sxs-lookup"><span data-stu-id="37797-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="37797-131">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="37797-131">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="37797-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="37797-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="37797-133">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="37797-133">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="37797-134">$filter 参数支持的属性列表</span><span class="sxs-lookup"><span data-stu-id="37797-134">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="37797-135">属性名</span><span class="sxs-lookup"><span data-stu-id="37797-135">Attribute Name</span></span> |<span data-ttu-id="37797-136">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="37797-136">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="37797-137">id</span><span class="sxs-lookup"><span data-stu-id="37797-137">id</span></span>|<span data-ttu-id="37797-138">eq</span><span class="sxs-lookup"><span data-stu-id="37797-138">eq</span></span>|
|<span data-ttu-id="37797-139">userId</span><span class="sxs-lookup"><span data-stu-id="37797-139">userId</span></span>|<span data-ttu-id="37797-140">eq</span><span class="sxs-lookup"><span data-stu-id="37797-140">eq</span></span>|
|<span data-ttu-id="37797-141">appId</span><span class="sxs-lookup"><span data-stu-id="37797-141">appId</span></span>|<span data-ttu-id="37797-142">eq</span><span class="sxs-lookup"><span data-stu-id="37797-142">eq</span></span>|
|<span data-ttu-id="37797-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37797-143">createdDateTime</span></span>| <span data-ttu-id="37797-144">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="37797-144">eq, ge, le</span></span>|
|<span data-ttu-id="37797-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="37797-145">userDisplayName</span></span>| <span data-ttu-id="37797-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="37797-146">eq, startswith</span></span>|
|<span data-ttu-id="37797-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="37797-147">userPrincipalName</span></span>| <span data-ttu-id="37797-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="37797-148">eq, startswith</span></span>|
|<span data-ttu-id="37797-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="37797-149">appDisplayName</span></span>| <span data-ttu-id="37797-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="37797-150">eq, startswith</span></span>|
|<span data-ttu-id="37797-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="37797-151">ipAddress</span></span>| <span data-ttu-id="37797-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="37797-152">eq, startswith</span></span>|
|<span data-ttu-id="37797-153">location/city</span><span class="sxs-lookup"><span data-stu-id="37797-153">location/city</span></span>| <span data-ttu-id="37797-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="37797-154">eq, startswith</span></span>|
|<span data-ttu-id="37797-155">location/state</span><span class="sxs-lookup"><span data-stu-id="37797-155">location/state</span></span>| <span data-ttu-id="37797-156">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="37797-156">eq, startswith</span></span>|
|<span data-ttu-id="37797-157">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="37797-157">location/countryOrRegion</span></span>| <span data-ttu-id="37797-158">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="37797-158">eq, startswith</span></span>|
|<span data-ttu-id="37797-159">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="37797-159">status/errorCode</span></span>|<span data-ttu-id="37797-160">eq</span><span class="sxs-lookup"><span data-stu-id="37797-160">eq</span></span>|
|<span data-ttu-id="37797-161">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="37797-161">initiatedBy/user/id</span></span>|<span data-ttu-id="37797-162">eq</span><span class="sxs-lookup"><span data-stu-id="37797-162">eq</span></span>|
|<span data-ttu-id="37797-163">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="37797-163">initiatedBy/user/displayName</span></span>| <span data-ttu-id="37797-164">eq</span><span class="sxs-lookup"><span data-stu-id="37797-164">eq</span></span>|
|<span data-ttu-id="37797-165">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="37797-165">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="37797-166">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="37797-166">eq, startswith</span></span>|
|<span data-ttu-id="37797-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="37797-167">clientAppUsed</span></span>| <span data-ttu-id="37797-168">eq</span><span class="sxs-lookup"><span data-stu-id="37797-168">eq</span></span>|
|<span data-ttu-id="37797-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="37797-169">conditionalAccessStatus</span></span> | <span data-ttu-id="37797-170">eq</span><span class="sxs-lookup"><span data-stu-id="37797-170">eq</span></span>|
|<span data-ttu-id="37797-171">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="37797-171">deviceDetail/browser</span></span>| <span data-ttu-id="37797-172">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="37797-172">eq, startswith</span></span>|
|<span data-ttu-id="37797-173">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="37797-173">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="37797-174">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="37797-174">eq, startswith</span></span>|
|<span data-ttu-id="37797-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="37797-175">correlationId</span></span>| <span data-ttu-id="37797-176">eq</span><span class="sxs-lookup"><span data-stu-id="37797-176">eq</span></span>|
|<span data-ttu-id="37797-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="37797-177">riskDetail</span></span>| <span data-ttu-id="37797-178">eq</span><span class="sxs-lookup"><span data-stu-id="37797-178">eq</span></span>|
|<span data-ttu-id="37797-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="37797-179">riskLevelAggregated</span></span>| <span data-ttu-id="37797-180">eq</span><span class="sxs-lookup"><span data-stu-id="37797-180">eq</span></span>|
|<span data-ttu-id="37797-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="37797-181">riskLevelDuringSignIn</span></span>| <span data-ttu-id="37797-182">eq</span><span class="sxs-lookup"><span data-stu-id="37797-182">eq</span></span>|
|<span data-ttu-id="37797-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="37797-183">riskEventTypes</span></span>| <span data-ttu-id="37797-184">eq</span><span class="sxs-lookup"><span data-stu-id="37797-184">eq</span></span>|
|<span data-ttu-id="37797-185">riskState</span><span class="sxs-lookup"><span data-stu-id="37797-185">riskState</span></span>| <span data-ttu-id="37797-186">eq</span><span class="sxs-lookup"><span data-stu-id="37797-186">eq</span></span>|
|<span data-ttu-id="37797-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="37797-187">originalRequestId</span></span>| <span data-ttu-id="37797-188">eq</span><span class="sxs-lookup"><span data-stu-id="37797-188">eq</span></span>|
|<span data-ttu-id="37797-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="37797-189">tokenIssuerName</span></span>| <span data-ttu-id="37797-190">eq</span><span class="sxs-lookup"><span data-stu-id="37797-190">eq</span></span>|
|<span data-ttu-id="37797-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="37797-191">tokenIssuerType</span></span>| <span data-ttu-id="37797-192">eq</span><span class="sxs-lookup"><span data-stu-id="37797-192">eq</span></span>|
|<span data-ttu-id="37797-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="37797-193">resourceDisplayName</span></span>| <span data-ttu-id="37797-194">eq</span><span class="sxs-lookup"><span data-stu-id="37797-194">eq</span></span>|
|<span data-ttu-id="37797-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="37797-195">resourceId</span></span>| <span data-ttu-id="37797-196">eq</span><span class="sxs-lookup"><span data-stu-id="37797-196">eq</span></span>|


## <a name="response"></a><span data-ttu-id="37797-197">响应</span><span class="sxs-lookup"><span data-stu-id="37797-197">Response</span></span>
<span data-ttu-id="37797-198">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="37797-198">If successful, this method returns a `200 OK` response code and collection of [directoryAudit](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="37797-199">示例</span><span class="sxs-lookup"><span data-stu-id="37797-199">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37797-200">请求</span><span class="sxs-lookup"><span data-stu-id="37797-200">Request</span></span>
<span data-ttu-id="37797-201">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37797-201">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="37797-202">响应</span><span class="sxs-lookup"><span data-stu-id="37797-202">Response</span></span>
<span data-ttu-id="37797-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="37797-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
