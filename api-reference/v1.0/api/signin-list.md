---
title: 列出 signIn
description: 介绍 Microsoft Graph API 中登录资源 (实体) 的列表方法。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b628abb986e04a137fb2fa50fe27d39a9390d580
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891590"
---
# <a name="list-signins"></a><span data-ttu-id="0afaa-103">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="0afaa-103">List signIns</span></span>

<span data-ttu-id="0afaa-104">检索租户的 Azure AD 用户登录信息。</span><span class="sxs-lookup"><span data-stu-id="0afaa-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="0afaa-105">在性质 (用户名/密码作为身份验证令牌的一部分传递) 和成功的联合登录中当前包括在登录日志中的登录登录。</span><span class="sxs-lookup"><span data-stu-id="0afaa-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="0afaa-106">权限</span><span class="sxs-lookup"><span data-stu-id="0afaa-106">Permissions</span></span>

<span data-ttu-id="0afaa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="0afaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="0afaa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0afaa-109">Permission type</span></span>      | <span data-ttu-id="0afaa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0afaa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0afaa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0afaa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0afaa-112">AuditLog 和所有目录。全部读取. 所有</span><span class="sxs-lookup"><span data-stu-id="0afaa-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="0afaa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0afaa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0afaa-114">不支持</span><span class="sxs-lookup"><span data-stu-id="0afaa-114">Not supported</span></span>   |
|<span data-ttu-id="0afaa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0afaa-115">Application</span></span> | <span data-ttu-id="0afaa-116">AuditLog 和所有目录。全部读取. 所有</span><span class="sxs-lookup"><span data-stu-id="0afaa-116">AuditLog.Read.All and Directory.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0afaa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0afaa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0afaa-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0afaa-118">Optional query parameters</span></span>

<span data-ttu-id="0afaa-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0afaa-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="0afaa-120">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="0afaa-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="0afaa-121">名称</span><span class="sxs-lookup"><span data-stu-id="0afaa-121">Name</span></span>     |<span data-ttu-id="0afaa-122">说明</span><span class="sxs-lookup"><span data-stu-id="0afaa-122">Description</span></span>                            |<span data-ttu-id="0afaa-123">示例</span><span class="sxs-lookup"><span data-stu-id="0afaa-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="0afaa-124">$filter</span><span class="sxs-lookup"><span data-stu-id="0afaa-124">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="0afaa-125">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="0afaa-125">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="0afaa-126">$top</span><span class="sxs-lookup"><span data-stu-id="0afaa-126">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="0afaa-127">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="0afaa-127">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="0afaa-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="0afaa-128">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="0afaa-129">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="0afaa-129">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="0afaa-130">$Filter 参数支持的属性</span><span class="sxs-lookup"><span data-stu-id="0afaa-130">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="0afaa-131">属性名</span><span class="sxs-lookup"><span data-stu-id="0afaa-131">Attribute name</span></span> |<span data-ttu-id="0afaa-132">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="0afaa-132">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="0afaa-133">id</span><span class="sxs-lookup"><span data-stu-id="0afaa-133">id</span></span>|<span data-ttu-id="0afaa-134">eq</span><span class="sxs-lookup"><span data-stu-id="0afaa-134">eq</span></span>|
|<span data-ttu-id="0afaa-135">userId</span><span class="sxs-lookup"><span data-stu-id="0afaa-135">userId</span></span>|<span data-ttu-id="0afaa-136">eq</span><span class="sxs-lookup"><span data-stu-id="0afaa-136">eq</span></span>|
|<span data-ttu-id="0afaa-137">appId</span><span class="sxs-lookup"><span data-stu-id="0afaa-137">appId</span></span>|<span data-ttu-id="0afaa-138">eq</span><span class="sxs-lookup"><span data-stu-id="0afaa-138">eq</span></span>|
|<span data-ttu-id="0afaa-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0afaa-139">createdDateTime</span></span>| <span data-ttu-id="0afaa-140">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="0afaa-140">eq, le, ge</span></span>|
|<span data-ttu-id="0afaa-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0afaa-141">userDisplayName</span></span>| <span data-ttu-id="0afaa-142">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="0afaa-142">eq, startswith</span></span>|
|<span data-ttu-id="0afaa-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0afaa-143">userPrincipalName</span></span>| <span data-ttu-id="0afaa-144">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="0afaa-144">eq, startswith</span></span>|
|<span data-ttu-id="0afaa-145">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="0afaa-145">appDisplayName</span></span>| <span data-ttu-id="0afaa-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="0afaa-146">eq, startswith</span></span>|
|<span data-ttu-id="0afaa-147">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0afaa-147">ipAddress</span></span>| <span data-ttu-id="0afaa-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="0afaa-148">eq, startswith</span></span>|
|<span data-ttu-id="0afaa-149">location/city</span><span class="sxs-lookup"><span data-stu-id="0afaa-149">location/city</span></span>| <span data-ttu-id="0afaa-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="0afaa-150">eq, startswith</span></span>|
|<span data-ttu-id="0afaa-151">location/state</span><span class="sxs-lookup"><span data-stu-id="0afaa-151">location/state</span></span>| <span data-ttu-id="0afaa-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="0afaa-152">eq, startswith</span></span>|
|<span data-ttu-id="0afaa-153">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="0afaa-153">location/countryOrRegion</span></span>| <span data-ttu-id="0afaa-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="0afaa-154">eq, startswith</span></span>|
|<span data-ttu-id="0afaa-155">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="0afaa-155">status/errorCode</span></span>|<span data-ttu-id="0afaa-156">eq</span><span class="sxs-lookup"><span data-stu-id="0afaa-156">eq</span></span>|
|<span data-ttu-id="0afaa-157">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="0afaa-157">initiatedBy/user/id</span></span>|<span data-ttu-id="0afaa-158">eq</span><span class="sxs-lookup"><span data-stu-id="0afaa-158">eq</span></span>|
|<span data-ttu-id="0afaa-159">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="0afaa-159">initiatedBy/user/displayName</span></span>| <span data-ttu-id="0afaa-160">eq</span><span class="sxs-lookup"><span data-stu-id="0afaa-160">eq</span></span>|
|<span data-ttu-id="0afaa-161">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0afaa-161">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="0afaa-162">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="0afaa-162">eq, startswith</span></span>|
|<span data-ttu-id="0afaa-163">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="0afaa-163">clientAppUsed</span></span>| <span data-ttu-id="0afaa-164">eq</span><span class="sxs-lookup"><span data-stu-id="0afaa-164">eq</span></span>|
|<span data-ttu-id="0afaa-165">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="0afaa-165">conditionalAccessStatus</span></span> | <span data-ttu-id="0afaa-166">eq</span><span class="sxs-lookup"><span data-stu-id="0afaa-166">eq</span></span>|
|<span data-ttu-id="0afaa-167">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="0afaa-167">deviceDetail/browser</span></span>| <span data-ttu-id="0afaa-168">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="0afaa-168">eq, startswith</span></span>|
|<span data-ttu-id="0afaa-169">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0afaa-169">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="0afaa-170">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="0afaa-170">eq, startswith</span></span>|
|<span data-ttu-id="0afaa-171">correlationId</span><span class="sxs-lookup"><span data-stu-id="0afaa-171">correlationId</span></span>| <span data-ttu-id="0afaa-172">eq</span><span class="sxs-lookup"><span data-stu-id="0afaa-172">eq</span></span>|
|<span data-ttu-id="0afaa-173">isRisky</span><span class="sxs-lookup"><span data-stu-id="0afaa-173">isRisky</span></span>| <span data-ttu-id="0afaa-174">eq</span><span class="sxs-lookup"><span data-stu-id="0afaa-174">eq</span></span>|

## <a name="response"></a><span data-ttu-id="0afaa-175">响应</span><span class="sxs-lookup"><span data-stu-id="0afaa-175">Response</span></span>

<span data-ttu-id="0afaa-176">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0afaa-176">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0afaa-177">示例</span><span class="sxs-lookup"><span data-stu-id="0afaa-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="0afaa-178">请求</span><span class="sxs-lookup"><span data-stu-id="0afaa-178">Request</span></span>

<span data-ttu-id="0afaa-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0afaa-179">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0afaa-180">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0afaa-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0afaa-181">C#</span><span class="sxs-lookup"><span data-stu-id="0afaa-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0afaa-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="0afaa-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0afaa-183">目标-C</span><span class="sxs-lookup"><span data-stu-id="0afaa-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0afaa-184">Java</span><span class="sxs-lookup"><span data-stu-id="0afaa-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0afaa-185">响应</span><span class="sxs-lookup"><span data-stu-id="0afaa-185">Response</span></span>

<span data-ttu-id="0afaa-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0afaa-186">Here is an example of the response.</span></span>
><span data-ttu-id="0afaa-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0afaa-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
