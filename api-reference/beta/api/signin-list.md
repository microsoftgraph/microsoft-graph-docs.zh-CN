---
title: 列出 signIn
doc_type: apiPageType
description: 获取 Azure Active Directory 租户中的用户登录列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5fa97184a4858d3b8fee7b537310cc09270a749b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938363"
---
# <a name="list-signins"></a><span data-ttu-id="c7a1b-103">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="c7a1b-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7a1b-104">获取[登录](../resources/signin.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-104">Get a list of [signIn](../resources/signin.md) objects.</span></span> <span data-ttu-id="c7a1b-105">此列表包含 Azure Active Directory 租户的用户登录。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-105">The list contains the user sign-ins for your Azure Active Directory tenant.</span></span> <span data-ttu-id="c7a1b-106">登录，其中用户名和密码作为授权令牌的一部分进行传递，并且成功的联合登录当前包含在登录日志中。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-106">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="c7a1b-107">最新的登录首先返回。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-107">The most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7a1b-108">权限</span><span class="sxs-lookup"><span data-stu-id="c7a1b-108">Permissions</span></span>

<span data-ttu-id="c7a1b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7a1b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7a1b-111">Permission type</span></span> | <span data-ttu-id="c7a1b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7a1b-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="c7a1b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7a1b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c7a1b-114">AuditLog、目录、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="c7a1b-114">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="c7a1b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7a1b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7a1b-116">不支持</span><span class="sxs-lookup"><span data-stu-id="c7a1b-116">Not supported</span></span> |
| <span data-ttu-id="c7a1b-117">Application</span><span class="sxs-lookup"><span data-stu-id="c7a1b-117">Application</span></span> | <span data-ttu-id="c7a1b-118">AuditLog、目录、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="c7a1b-118">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="c7a1b-119">此外，还必须将应用正确注册到 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-119">In addition, apps must be properly registered to Azure Active Directory.</span></span>

## <a name="http-request"></a><span data-ttu-id="c7a1b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7a1b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7a1b-121">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="c7a1b-121">Optional query parameters</span></span>

<span data-ttu-id="c7a1b-122">此方法支持以下 OData 查询参数，它们有助于自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-122">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="c7a1b-123">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-123">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

| <span data-ttu-id="c7a1b-124">名称</span><span class="sxs-lookup"><span data-stu-id="c7a1b-124">Name</span></span> | <span data-ttu-id="c7a1b-125">说明</span><span class="sxs-lookup"><span data-stu-id="c7a1b-125">Description</span></span> | <span data-ttu-id="c7a1b-126">示例</span><span class="sxs-lookup"><span data-stu-id="c7a1b-126">Example</span></span> |
|:---- |:----------- |:------- |
| [<span data-ttu-id="c7a1b-127">$filter</span><span class="sxs-lookup"><span data-stu-id="c7a1b-127">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)| <span data-ttu-id="c7a1b-128">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-128">Filters results (rows).</span></span> | `/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24` |
| [<span data-ttu-id="c7a1b-129">$top</span><span class="sxs-lookup"><span data-stu-id="c7a1b-129">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter) | <span data-ttu-id="c7a1b-130">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-130">Sets the page size of results.</span></span> | `/auditLogs/signIns?$top=1` |
| [<span data-ttu-id="c7a1b-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="c7a1b-131">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter) | <span data-ttu-id="c7a1b-132">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-132">Retrieves the next page of results from result sets that span multiple pages.</span></span> |`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="c7a1b-133">$filter 参数支持的属性</span><span class="sxs-lookup"><span data-stu-id="c7a1b-133">Attributes supported by $filter parameter</span></span>

| <span data-ttu-id="c7a1b-134">属性名</span><span class="sxs-lookup"><span data-stu-id="c7a1b-134">Attribute Name</span></span> | <span data-ttu-id="c7a1b-135">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="c7a1b-135">Supported operators</span></span> |
|:-------------- |:------------------- |
| <span data-ttu-id="c7a1b-136">id</span><span class="sxs-lookup"><span data-stu-id="c7a1b-136">id</span></span> | <span data-ttu-id="c7a1b-137">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-137">eq</span></span> |
| <span data-ttu-id="c7a1b-138">userId</span><span class="sxs-lookup"><span data-stu-id="c7a1b-138">userId</span></span> | <span data-ttu-id="c7a1b-139">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-139">eq</span></span> |
| <span data-ttu-id="c7a1b-140">appId</span><span class="sxs-lookup"><span data-stu-id="c7a1b-140">appId</span></span> | <span data-ttu-id="c7a1b-141">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-141">eq</span></span> |
| <span data-ttu-id="c7a1b-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7a1b-142">createdDateTime</span></span> | <span data-ttu-id="c7a1b-143">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="c7a1b-143">eq, le, ge</span></span> |
| <span data-ttu-id="c7a1b-144">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c7a1b-144">userDisplayName</span></span> | <span data-ttu-id="c7a1b-145">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-145">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c7a1b-146">userPrincipalName</span></span> | <span data-ttu-id="c7a1b-147">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-147">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="c7a1b-148">appDisplayName</span></span> | <span data-ttu-id="c7a1b-149">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-149">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-150">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c7a1b-150">ipAddress</span></span> | <span data-ttu-id="c7a1b-151">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-151">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-152">location/city</span><span class="sxs-lookup"><span data-stu-id="c7a1b-152">location/city</span></span> | <span data-ttu-id="c7a1b-153">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-153">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-154">location/state</span><span class="sxs-lookup"><span data-stu-id="c7a1b-154">location/state</span></span> | <span data-ttu-id="c7a1b-155">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-155">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-156">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="c7a1b-156">location/countryOrRegion</span></span> | <span data-ttu-id="c7a1b-157">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-157">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-158">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="c7a1b-158">status/errorCode</span></span> | <span data-ttu-id="c7a1b-159">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-159">eq</span></span> |
| <span data-ttu-id="c7a1b-160">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="c7a1b-160">initiatedBy/user/id</span></span> | <span data-ttu-id="c7a1b-161">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-161">eq</span></span> |
| <span data-ttu-id="c7a1b-162">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="c7a1b-162">initiatedBy/user/displayName</span></span> | <span data-ttu-id="c7a1b-163">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-163">eq</span></span> |
| <span data-ttu-id="c7a1b-164">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c7a1b-164">initiatedBy/user/userPrincipalName</span></span> | <span data-ttu-id="c7a1b-165">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-165">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-166">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="c7a1b-166">clientAppUsed</span></span> | <span data-ttu-id="c7a1b-167">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-167">eq</span></span> |
| <span data-ttu-id="c7a1b-168">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="c7a1b-168">conditionalAccessStatus</span></span> | <span data-ttu-id="c7a1b-169">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-169">eq</span></span> |
| <span data-ttu-id="c7a1b-170">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="c7a1b-170">deviceDetail/browser</span></span> | <span data-ttu-id="c7a1b-171">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-171">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-172">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c7a1b-172">deviceDetail/operatingSystem</span></span> | <span data-ttu-id="c7a1b-173">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-173">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-174">correlationId</span><span class="sxs-lookup"><span data-stu-id="c7a1b-174">correlationId</span></span> | <span data-ttu-id="c7a1b-175">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-175">eq</span></span> |
| <span data-ttu-id="c7a1b-176">riskDetail</span><span class="sxs-lookup"><span data-stu-id="c7a1b-176">riskDetail</span></span> | <span data-ttu-id="c7a1b-177">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-177">eq</span></span> |
| <span data-ttu-id="c7a1b-178">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="c7a1b-178">riskLevelAggregated</span></span> | <span data-ttu-id="c7a1b-179">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-179">eq</span></span> |
| <span data-ttu-id="c7a1b-180">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="c7a1b-180">riskLevelDuringSignIn</span></span> | <span data-ttu-id="c7a1b-181">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-181">eq</span></span> |
| <span data-ttu-id="c7a1b-182">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="c7a1b-182">riskEventTypes</span></span> | <span data-ttu-id="c7a1b-183">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-183">eq</span></span> |
| <span data-ttu-id="c7a1b-184">riskState</span><span class="sxs-lookup"><span data-stu-id="c7a1b-184">riskState</span></span> | <span data-ttu-id="c7a1b-185">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-185">eq</span></span> |
| <span data-ttu-id="c7a1b-186">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="c7a1b-186">originalRequestId</span></span> | <span data-ttu-id="c7a1b-187">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-187">eq</span></span> |
| <span data-ttu-id="c7a1b-188">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="c7a1b-188">tokenIssuerName</span></span> | <span data-ttu-id="c7a1b-189">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-189">eq</span></span> |
| <span data-ttu-id="c7a1b-190">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="c7a1b-190">tokenIssuerType</span></span> | <span data-ttu-id="c7a1b-191">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-191">eq</span></span> |
| <span data-ttu-id="c7a1b-192">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c7a1b-192">resourceDisplayName</span></span> | <span data-ttu-id="c7a1b-193">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-193">eq</span></span> |
| <span data-ttu-id="c7a1b-194">resourceId</span><span class="sxs-lookup"><span data-stu-id="c7a1b-194">resourceId</span></span> | <span data-ttu-id="c7a1b-195">eq</span><span class="sxs-lookup"><span data-stu-id="c7a1b-195">eq</span></span> |
| <span data-ttu-id="c7a1b-196">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="c7a1b-196">servicePrincipalId</span></span> | <span data-ttu-id="c7a1b-197">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-197">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-198">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="c7a1b-198">servicePrincipalName</span></span> | <span data-ttu-id="c7a1b-199">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-199">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-200">userAgent</span><span class="sxs-lookup"><span data-stu-id="c7a1b-200">userAgent</span></span> | <span data-ttu-id="c7a1b-201">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-201">eq, startswith</span></span> |
| <span data-ttu-id="c7a1b-202">alternateSignInName</span><span class="sxs-lookup"><span data-stu-id="c7a1b-202">alternateSignInName</span></span> | <span data-ttu-id="c7a1b-203">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="c7a1b-203">eq, startswith</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c7a1b-204">请求头</span><span class="sxs-lookup"><span data-stu-id="c7a1b-204">Request headers</span></span>

| <span data-ttu-id="c7a1b-205">名称</span><span class="sxs-lookup"><span data-stu-id="c7a1b-205">Name</span></span>      |<span data-ttu-id="c7a1b-206">说明</span><span class="sxs-lookup"><span data-stu-id="c7a1b-206">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7a1b-207">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7a1b-207">Authorization</span></span> | <span data-ttu-id="c7a1b-208">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="c7a1b-208">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7a1b-209">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7a1b-209">Request body</span></span>

<span data-ttu-id="c7a1b-210">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-210">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7a1b-211">响应</span><span class="sxs-lookup"><span data-stu-id="c7a1b-211">Response</span></span>

<span data-ttu-id="c7a1b-212">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-212">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7a1b-213">示例</span><span class="sxs-lookup"><span data-stu-id="c7a1b-213">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="c7a1b-214">示例1：用户使用 MFA 登录，这是由条件访问策略触发的。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-214">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="c7a1b-215">主要身份验证是通过 FIDO。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-215">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="c7a1b-216">请求</span><span class="sxs-lookup"><span data-stu-id="c7a1b-216">Request</span></span>

<span data-ttu-id="c7a1b-217">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-217">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c7a1b-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7a1b-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c7a1b-219">C#</span><span class="sxs-lookup"><span data-stu-id="c7a1b-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7a1b-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7a1b-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c7a1b-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7a1b-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c7a1b-222">响应</span><span class="sxs-lookup"><span data-stu-id="c7a1b-222">Response</span></span>

<span data-ttu-id="c7a1b-223">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-223">The following is an example of the response.</span></span>

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
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
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
          "result":"applied"
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
### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="c7a1b-224">示例2：用户仅使用主身份验证进行登录。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-224">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="c7a1b-225">主要身份验证通过云密码。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-225">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="c7a1b-226">请求</span><span class="sxs-lookup"><span data-stu-id="c7a1b-226">Request</span></span>

<span data-ttu-id="c7a1b-227">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-227">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```

#### <a name="response"></a><span data-ttu-id="c7a1b-228">响应</span><span class="sxs-lookup"><span data-stu-id="c7a1b-228">Response</span></span>

<span data-ttu-id="c7a1b-229">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c7a1b-229">The following is an example of the response.</span></span>

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
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
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