---
title: 列出 signIn
doc_type: apiPageType
description: 获取 Azure Active Directory 租户中的用户登录列表。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: d850fdf92f88c2c6cd3290dfe9479df8e09834be
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132130"
---
# <a name="list-signins"></a><span data-ttu-id="617d2-103">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="617d2-103">List signIns</span></span>

<span data-ttu-id="617d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="617d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="617d2-105">获取 [signIn 对象](../resources/signin.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="617d2-105">Get a list of [signIn](../resources/signin.md) objects.</span></span> <span data-ttu-id="617d2-106">该列表包含 Azure Active Directory 租户的用户登录。</span><span class="sxs-lookup"><span data-stu-id="617d2-106">The list contains the user sign-ins for your Azure Active Directory tenant.</span></span> <span data-ttu-id="617d2-107">用户名和密码作为授权令牌的一部分传递的登录，并且成功的联合登录当前包含在登录日志中。</span><span class="sxs-lookup"><span data-stu-id="617d2-107">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="617d2-108">首先返回最近的登录。</span><span class="sxs-lookup"><span data-stu-id="617d2-108">The most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="617d2-109">权限</span><span class="sxs-lookup"><span data-stu-id="617d2-109">Permissions</span></span>

<span data-ttu-id="617d2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="617d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="617d2-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="617d2-112">Permission type</span></span> | <span data-ttu-id="617d2-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="617d2-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="617d2-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="617d2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="617d2-115">AuditLog.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="617d2-115">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="617d2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="617d2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="617d2-117">不支持</span><span class="sxs-lookup"><span data-stu-id="617d2-117">Not supported</span></span> |
| <span data-ttu-id="617d2-118">Application</span><span class="sxs-lookup"><span data-stu-id="617d2-118">Application</span></span> | <span data-ttu-id="617d2-119">AuditLog.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="617d2-119">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="617d2-120">此外，应用必须正确注册到 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="617d2-120">In addition, apps must be properly registered to Azure Active Directory.</span></span>

## <a name="http-request"></a><span data-ttu-id="617d2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="617d2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="617d2-122">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="617d2-122">Optional query parameters</span></span>

<span data-ttu-id="617d2-123">此方法支持以下 OData 查询参数，它们有助于自定义响应。</span><span class="sxs-lookup"><span data-stu-id="617d2-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="617d2-124">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="617d2-124">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

| <span data-ttu-id="617d2-125">名称</span><span class="sxs-lookup"><span data-stu-id="617d2-125">Name</span></span> | <span data-ttu-id="617d2-126">说明</span><span class="sxs-lookup"><span data-stu-id="617d2-126">Description</span></span> | <span data-ttu-id="617d2-127">示例</span><span class="sxs-lookup"><span data-stu-id="617d2-127">Example</span></span> |
|:---- |:----------- |:------- |
| [<span data-ttu-id="617d2-128">$filter</span><span class="sxs-lookup"><span data-stu-id="617d2-128">$filter</span></span>](/graph/query-parameters#filter-parameter)| <span data-ttu-id="617d2-129">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="617d2-129">Filters results (rows).</span></span> | `/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24` |
| [<span data-ttu-id="617d2-130">$top</span><span class="sxs-lookup"><span data-stu-id="617d2-130">$top</span></span>](/graph/query-parameters#top-parameter) | <span data-ttu-id="617d2-131">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="617d2-131">Sets the page size of results.</span></span> | `/auditLogs/signIns?$top=1` |
| [<span data-ttu-id="617d2-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="617d2-132">$skiptoken</span></span>](/graph/query-parameters#skiptoken-parameter) | <span data-ttu-id="617d2-133">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="617d2-133">Retrieves the next page of results from result sets that span multiple pages.</span></span> |`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="617d2-134">$filter参数支持的属性</span><span class="sxs-lookup"><span data-stu-id="617d2-134">Attributes supported by $filter parameter</span></span>

| <span data-ttu-id="617d2-135">属性名</span><span class="sxs-lookup"><span data-stu-id="617d2-135">Attribute Name</span></span> | <span data-ttu-id="617d2-136">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="617d2-136">Supported operators</span></span> |
|:-------------- |:------------------- |
| <span data-ttu-id="617d2-137">id</span><span class="sxs-lookup"><span data-stu-id="617d2-137">id</span></span> | <span data-ttu-id="617d2-138">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-138">eq</span></span> |
| <span data-ttu-id="617d2-139">userId</span><span class="sxs-lookup"><span data-stu-id="617d2-139">userId</span></span> | <span data-ttu-id="617d2-140">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-140">eq</span></span> |
| <span data-ttu-id="617d2-141">appId</span><span class="sxs-lookup"><span data-stu-id="617d2-141">appId</span></span> | <span data-ttu-id="617d2-142">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-142">eq</span></span> |
| <span data-ttu-id="617d2-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="617d2-143">createdDateTime</span></span> | <span data-ttu-id="617d2-144">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="617d2-144">eq, le, ge</span></span> |
| <span data-ttu-id="617d2-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="617d2-145">userDisplayName</span></span> | <span data-ttu-id="617d2-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-146">eq, startswith</span></span> |
| <span data-ttu-id="617d2-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="617d2-147">userPrincipalName</span></span> | <span data-ttu-id="617d2-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-148">eq, startswith</span></span> |
| <span data-ttu-id="617d2-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="617d2-149">appDisplayName</span></span> | <span data-ttu-id="617d2-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-150">eq, startswith</span></span> |
| <span data-ttu-id="617d2-151">authenticationRequirement</span><span class="sxs-lookup"><span data-stu-id="617d2-151">authenticationRequirement</span></span> |<span data-ttu-id="617d2-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-152">eq, startswith</span></span> |
| <span data-ttu-id="617d2-153">ipAddress</span><span class="sxs-lookup"><span data-stu-id="617d2-153">ipAddress</span></span> | <span data-ttu-id="617d2-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-154">eq, startswith</span></span> |
| <span data-ttu-id="617d2-155">location/city</span><span class="sxs-lookup"><span data-stu-id="617d2-155">location/city</span></span> | <span data-ttu-id="617d2-156">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-156">eq, startswith</span></span> |
| <span data-ttu-id="617d2-157">location/state</span><span class="sxs-lookup"><span data-stu-id="617d2-157">location/state</span></span> | <span data-ttu-id="617d2-158">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-158">eq, startswith</span></span> |
| <span data-ttu-id="617d2-159">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="617d2-159">location/countryOrRegion</span></span> | <span data-ttu-id="617d2-160">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-160">eq, startswith</span></span> |
| <span data-ttu-id="617d2-161">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="617d2-161">status/errorCode</span></span> | <span data-ttu-id="617d2-162">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-162">eq</span></span> |
| <span data-ttu-id="617d2-163">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="617d2-163">initiatedBy/user/id</span></span> | <span data-ttu-id="617d2-164">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-164">eq</span></span> |
| <span data-ttu-id="617d2-165">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="617d2-165">initiatedBy/user/displayName</span></span> | <span data-ttu-id="617d2-166">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-166">eq</span></span> |
| <span data-ttu-id="617d2-167">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="617d2-167">initiatedBy/user/userPrincipalName</span></span> | <span data-ttu-id="617d2-168">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-168">eq, startswith</span></span> |
| <span data-ttu-id="617d2-169">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="617d2-169">clientAppUsed</span></span> | <span data-ttu-id="617d2-170">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-170">eq</span></span> |
| <span data-ttu-id="617d2-171">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="617d2-171">conditionalAccessStatus</span></span> | <span data-ttu-id="617d2-172">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-172">eq</span></span> |
| <span data-ttu-id="617d2-173">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="617d2-173">deviceDetail/browser</span></span> | <span data-ttu-id="617d2-174">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-174">eq, startswith</span></span> |
| <span data-ttu-id="617d2-175">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="617d2-175">deviceDetail/operatingSystem</span></span> | <span data-ttu-id="617d2-176">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-176">eq, startswith</span></span> |
| <span data-ttu-id="617d2-177">correlationId</span><span class="sxs-lookup"><span data-stu-id="617d2-177">correlationId</span></span> | <span data-ttu-id="617d2-178">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-178">eq</span></span> |
| <span data-ttu-id="617d2-179">riskDetail</span><span class="sxs-lookup"><span data-stu-id="617d2-179">riskDetail</span></span> | <span data-ttu-id="617d2-180">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-180">eq</span></span> |
| <span data-ttu-id="617d2-181">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="617d2-181">riskLevelAggregated</span></span> | <span data-ttu-id="617d2-182">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-182">eq</span></span> |
| <span data-ttu-id="617d2-183">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="617d2-183">riskLevelDuringSignIn</span></span> | <span data-ttu-id="617d2-184">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-184">eq</span></span> |
| <span data-ttu-id="617d2-185">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="617d2-185">riskEventTypes</span></span> | <span data-ttu-id="617d2-186">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-186">eq</span></span> |
| <span data-ttu-id="617d2-187">riskEventTypes_v2</span><span class="sxs-lookup"><span data-stu-id="617d2-187">riskEventTypes_v2</span></span> | <span data-ttu-id="617d2-188">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-188">eq, startswith</span></span> |
| <span data-ttu-id="617d2-189">riskState</span><span class="sxs-lookup"><span data-stu-id="617d2-189">riskState</span></span> | <span data-ttu-id="617d2-190">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-190">eq</span></span> |
| <span data-ttu-id="617d2-191">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="617d2-191">originalRequestId</span></span> | <span data-ttu-id="617d2-192">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-192">eq</span></span> |
| <span data-ttu-id="617d2-193">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="617d2-193">tokenIssuerName</span></span> | <span data-ttu-id="617d2-194">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-194">eq</span></span> |
| <span data-ttu-id="617d2-195">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="617d2-195">tokenIssuerType</span></span> | <span data-ttu-id="617d2-196">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-196">eq</span></span> |
| <span data-ttu-id="617d2-197">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="617d2-197">resourceDisplayName</span></span> | <span data-ttu-id="617d2-198">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-198">eq</span></span> |
| <span data-ttu-id="617d2-199">resourceId</span><span class="sxs-lookup"><span data-stu-id="617d2-199">resourceId</span></span> | <span data-ttu-id="617d2-200">eq</span><span class="sxs-lookup"><span data-stu-id="617d2-200">eq</span></span> |
| <span data-ttu-id="617d2-201">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="617d2-201">servicePrincipalId</span></span> | <span data-ttu-id="617d2-202">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-202">eq, startswith</span></span> |
| <span data-ttu-id="617d2-203">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="617d2-203">servicePrincipalName</span></span> | <span data-ttu-id="617d2-204">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-204">eq, startswith</span></span> |
| <span data-ttu-id="617d2-205">userAgent</span><span class="sxs-lookup"><span data-stu-id="617d2-205">userAgent</span></span> | <span data-ttu-id="617d2-206">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-206">eq, startswith</span></span> |
| <span data-ttu-id="617d2-207">alternateSignInName</span><span class="sxs-lookup"><span data-stu-id="617d2-207">alternateSignInName</span></span> | <span data-ttu-id="617d2-208">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="617d2-208">eq, startswith</span></span> |

## <a name="request-headers"></a><span data-ttu-id="617d2-209">请求头</span><span class="sxs-lookup"><span data-stu-id="617d2-209">Request headers</span></span>

| <span data-ttu-id="617d2-210">名称</span><span class="sxs-lookup"><span data-stu-id="617d2-210">Name</span></span>      |<span data-ttu-id="617d2-211">说明</span><span class="sxs-lookup"><span data-stu-id="617d2-211">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="617d2-212">Authorization</span><span class="sxs-lookup"><span data-stu-id="617d2-212">Authorization</span></span> | <span data-ttu-id="617d2-213">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="617d2-213">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="617d2-214">请求正文</span><span class="sxs-lookup"><span data-stu-id="617d2-214">Request body</span></span>

<span data-ttu-id="617d2-215">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="617d2-215">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="617d2-216">响应</span><span class="sxs-lookup"><span data-stu-id="617d2-216">Response</span></span>

<span data-ttu-id="617d2-217">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="617d2-217">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="617d2-218">示例</span><span class="sxs-lookup"><span data-stu-id="617d2-218">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="617d2-219">示例 1：用户使用由条件访问策略触发的 MFA 登录。</span><span class="sxs-lookup"><span data-stu-id="617d2-219">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="617d2-220">主身份验证通过 FIDO 进行。</span><span class="sxs-lookup"><span data-stu-id="617d2-220">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="617d2-221">请求</span><span class="sxs-lookup"><span data-stu-id="617d2-221">Request</span></span>

<span data-ttu-id="617d2-222">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="617d2-222">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="617d2-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="617d2-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="617d2-224">C#</span><span class="sxs-lookup"><span data-stu-id="617d2-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="617d2-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="617d2-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="617d2-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="617d2-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="617d2-227">Java</span><span class="sxs-lookup"><span data-stu-id="617d2-227">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="617d2-228">响应</span><span class="sxs-lookup"><span data-stu-id="617d2-228">Response</span></span>

<span data-ttu-id="617d2-229">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="617d2-229">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [
        {
            "id": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-1111-5555-b4e2-a37c6808512d",
            "appId": "de8bc8b5-5555-6666-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "authenticationRequirement": "multiFactorAuthentication",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Safari/537.36 Edg/80.0.361.66",
            "correlationId": "d79f5bee-blah-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "originalRequestId": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "isInteractive": true,
            "tokenIssuerName": "",
            "tokenIssuerType": "AzureAD",
            "processingTimeInMilliseconds": 541,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "riskEventTypes_v2": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
            "authenticationMethodsUsed": [],
            "alternateSignInName": "testaccount2.contoso.com",
            "servicePrincipalName": null,
            "servicePrincipalId": "",
            "mfaDetail": null,
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
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
               
            ],
            "authenticationProcessingDetails": [],
            "networkLocationDetails": [],
            "authenticationDetails": [
                    {
              "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
              "authenticationMethod":"FIDO2",
              "authenticationMethodDetail":"1G54395783",
              "succeeded":true,
              "authenticationStepResultDetail":"methodSucceeded",
              "authenticationStepRequirement":"Primary authentication"
            },
            {
              "authenticationStepDateTime":"2018-11-06T18:48:12.94725647Z",
              "authenticationMethod":"Claim in access token",
              "authenticationMethodDetail":null,
              "succeeded":true,
              "authenticationStepResultDetail":"methodSucceeded",
              "authenticationStepRequirement":"MFA"
            }
            ],
            "authenticationRequirementPolicies": []
        }
    ]
}
```
### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="617d2-230">示例 2：用户仅使用主身份验证登录。</span><span class="sxs-lookup"><span data-stu-id="617d2-230">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="617d2-231">主身份验证通过云密码进行。</span><span class="sxs-lookup"><span data-stu-id="617d2-231">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="617d2-232">请求</span><span class="sxs-lookup"><span data-stu-id="617d2-232">Request</span></span>

<span data-ttu-id="617d2-233">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="617d2-233">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="617d2-234">HTTP</span><span class="sxs-lookup"><span data-stu-id="617d2-234">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="617d2-235">C#</span><span class="sxs-lookup"><span data-stu-id="617d2-235">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="617d2-236">JavaScript</span><span class="sxs-lookup"><span data-stu-id="617d2-236">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="617d2-237">Objective-C</span><span class="sxs-lookup"><span data-stu-id="617d2-237">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="617d2-238">Java</span><span class="sxs-lookup"><span data-stu-id="617d2-238">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="617d2-239">响应</span><span class="sxs-lookup"><span data-stu-id="617d2-239">Response</span></span>

<span data-ttu-id="617d2-240">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="617d2-240">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
       "authenticationRequirement": "singleFactorAuthentication",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [ 
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"Password",
          "authenticationMethodDetail":"Cloud password",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"notApplied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```
