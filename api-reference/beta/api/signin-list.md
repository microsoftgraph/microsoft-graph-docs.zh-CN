---
title: 列表 signIns
description: 检索 Azure AD 用户登录您的租户。 在登录日志中当前包括交互中 （其中用户名/密码作为授权令牌的一部分传递） 的性质和成功联合的登录的登录。  最新 signIns 是首先返回。
ms.openlocfilehash: 3abca59187dcc9667789e33bcefc1bcc51d5ab10
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043088"
---
# <a name="list-signins"></a><span data-ttu-id="30163-105">列表 signIns</span><span class="sxs-lookup"><span data-stu-id="30163-105">List signIns</span></span>

<span data-ttu-id="30163-106">检索 Azure AD 用户登录您的租户。</span><span class="sxs-lookup"><span data-stu-id="30163-106">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="30163-107">在登录日志中当前包括交互中 （其中用户名/密码作为授权令牌的一部分传递） 的性质和成功联合的登录的登录。</span><span class="sxs-lookup"><span data-stu-id="30163-107">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="30163-108">最新 signIns 是首先返回。</span><span class="sxs-lookup"><span data-stu-id="30163-108">The most recent signIns are returned first.</span></span>


## <a name="permissions"></a><span data-ttu-id="30163-109">权限</span><span class="sxs-lookup"><span data-stu-id="30163-109">Permissions</span></span>
<span data-ttu-id="30163-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30163-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30163-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="30163-112">Permission type</span></span>      | <span data-ttu-id="30163-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30163-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30163-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30163-114">Delegated (work or school account)</span></span> | <span data-ttu-id="30163-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="30163-115">AuditLog.Read.All</span></span> |
|<span data-ttu-id="30163-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30163-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30163-117">不支持</span><span class="sxs-lookup"><span data-stu-id="30163-117">Not supported</span></span>   |
|<span data-ttu-id="30163-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="30163-118">Application</span></span> | <span data-ttu-id="30163-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="30163-119">AuditLog.Read.All</span></span> | 

<span data-ttu-id="30163-120">此外，应用程序必须采用到 Azure AD 中[正确注册](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="30163-120">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="30163-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30163-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="30163-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="30163-122">Optional query parameters</span></span>
<span data-ttu-id="30163-123">此方法支持以下 OData 查询参数，有助于自定义响应。</span><span class="sxs-lookup"><span data-stu-id="30163-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="30163-124">查看有关如何使用这些参数的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="30163-124">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

|<span data-ttu-id="30163-125">名称</span><span class="sxs-lookup"><span data-stu-id="30163-125">Name</span></span>     |<span data-ttu-id="30163-126">说明</span><span class="sxs-lookup"><span data-stu-id="30163-126">Description</span></span>                            |<span data-ttu-id="30163-127">示例</span><span class="sxs-lookup"><span data-stu-id="30163-127">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="30163-128">$filter</span><span class="sxs-lookup"><span data-stu-id="30163-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="30163-129">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="30163-129">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="30163-130">$top</span><span class="sxs-lookup"><span data-stu-id="30163-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="30163-131">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="30163-131">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="30163-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="30163-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="30163-133">检索下一步页的结果的结果集跨越多个页面。</span><span class="sxs-lookup"><span data-stu-id="30163-133">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="30163-134">支持的 $filter 参数属性的列表</span><span class="sxs-lookup"><span data-stu-id="30163-134">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="30163-135">属性名称</span><span class="sxs-lookup"><span data-stu-id="30163-135">Attribute Name</span></span> |<span data-ttu-id="30163-136">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="30163-136">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="30163-137">id</span><span class="sxs-lookup"><span data-stu-id="30163-137">id</span></span>|<span data-ttu-id="30163-138">eq</span><span class="sxs-lookup"><span data-stu-id="30163-138">eq</span></span>|
|<span data-ttu-id="30163-139">userId</span><span class="sxs-lookup"><span data-stu-id="30163-139">userId</span></span>|<span data-ttu-id="30163-140">eq</span><span class="sxs-lookup"><span data-stu-id="30163-140">eq</span></span>|
|<span data-ttu-id="30163-141">appId</span><span class="sxs-lookup"><span data-stu-id="30163-141">appId</span></span>|<span data-ttu-id="30163-142">eq</span><span class="sxs-lookup"><span data-stu-id="30163-142">eq</span></span>|
|<span data-ttu-id="30163-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30163-143">createdDateTime</span></span>| <span data-ttu-id="30163-144">eq，le，ge</span><span class="sxs-lookup"><span data-stu-id="30163-144">eq, le, ge</span></span>|
|<span data-ttu-id="30163-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="30163-145">userDisplayName</span></span>| <span data-ttu-id="30163-146">eq startswith</span><span class="sxs-lookup"><span data-stu-id="30163-146">eq, startswith</span></span>|
|<span data-ttu-id="30163-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="30163-147">userPrincipalName</span></span>| <span data-ttu-id="30163-148">eq startswith</span><span class="sxs-lookup"><span data-stu-id="30163-148">eq, startswith</span></span>|
|<span data-ttu-id="30163-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="30163-149">appDisplayName</span></span>| <span data-ttu-id="30163-150">eq startswith</span><span class="sxs-lookup"><span data-stu-id="30163-150">eq, startswith</span></span>|
|<span data-ttu-id="30163-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="30163-151">ipAddress</span></span>| <span data-ttu-id="30163-152">eq startswith</span><span class="sxs-lookup"><span data-stu-id="30163-152">eq, startswith</span></span>|
|<span data-ttu-id="30163-153">城市 /</span><span class="sxs-lookup"><span data-stu-id="30163-153">location/city</span></span>| <span data-ttu-id="30163-154">eq startswith</span><span class="sxs-lookup"><span data-stu-id="30163-154">eq, startswith</span></span>|
|<span data-ttu-id="30163-155">位置/状态</span><span class="sxs-lookup"><span data-stu-id="30163-155">location/state</span></span>| <span data-ttu-id="30163-156">eq startswith</span><span class="sxs-lookup"><span data-stu-id="30163-156">eq, startswith</span></span>|
|<span data-ttu-id="30163-157">位置/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="30163-157">location/countryOrRegion</span></span>| <span data-ttu-id="30163-158">eq startswith</span><span class="sxs-lookup"><span data-stu-id="30163-158">eq, startswith</span></span>|
|<span data-ttu-id="30163-159">状态/错误代码</span><span class="sxs-lookup"><span data-stu-id="30163-159">status/errorCode</span></span>|<span data-ttu-id="30163-160">eq</span><span class="sxs-lookup"><span data-stu-id="30163-160">eq</span></span>|
|<span data-ttu-id="30163-161">initiatedBy/用户/id</span><span class="sxs-lookup"><span data-stu-id="30163-161">initiatedBy/user/id</span></span>|<span data-ttu-id="30163-162">eq</span><span class="sxs-lookup"><span data-stu-id="30163-162">eq</span></span>|
|<span data-ttu-id="30163-163">initiatedBy/用户/displayName</span><span class="sxs-lookup"><span data-stu-id="30163-163">initiatedBy/user/displayName</span></span>| <span data-ttu-id="30163-164">eq</span><span class="sxs-lookup"><span data-stu-id="30163-164">eq</span></span>|
|<span data-ttu-id="30163-165">userprincipalname 属性 initiatedBy/用户</span><span class="sxs-lookup"><span data-stu-id="30163-165">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="30163-166">eq startswith</span><span class="sxs-lookup"><span data-stu-id="30163-166">eq, startswith</span></span>|
|<span data-ttu-id="30163-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="30163-167">clientAppUsed</span></span>| <span data-ttu-id="30163-168">eq</span><span class="sxs-lookup"><span data-stu-id="30163-168">eq</span></span>|
|<span data-ttu-id="30163-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="30163-169">conditionalAccessStatus</span></span> | <span data-ttu-id="30163-170">eq</span><span class="sxs-lookup"><span data-stu-id="30163-170">eq</span></span>|
|<span data-ttu-id="30163-171">deviceDetail/浏览器</span><span class="sxs-lookup"><span data-stu-id="30163-171">deviceDetail/browser</span></span>| <span data-ttu-id="30163-172">eq startswith</span><span class="sxs-lookup"><span data-stu-id="30163-172">eq, startswith</span></span>|
|<span data-ttu-id="30163-173">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="30163-173">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="30163-174">eq startswith</span><span class="sxs-lookup"><span data-stu-id="30163-174">eq, startswith</span></span>|
|<span data-ttu-id="30163-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="30163-175">correlationId</span></span>| <span data-ttu-id="30163-176">eq</span><span class="sxs-lookup"><span data-stu-id="30163-176">eq</span></span>|
|<span data-ttu-id="30163-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="30163-177">riskDetail</span></span>| <span data-ttu-id="30163-178">eq</span><span class="sxs-lookup"><span data-stu-id="30163-178">eq</span></span>|
|<span data-ttu-id="30163-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="30163-179">riskLevelAggregated</span></span>| <span data-ttu-id="30163-180">eq</span><span class="sxs-lookup"><span data-stu-id="30163-180">eq</span></span>|
|<span data-ttu-id="30163-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="30163-181">riskLevelDuringSignIn</span></span>| <span data-ttu-id="30163-182">eq</span><span class="sxs-lookup"><span data-stu-id="30163-182">eq</span></span>|
|<span data-ttu-id="30163-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="30163-183">riskEventTypes</span></span>| <span data-ttu-id="30163-184">eq</span><span class="sxs-lookup"><span data-stu-id="30163-184">eq</span></span>|
|<span data-ttu-id="30163-185">riskState</span><span class="sxs-lookup"><span data-stu-id="30163-185">riskState</span></span>| <span data-ttu-id="30163-186">eq</span><span class="sxs-lookup"><span data-stu-id="30163-186">eq</span></span>|
|<span data-ttu-id="30163-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="30163-187">originalRequestId</span></span>| <span data-ttu-id="30163-188">eq</span><span class="sxs-lookup"><span data-stu-id="30163-188">eq</span></span>|
|<span data-ttu-id="30163-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="30163-189">tokenIssuerName</span></span>| <span data-ttu-id="30163-190">eq</span><span class="sxs-lookup"><span data-stu-id="30163-190">eq</span></span>|
|<span data-ttu-id="30163-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="30163-191">tokenIssuerType</span></span>| <span data-ttu-id="30163-192">eq</span><span class="sxs-lookup"><span data-stu-id="30163-192">eq</span></span>|
|<span data-ttu-id="30163-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="30163-193">resourceDisplayName</span></span>| <span data-ttu-id="30163-194">eq</span><span class="sxs-lookup"><span data-stu-id="30163-194">eq</span></span>|
|<span data-ttu-id="30163-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="30163-195">resourceId</span></span>| <span data-ttu-id="30163-196">eq</span><span class="sxs-lookup"><span data-stu-id="30163-196">eq</span></span>|


## <a name="response"></a><span data-ttu-id="30163-197">响应</span><span class="sxs-lookup"><span data-stu-id="30163-197">Response</span></span>
<span data-ttu-id="30163-198">如果成功，此方法返回`200 OK`响应代码和响应正文中的[登录](../resources/signin.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="30163-198">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30163-199">示例</span><span class="sxs-lookup"><span data-stu-id="30163-199">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30163-200">请求</span><span class="sxs-lookup"><span data-stu-id="30163-200">Request</span></span>
<span data-ttu-id="30163-201">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30163-201">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="30163-202">响应</span><span class="sxs-lookup"><span data-stu-id="30163-202">Response</span></span>
<span data-ttu-id="30163-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30163-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
