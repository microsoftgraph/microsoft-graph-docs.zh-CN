---
title: 列出 signIn
description: 介绍 Microsoft Graph API 中登录资源 (实体) 的列表方法。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0e619f0d5577ffe4db91142eccc257d9fa93e643
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729250"
---
# <a name="list-signins"></a><span data-ttu-id="fb1c1-103">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="fb1c1-103">List signIns</span></span>

<span data-ttu-id="fb1c1-104">检索租户的 Azure AD 用户登录信息。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="fb1c1-105">在性质 (用户名/密码作为身份验证令牌的一部分传递) 和成功的联合登录中当前包括在登录日志中的登录登录。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb1c1-106">权限</span><span class="sxs-lookup"><span data-stu-id="fb1c1-106">Permissions</span></span>

<span data-ttu-id="fb1c1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="fb1c1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb1c1-109">Permission type</span></span>      | <span data-ttu-id="fb1c1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb1c1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb1c1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb1c1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fb1c1-112">AuditLog 和所有目录。全部读取. 所有</span><span class="sxs-lookup"><span data-stu-id="fb1c1-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="fb1c1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb1c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb1c1-114">不支持</span><span class="sxs-lookup"><span data-stu-id="fb1c1-114">Not supported</span></span>   |
|<span data-ttu-id="fb1c1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb1c1-115">Application</span></span> | <span data-ttu-id="fb1c1-116">AuditLog 和所有目录。全部读取. 所有</span><span class="sxs-lookup"><span data-stu-id="fb1c1-116">AuditLog.Read.All and Directory.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fb1c1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb1c1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb1c1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fb1c1-118">Optional query parameters</span></span>

<span data-ttu-id="fb1c1-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="fb1c1-120">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="fb1c1-121">名称</span><span class="sxs-lookup"><span data-stu-id="fb1c1-121">Name</span></span>     |<span data-ttu-id="fb1c1-122">说明</span><span class="sxs-lookup"><span data-stu-id="fb1c1-122">Description</span></span>                            |<span data-ttu-id="fb1c1-123">示例</span><span class="sxs-lookup"><span data-stu-id="fb1c1-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="fb1c1-124">$filter</span><span class="sxs-lookup"><span data-stu-id="fb1c1-124">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="fb1c1-125">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-125">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="fb1c1-126">$top</span><span class="sxs-lookup"><span data-stu-id="fb1c1-126">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="fb1c1-127">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-127">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="fb1c1-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="fb1c1-128">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="fb1c1-129">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-129">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="fb1c1-130">$filter 参数支持的属性</span><span class="sxs-lookup"><span data-stu-id="fb1c1-130">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="fb1c1-131">属性名</span><span class="sxs-lookup"><span data-stu-id="fb1c1-131">Attribute name</span></span> |<span data-ttu-id="fb1c1-132">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="fb1c1-132">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="fb1c1-133">id</span><span class="sxs-lookup"><span data-stu-id="fb1c1-133">id</span></span>|<span data-ttu-id="fb1c1-134">eq</span><span class="sxs-lookup"><span data-stu-id="fb1c1-134">eq</span></span>|
|<span data-ttu-id="fb1c1-135">userId</span><span class="sxs-lookup"><span data-stu-id="fb1c1-135">userId</span></span>|<span data-ttu-id="fb1c1-136">eq</span><span class="sxs-lookup"><span data-stu-id="fb1c1-136">eq</span></span>|
|<span data-ttu-id="fb1c1-137">appId</span><span class="sxs-lookup"><span data-stu-id="fb1c1-137">appId</span></span>|<span data-ttu-id="fb1c1-138">eq</span><span class="sxs-lookup"><span data-stu-id="fb1c1-138">eq</span></span>|
|<span data-ttu-id="fb1c1-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb1c1-139">createdDateTime</span></span>| <span data-ttu-id="fb1c1-140">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="fb1c1-140">eq, le, ge</span></span>|
|<span data-ttu-id="fb1c1-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fb1c1-141">userDisplayName</span></span>| <span data-ttu-id="fb1c1-142">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="fb1c1-142">eq, startswith</span></span>|
|<span data-ttu-id="fb1c1-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fb1c1-143">userPrincipalName</span></span>| <span data-ttu-id="fb1c1-144">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="fb1c1-144">eq, startswith</span></span>|
|<span data-ttu-id="fb1c1-145">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="fb1c1-145">appDisplayName</span></span>| <span data-ttu-id="fb1c1-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="fb1c1-146">eq, startswith</span></span>|
|<span data-ttu-id="fb1c1-147">ipAddress</span><span class="sxs-lookup"><span data-stu-id="fb1c1-147">ipAddress</span></span>| <span data-ttu-id="fb1c1-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="fb1c1-148">eq, startswith</span></span>|
|<span data-ttu-id="fb1c1-149">location/city</span><span class="sxs-lookup"><span data-stu-id="fb1c1-149">location/city</span></span>| <span data-ttu-id="fb1c1-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="fb1c1-150">eq, startswith</span></span>|
|<span data-ttu-id="fb1c1-151">location/state</span><span class="sxs-lookup"><span data-stu-id="fb1c1-151">location/state</span></span>| <span data-ttu-id="fb1c1-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="fb1c1-152">eq, startswith</span></span>|
|<span data-ttu-id="fb1c1-153">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="fb1c1-153">location/countryOrRegion</span></span>| <span data-ttu-id="fb1c1-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="fb1c1-154">eq, startswith</span></span>|
|<span data-ttu-id="fb1c1-155">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="fb1c1-155">status/errorCode</span></span>|<span data-ttu-id="fb1c1-156">eq</span><span class="sxs-lookup"><span data-stu-id="fb1c1-156">eq</span></span>|
|<span data-ttu-id="fb1c1-157">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="fb1c1-157">initiatedBy/user/id</span></span>|<span data-ttu-id="fb1c1-158">eq</span><span class="sxs-lookup"><span data-stu-id="fb1c1-158">eq</span></span>|
|<span data-ttu-id="fb1c1-159">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="fb1c1-159">initiatedBy/user/displayName</span></span>| <span data-ttu-id="fb1c1-160">eq</span><span class="sxs-lookup"><span data-stu-id="fb1c1-160">eq</span></span>|
|<span data-ttu-id="fb1c1-161">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fb1c1-161">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="fb1c1-162">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="fb1c1-162">eq, startswith</span></span>|
|<span data-ttu-id="fb1c1-163">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="fb1c1-163">clientAppUsed</span></span>| <span data-ttu-id="fb1c1-164">eq</span><span class="sxs-lookup"><span data-stu-id="fb1c1-164">eq</span></span>|
|<span data-ttu-id="fb1c1-165">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="fb1c1-165">conditionalAccessStatus</span></span> | <span data-ttu-id="fb1c1-166">eq</span><span class="sxs-lookup"><span data-stu-id="fb1c1-166">eq</span></span>|
|<span data-ttu-id="fb1c1-167">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="fb1c1-167">deviceDetail/browser</span></span>| <span data-ttu-id="fb1c1-168">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="fb1c1-168">eq, startswith</span></span>|
|<span data-ttu-id="fb1c1-169">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="fb1c1-169">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="fb1c1-170">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="fb1c1-170">eq, startswith</span></span>|
|<span data-ttu-id="fb1c1-171">correlationId</span><span class="sxs-lookup"><span data-stu-id="fb1c1-171">correlationId</span></span>| <span data-ttu-id="fb1c1-172">eq</span><span class="sxs-lookup"><span data-stu-id="fb1c1-172">eq</span></span>|
|<span data-ttu-id="fb1c1-173">isRisky</span><span class="sxs-lookup"><span data-stu-id="fb1c1-173">isRisky</span></span>| <span data-ttu-id="fb1c1-174">eq</span><span class="sxs-lookup"><span data-stu-id="fb1c1-174">eq</span></span>|

## <a name="response"></a><span data-ttu-id="fb1c1-175">响应</span><span class="sxs-lookup"><span data-stu-id="fb1c1-175">Response</span></span>

<span data-ttu-id="fb1c1-176">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-176">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb1c1-177">示例</span><span class="sxs-lookup"><span data-stu-id="fb1c1-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb1c1-178">请求</span><span class="sxs-lookup"><span data-stu-id="fb1c1-178">Request</span></span>

<span data-ttu-id="fb1c1-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-179">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fb1c1-180">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fb1c1-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fb1c1-181">C#</span><span class="sxs-lookup"><span data-stu-id="fb1c1-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb1c1-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb1c1-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fb1c1-183">目标-C</span><span class="sxs-lookup"><span data-stu-id="fb1c1-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fb1c1-184">Java</span><span class="sxs-lookup"><span data-stu-id="fb1c1-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fb1c1-185">响应</span><span class="sxs-lookup"><span data-stu-id="fb1c1-185">Response</span></span>

<span data-ttu-id="fb1c1-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-186">Here is an example of the response.</span></span>
><span data-ttu-id="fb1c1-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fb1c1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}-->
