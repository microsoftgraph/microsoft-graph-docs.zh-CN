---
title: 列出 signIn
doc_type: apiPageType
description: 获取 Azure Active Directory 租户中的用户登录列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 33b72a0361776a991f0f29675fced77379e3e215
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453266"
---
# <a name="list-signins"></a><span data-ttu-id="dd773-103">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="dd773-103">List signIns</span></span>

<span data-ttu-id="dd773-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dd773-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd773-105">获取[登录](../resources/signin.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="dd773-105">Get a list of [signIn](../resources/signin.md) objects.</span></span> <span data-ttu-id="dd773-106">此列表包含 Azure Active Directory 租户的用户登录。</span><span class="sxs-lookup"><span data-stu-id="dd773-106">The list contains the user sign-ins for your Azure Active Directory tenant.</span></span> <span data-ttu-id="dd773-107">登录，其中用户名和密码作为授权令牌的一部分进行传递，并且成功的联合登录当前包含在登录日志中。</span><span class="sxs-lookup"><span data-stu-id="dd773-107">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="dd773-108">最新的登录首先返回。</span><span class="sxs-lookup"><span data-stu-id="dd773-108">The most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd773-109">权限</span><span class="sxs-lookup"><span data-stu-id="dd773-109">Permissions</span></span>

<span data-ttu-id="dd773-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd773-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd773-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd773-112">Permission type</span></span> | <span data-ttu-id="dd773-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd773-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="dd773-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd773-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dd773-115">AuditLog、目录、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="dd773-115">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="dd773-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd773-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd773-117">不支持</span><span class="sxs-lookup"><span data-stu-id="dd773-117">Not supported</span></span> |
| <span data-ttu-id="dd773-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd773-118">Application</span></span> | <span data-ttu-id="dd773-119">AuditLog、目录、全部读取。所有</span><span class="sxs-lookup"><span data-stu-id="dd773-119">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="dd773-120">此外，还必须将应用正确注册到 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="dd773-120">In addition, apps must be properly registered to Azure Active Directory.</span></span>

## <a name="http-request"></a><span data-ttu-id="dd773-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd773-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd773-122">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="dd773-122">Optional query parameters</span></span>

<span data-ttu-id="dd773-123">此方法支持以下 OData 查询参数，它们有助于自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dd773-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="dd773-124">关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="dd773-124">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

| <span data-ttu-id="dd773-125">名称</span><span class="sxs-lookup"><span data-stu-id="dd773-125">Name</span></span> | <span data-ttu-id="dd773-126">说明</span><span class="sxs-lookup"><span data-stu-id="dd773-126">Description</span></span> | <span data-ttu-id="dd773-127">示例</span><span class="sxs-lookup"><span data-stu-id="dd773-127">Example</span></span> |
|:---- |:----------- |:------- |
| [<span data-ttu-id="dd773-128">$filter</span><span class="sxs-lookup"><span data-stu-id="dd773-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)| <span data-ttu-id="dd773-129">筛选结果（行）。</span><span class="sxs-lookup"><span data-stu-id="dd773-129">Filters results (rows).</span></span> | `/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24` |
| [<span data-ttu-id="dd773-130">$top</span><span class="sxs-lookup"><span data-stu-id="dd773-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter) | <span data-ttu-id="dd773-131">设置结果的页面大小。</span><span class="sxs-lookup"><span data-stu-id="dd773-131">Sets the page size of results.</span></span> | `/auditLogs/signIns?$top=1` |
| [<span data-ttu-id="dd773-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="dd773-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter) | <span data-ttu-id="dd773-133">从跨多页的结果集中检索下一页结果。</span><span class="sxs-lookup"><span data-stu-id="dd773-133">Retrieves the next page of results from result sets that span multiple pages.</span></span> |`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="dd773-134">$filter 参数支持的属性</span><span class="sxs-lookup"><span data-stu-id="dd773-134">Attributes supported by $filter parameter</span></span>

| <span data-ttu-id="dd773-135">属性名</span><span class="sxs-lookup"><span data-stu-id="dd773-135">Attribute Name</span></span> | <span data-ttu-id="dd773-136">支持的运算符</span><span class="sxs-lookup"><span data-stu-id="dd773-136">Supported operators</span></span> |
|:-------------- |:------------------- |
| <span data-ttu-id="dd773-137">id</span><span class="sxs-lookup"><span data-stu-id="dd773-137">id</span></span> | <span data-ttu-id="dd773-138">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-138">eq</span></span> |
| <span data-ttu-id="dd773-139">userId</span><span class="sxs-lookup"><span data-stu-id="dd773-139">userId</span></span> | <span data-ttu-id="dd773-140">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-140">eq</span></span> |
| <span data-ttu-id="dd773-141">appId</span><span class="sxs-lookup"><span data-stu-id="dd773-141">appId</span></span> | <span data-ttu-id="dd773-142">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-142">eq</span></span> |
| <span data-ttu-id="dd773-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd773-143">createdDateTime</span></span> | <span data-ttu-id="dd773-144">eq、le、ge</span><span class="sxs-lookup"><span data-stu-id="dd773-144">eq, le, ge</span></span> |
| <span data-ttu-id="dd773-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dd773-145">userDisplayName</span></span> | <span data-ttu-id="dd773-146">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-146">eq, startswith</span></span> |
| <span data-ttu-id="dd773-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dd773-147">userPrincipalName</span></span> | <span data-ttu-id="dd773-148">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-148">eq, startswith</span></span> |
| <span data-ttu-id="dd773-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="dd773-149">appDisplayName</span></span> | <span data-ttu-id="dd773-150">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-150">eq, startswith</span></span> |
| <span data-ttu-id="dd773-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="dd773-151">ipAddress</span></span> | <span data-ttu-id="dd773-152">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-152">eq, startswith</span></span> |
| <span data-ttu-id="dd773-153">location/city</span><span class="sxs-lookup"><span data-stu-id="dd773-153">location/city</span></span> | <span data-ttu-id="dd773-154">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-154">eq, startswith</span></span> |
| <span data-ttu-id="dd773-155">location/state</span><span class="sxs-lookup"><span data-stu-id="dd773-155">location/state</span></span> | <span data-ttu-id="dd773-156">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-156">eq, startswith</span></span> |
| <span data-ttu-id="dd773-157">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="dd773-157">location/countryOrRegion</span></span> | <span data-ttu-id="dd773-158">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-158">eq, startswith</span></span> |
| <span data-ttu-id="dd773-159">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="dd773-159">status/errorCode</span></span> | <span data-ttu-id="dd773-160">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-160">eq</span></span> |
| <span data-ttu-id="dd773-161">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="dd773-161">initiatedBy/user/id</span></span> | <span data-ttu-id="dd773-162">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-162">eq</span></span> |
| <span data-ttu-id="dd773-163">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="dd773-163">initiatedBy/user/displayName</span></span> | <span data-ttu-id="dd773-164">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-164">eq</span></span> |
| <span data-ttu-id="dd773-165">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dd773-165">initiatedBy/user/userPrincipalName</span></span> | <span data-ttu-id="dd773-166">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-166">eq, startswith</span></span> |
| <span data-ttu-id="dd773-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="dd773-167">clientAppUsed</span></span> | <span data-ttu-id="dd773-168">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-168">eq</span></span> |
| <span data-ttu-id="dd773-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="dd773-169">conditionalAccessStatus</span></span> | <span data-ttu-id="dd773-170">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-170">eq</span></span> |
| <span data-ttu-id="dd773-171">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="dd773-171">deviceDetail/browser</span></span> | <span data-ttu-id="dd773-172">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-172">eq, startswith</span></span> |
| <span data-ttu-id="dd773-173">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="dd773-173">deviceDetail/operatingSystem</span></span> | <span data-ttu-id="dd773-174">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-174">eq, startswith</span></span> |
| <span data-ttu-id="dd773-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="dd773-175">correlationId</span></span> | <span data-ttu-id="dd773-176">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-176">eq</span></span> |
| <span data-ttu-id="dd773-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="dd773-177">riskDetail</span></span> | <span data-ttu-id="dd773-178">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-178">eq</span></span> |
| <span data-ttu-id="dd773-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="dd773-179">riskLevelAggregated</span></span> | <span data-ttu-id="dd773-180">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-180">eq</span></span> |
| <span data-ttu-id="dd773-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="dd773-181">riskLevelDuringSignIn</span></span> | <span data-ttu-id="dd773-182">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-182">eq</span></span> |
| <span data-ttu-id="dd773-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="dd773-183">riskEventTypes</span></span> | <span data-ttu-id="dd773-184">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-184">eq</span></span> |
| <span data-ttu-id="dd773-185">riskState</span><span class="sxs-lookup"><span data-stu-id="dd773-185">riskState</span></span> | <span data-ttu-id="dd773-186">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-186">eq</span></span> |
| <span data-ttu-id="dd773-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="dd773-187">originalRequestId</span></span> | <span data-ttu-id="dd773-188">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-188">eq</span></span> |
| <span data-ttu-id="dd773-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="dd773-189">tokenIssuerName</span></span> | <span data-ttu-id="dd773-190">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-190">eq</span></span> |
| <span data-ttu-id="dd773-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="dd773-191">tokenIssuerType</span></span> | <span data-ttu-id="dd773-192">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-192">eq</span></span> |
| <span data-ttu-id="dd773-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="dd773-193">resourceDisplayName</span></span> | <span data-ttu-id="dd773-194">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-194">eq</span></span> |
| <span data-ttu-id="dd773-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="dd773-195">resourceId</span></span> | <span data-ttu-id="dd773-196">eq</span><span class="sxs-lookup"><span data-stu-id="dd773-196">eq</span></span> |
| <span data-ttu-id="dd773-197">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="dd773-197">servicePrincipalId</span></span> | <span data-ttu-id="dd773-198">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-198">eq, startswith</span></span> |
| <span data-ttu-id="dd773-199">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="dd773-199">servicePrincipalName</span></span> | <span data-ttu-id="dd773-200">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-200">eq, startswith</span></span> |
| <span data-ttu-id="dd773-201">userAgent</span><span class="sxs-lookup"><span data-stu-id="dd773-201">userAgent</span></span> | <span data-ttu-id="dd773-202">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-202">eq, startswith</span></span> |
| <span data-ttu-id="dd773-203">alternateSignInName</span><span class="sxs-lookup"><span data-stu-id="dd773-203">alternateSignInName</span></span> | <span data-ttu-id="dd773-204">eq、startswith</span><span class="sxs-lookup"><span data-stu-id="dd773-204">eq, startswith</span></span> |

## <a name="request-headers"></a><span data-ttu-id="dd773-205">请求头</span><span class="sxs-lookup"><span data-stu-id="dd773-205">Request headers</span></span>

| <span data-ttu-id="dd773-206">名称</span><span class="sxs-lookup"><span data-stu-id="dd773-206">Name</span></span>      |<span data-ttu-id="dd773-207">说明</span><span class="sxs-lookup"><span data-stu-id="dd773-207">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd773-208">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd773-208">Authorization</span></span> | <span data-ttu-id="dd773-209">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="dd773-209">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd773-210">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd773-210">Request body</span></span>

<span data-ttu-id="dd773-211">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd773-211">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd773-212">响应</span><span class="sxs-lookup"><span data-stu-id="dd773-212">Response</span></span>

<span data-ttu-id="dd773-213">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dd773-213">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd773-214">示例</span><span class="sxs-lookup"><span data-stu-id="dd773-214">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="dd773-215">示例1：用户使用 MFA 登录，这是由条件访问策略触发的。</span><span class="sxs-lookup"><span data-stu-id="dd773-215">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="dd773-216">主要身份验证是通过 FIDO。</span><span class="sxs-lookup"><span data-stu-id="dd773-216">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="dd773-217">请求</span><span class="sxs-lookup"><span data-stu-id="dd773-217">Request</span></span>

<span data-ttu-id="dd773-218">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dd773-218">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd773-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd773-219">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="dd773-220">C#</span><span class="sxs-lookup"><span data-stu-id="dd773-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd773-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd773-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd773-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd773-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="dd773-223">响应</span><span class="sxs-lookup"><span data-stu-id="dd773-223">Response</span></span>

<span data-ttu-id="dd773-224">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dd773-224">The following is an example of the response.</span></span>

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
### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="dd773-225">示例2：用户仅使用主身份验证进行登录。</span><span class="sxs-lookup"><span data-stu-id="dd773-225">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="dd773-226">主要身份验证通过云密码。</span><span class="sxs-lookup"><span data-stu-id="dd773-226">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="dd773-227">请求</span><span class="sxs-lookup"><span data-stu-id="dd773-227">Request</span></span>

<span data-ttu-id="dd773-228">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dd773-228">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dd773-229">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd773-229">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="dd773-230">C#</span><span class="sxs-lookup"><span data-stu-id="dd773-230">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd773-231">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd773-231">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd773-232">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd773-232">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dd773-233">响应</span><span class="sxs-lookup"><span data-stu-id="dd773-233">Response</span></span>

<span data-ttu-id="dd773-234">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dd773-234">The following is an example of the response.</span></span>

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
