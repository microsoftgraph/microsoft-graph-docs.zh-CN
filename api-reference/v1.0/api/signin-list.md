---
title: 列出 signIn
description: 介绍 Microsoft Graph API 中登录资源 (实体) 的列表方法。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3052ee368667f14932167f5a5d25dd168ab74264
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279273"
---
# <a name="list-signins"></a><span data-ttu-id="640e5-103">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="640e5-103">List signIns</span></span>

<span data-ttu-id="640e5-104">检索租户的 Azure AD 用户登录信息。</span><span class="sxs-lookup"><span data-stu-id="640e5-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="640e5-105">在性质 (用户名/密码作为身份验证令牌的一部分传递) 和成功的联合登录中当前包括在登录日志中的登录登录。</span><span class="sxs-lookup"><span data-stu-id="640e5-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="640e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="640e5-106">Permissions</span></span>

<span data-ttu-id="640e5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="640e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="640e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="640e5-109">Permission type</span></span>      | <span data-ttu-id="640e5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="640e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="640e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="640e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="640e5-112">AuditLog 和所有目录。全部读取. 所有</span><span class="sxs-lookup"><span data-stu-id="640e5-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="640e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="640e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="640e5-114">不支持</span><span class="sxs-lookup"><span data-stu-id="640e5-114">Not supported</span></span>   |
|<span data-ttu-id="640e5-115">应用</span><span class="sxs-lookup"><span data-stu-id="640e5-115">Application</span></span> | <span data-ttu-id="640e5-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="640e5-116">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="640e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="640e5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="640e5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="640e5-118">Optional query parameters</span></span>

<span data-ttu-id="640e5-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="640e5-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="640e5-120">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="640e5-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="640e5-121">名称</span><span class="sxs-lookup"><span data-stu-id="640e5-121">Name</span></span>     |<span data-ttu-id="640e5-122">说明</span><span class="sxs-lookup"><span data-stu-id="640e5-122">Description</span></span>                            |<span data-ttu-id="640e5-123">示例</span><span class="sxs-lookup"><span data-stu-id="640e5-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="640e5-124">$filter</span><span class="sxs-lookup"><span data-stu-id="640e5-124">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="640e5-125">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="640e5-125">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="640e5-126">$top</span><span class="sxs-lookup"><span data-stu-id="640e5-126">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="640e5-127">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="640e5-127">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="640e5-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="640e5-128">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="640e5-129">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="640e5-129">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="640e5-130">$Filter 参数支持的属性</span><span class="sxs-lookup"><span data-stu-id="640e5-130">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="640e5-131">属性名</span><span class="sxs-lookup"><span data-stu-id="640e5-131">Attribute name</span></span> |<span data-ttu-id="640e5-132">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="640e5-132">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="640e5-133">id</span><span class="sxs-lookup"><span data-stu-id="640e5-133">id</span></span>|<span data-ttu-id="640e5-134">eq</span><span class="sxs-lookup"><span data-stu-id="640e5-134">eq</span></span>|
|<span data-ttu-id="640e5-135">userId</span><span class="sxs-lookup"><span data-stu-id="640e5-135">userId</span></span>|<span data-ttu-id="640e5-136">eq</span><span class="sxs-lookup"><span data-stu-id="640e5-136">eq</span></span>|
|<span data-ttu-id="640e5-137">appId</span><span class="sxs-lookup"><span data-stu-id="640e5-137">appId</span></span>|<span data-ttu-id="640e5-138">eq</span><span class="sxs-lookup"><span data-stu-id="640e5-138">eq</span></span>|
|<span data-ttu-id="640e5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="640e5-139">createdDateTime</span></span>| <span data-ttu-id="640e5-140">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="640e5-140">eq, le, ge</span></span>|
|<span data-ttu-id="640e5-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="640e5-141">userDisplayName</span></span>| <span data-ttu-id="640e5-142">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="640e5-142">eq, startswith</span></span>|
|<span data-ttu-id="640e5-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="640e5-143">userPrincipalName</span></span>| <span data-ttu-id="640e5-144">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="640e5-144">eq, startswith</span></span>|
|<span data-ttu-id="640e5-145">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="640e5-145">appDisplayName</span></span>| <span data-ttu-id="640e5-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="640e5-146">eq, startswith</span></span>|
|<span data-ttu-id="640e5-147">ipAddress</span><span class="sxs-lookup"><span data-stu-id="640e5-147">ipAddress</span></span>| <span data-ttu-id="640e5-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="640e5-148">eq, startswith</span></span>|
|<span data-ttu-id="640e5-149">location/city</span><span class="sxs-lookup"><span data-stu-id="640e5-149">location/city</span></span>| <span data-ttu-id="640e5-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="640e5-150">eq, startswith</span></span>|
|<span data-ttu-id="640e5-151">location/state</span><span class="sxs-lookup"><span data-stu-id="640e5-151">location/state</span></span>| <span data-ttu-id="640e5-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="640e5-152">eq, startswith</span></span>|
|<span data-ttu-id="640e5-153">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="640e5-153">location/countryOrRegion</span></span>| <span data-ttu-id="640e5-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="640e5-154">eq, startswith</span></span>|
|<span data-ttu-id="640e5-155">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="640e5-155">status/errorCode</span></span>|<span data-ttu-id="640e5-156">eq</span><span class="sxs-lookup"><span data-stu-id="640e5-156">eq</span></span>|
|<span data-ttu-id="640e5-157">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="640e5-157">initiatedBy/user/id</span></span>|<span data-ttu-id="640e5-158">eq</span><span class="sxs-lookup"><span data-stu-id="640e5-158">eq</span></span>|
|<span data-ttu-id="640e5-159">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="640e5-159">initiatedBy/user/displayName</span></span>| <span data-ttu-id="640e5-160">eq</span><span class="sxs-lookup"><span data-stu-id="640e5-160">eq</span></span>|
|<span data-ttu-id="640e5-161">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="640e5-161">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="640e5-162">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="640e5-162">eq, startswith</span></span>|
|<span data-ttu-id="640e5-163">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="640e5-163">clientAppUsed</span></span>| <span data-ttu-id="640e5-164">eq</span><span class="sxs-lookup"><span data-stu-id="640e5-164">eq</span></span>|
|<span data-ttu-id="640e5-165">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="640e5-165">conditionalAccessStatus</span></span> | <span data-ttu-id="640e5-166">eq</span><span class="sxs-lookup"><span data-stu-id="640e5-166">eq</span></span>|
|<span data-ttu-id="640e5-167">deviceDetails/浏览器</span><span class="sxs-lookup"><span data-stu-id="640e5-167">deviceDetails/browser</span></span>| <span data-ttu-id="640e5-168">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="640e5-168">eq, startswith</span></span>|
|<span data-ttu-id="640e5-169">deviceDetails/操作系统</span><span class="sxs-lookup"><span data-stu-id="640e5-169">deviceDetails/operatingSystem</span></span>| <span data-ttu-id="640e5-170">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="640e5-170">eq, startswith</span></span>|
|<span data-ttu-id="640e5-171">correlationId</span><span class="sxs-lookup"><span data-stu-id="640e5-171">correlationId</span></span>| <span data-ttu-id="640e5-172">eq</span><span class="sxs-lookup"><span data-stu-id="640e5-172">eq</span></span>|
|<span data-ttu-id="640e5-173">isRisky</span><span class="sxs-lookup"><span data-stu-id="640e5-173">isRisky</span></span>| <span data-ttu-id="640e5-174">eq</span><span class="sxs-lookup"><span data-stu-id="640e5-174">eq</span></span>|

## <a name="response"></a><span data-ttu-id="640e5-175">响应</span><span class="sxs-lookup"><span data-stu-id="640e5-175">Response</span></span>

<span data-ttu-id="640e5-176">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="640e5-176">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="640e5-177">示例</span><span class="sxs-lookup"><span data-stu-id="640e5-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="640e5-178">请求</span><span class="sxs-lookup"><span data-stu-id="640e5-178">Request</span></span>

<span data-ttu-id="640e5-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="640e5-179">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```

### <a name="response"></a><span data-ttu-id="640e5-180">响应</span><span class="sxs-lookup"><span data-stu-id="640e5-180">Response</span></span>

<span data-ttu-id="640e5-181">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="640e5-181">Here is an example of the response.</span></span>
><span data-ttu-id="640e5-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="640e5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="640e5-184">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="640e5-184">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="640e5-185">C#</span><span class="sxs-lookup"><span data-stu-id="640e5-185">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list_signins-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="640e5-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="640e5-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list_signins-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="640e5-187">目标-C</span><span class="sxs-lookup"><span data-stu-id="640e5-187">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list_signins-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "value": [{
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
    }]
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
    "Error: /api-reference/v1.0/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
