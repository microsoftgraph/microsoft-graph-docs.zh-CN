---
title: 更新 identityProvider
description: 更新 identityProvider 的属性。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 34f718676926de1690d3ed9774c596168943a112
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435418"
---
# <a name="update-identityprovider"></a><span data-ttu-id="f7bab-103">更新 identityProvider</span><span class="sxs-lookup"><span data-stu-id="f7bab-103">Update identityProvider</span></span>

<span data-ttu-id="f7bab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7bab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7bab-105">更新 [identityProvider 对象](../resources/identityprovider.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f7bab-105">Update the properties of an [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7bab-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f7bab-106">Permissions</span></span>

<span data-ttu-id="f7bab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7bab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7bab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7bab-109">Permission type</span></span>      | <span data-ttu-id="f7bab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7bab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7bab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7bab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7bab-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7bab-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="f7bab-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="f7bab-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f7bab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7bab-114">Not supported.</span></span>|
|<span data-ttu-id="f7bab-115">Application</span><span class="sxs-lookup"><span data-stu-id="f7bab-115">Application</span></span>| <span data-ttu-id="f7bab-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7bab-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="f7bab-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="f7bab-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="f7bab-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="f7bab-118">Global administrator</span></span>
* <span data-ttu-id="f7bab-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="f7bab-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f7bab-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7bab-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f7bab-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7bab-121">Request headers</span></span>

|<span data-ttu-id="f7bab-122">名称</span><span class="sxs-lookup"><span data-stu-id="f7bab-122">Name</span></span>|<span data-ttu-id="f7bab-123">说明</span><span class="sxs-lookup"><span data-stu-id="f7bab-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f7bab-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7bab-124">Authorization</span></span>|<span data-ttu-id="f7bab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7bab-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f7bab-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7bab-127">Content-Type</span></span>|<span data-ttu-id="f7bab-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f7bab-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7bab-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7bab-130">Request body</span></span>

<span data-ttu-id="f7bab-131">在请求正文中，为 JSON 对象提供一个或多个属性，这些属性仅针对 Azure AD B2C ([identityProvider](../resources/identityprovider.md) 或 [openIdConnectProvider](../resources/openidconnectprovider.md)) 更新。</span><span class="sxs-lookup"><span data-stu-id="f7bab-131">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="f7bab-132">identityProvider 对象</span><span class="sxs-lookup"><span data-stu-id="f7bab-132">identityProvider object</span></span>

|<span data-ttu-id="f7bab-133">属性</span><span class="sxs-lookup"><span data-stu-id="f7bab-133">Property</span></span>|<span data-ttu-id="f7bab-134">类型</span><span class="sxs-lookup"><span data-stu-id="f7bab-134">Type</span></span>|<span data-ttu-id="f7bab-135">说明</span><span class="sxs-lookup"><span data-stu-id="f7bab-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7bab-136">clientId</span><span class="sxs-lookup"><span data-stu-id="f7bab-136">clientId</span></span>|<span data-ttu-id="f7bab-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f7bab-137">String</span></span>|<span data-ttu-id="f7bab-138">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="f7bab-138">The client ID for the application.</span></span> <span data-ttu-id="f7bab-139">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="f7bab-139">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="f7bab-140">clientSecret</span><span class="sxs-lookup"><span data-stu-id="f7bab-140">clientSecret</span></span>|<span data-ttu-id="f7bab-141">字符串</span><span class="sxs-lookup"><span data-stu-id="f7bab-141">String</span></span>|<span data-ttu-id="f7bab-142">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="f7bab-142">The client secret for the application.</span></span> <span data-ttu-id="f7bab-143">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="f7bab-143">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="f7bab-144">name</span><span class="sxs-lookup"><span data-stu-id="f7bab-144">name</span></span>|<span data-ttu-id="f7bab-145">字符串</span><span class="sxs-lookup"><span data-stu-id="f7bab-145">String</span></span>|<span data-ttu-id="f7bab-146">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f7bab-146">The display name of the identity provider.</span></span>|
|<span data-ttu-id="f7bab-147">type</span><span class="sxs-lookup"><span data-stu-id="f7bab-147">type</span></span>|<span data-ttu-id="f7bab-148">字符串</span><span class="sxs-lookup"><span data-stu-id="f7bab-148">String</span></span>|<span data-ttu-id="f7bab-149">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="f7bab-149">The identity provider type.</span></span><ul><span data-ttu-id="f7bab-150">对于 B2B 方案：</span><span class="sxs-lookup"><span data-stu-id="f7bab-150">For B2B scenario:</span></span><li/><span data-ttu-id="f7bab-151">Google</span><span class="sxs-lookup"><span data-stu-id="f7bab-151">Google</span></span><li/><span data-ttu-id="f7bab-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="f7bab-152">Facebook</span></span></ul><ul><span data-ttu-id="f7bab-153">对于 B2C 方案：</span><span class="sxs-lookup"><span data-stu-id="f7bab-153">For B2C scenario:</span></span><li/><span data-ttu-id="f7bab-154">Microsoft</span><span class="sxs-lookup"><span data-stu-id="f7bab-154">Microsoft</span></span><li/><span data-ttu-id="f7bab-155">Google</span><span class="sxs-lookup"><span data-stu-id="f7bab-155">Google</span></span><li/><span data-ttu-id="f7bab-156">Amazon</span><span class="sxs-lookup"><span data-stu-id="f7bab-156">Amazon</span></span><li/><span data-ttu-id="f7bab-157">领英</span><span class="sxs-lookup"><span data-stu-id="f7bab-157">LinkedIn</span></span><li/><span data-ttu-id="f7bab-158">Facebook</span><span class="sxs-lookup"><span data-stu-id="f7bab-158">Facebook</span></span><li/><span data-ttu-id="f7bab-159">GitHub</span><span class="sxs-lookup"><span data-stu-id="f7bab-159">GitHub</span></span><li/><span data-ttu-id="f7bab-160">Twitter</span><span class="sxs-lookup"><span data-stu-id="f7bab-160">Twitter</span></span><li/><span data-ttu-id="f7bab-161">微博</span><span class="sxs-lookup"><span data-stu-id="f7bab-161">Weibo</span></span><li/><span data-ttu-id="f7bab-162">QQ</span><span class="sxs-lookup"><span data-stu-id="f7bab-162">QQ</span></span><li/><span data-ttu-id="f7bab-163">微信</span><span class="sxs-lookup"><span data-stu-id="f7bab-163">WeChat</span></span><li/><span data-ttu-id="f7bab-164">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="f7bab-164">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="f7bab-165">openIdConnectProvider 对象</span><span class="sxs-lookup"><span data-stu-id="f7bab-165">openIdConnectProvider object</span></span>

|<span data-ttu-id="f7bab-166">属性</span><span class="sxs-lookup"><span data-stu-id="f7bab-166">Property</span></span>|<span data-ttu-id="f7bab-167">类型</span><span class="sxs-lookup"><span data-stu-id="f7bab-167">Type</span></span>|<span data-ttu-id="f7bab-168">说明</span><span class="sxs-lookup"><span data-stu-id="f7bab-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7bab-169">clientId</span><span class="sxs-lookup"><span data-stu-id="f7bab-169">clientId</span></span>|<span data-ttu-id="f7bab-170">字符串</span><span class="sxs-lookup"><span data-stu-id="f7bab-170">String</span></span>|<span data-ttu-id="f7bab-171">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="f7bab-171">The client ID for the application.</span></span> <span data-ttu-id="f7bab-172">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="f7bab-172">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="f7bab-173">clientSecret</span><span class="sxs-lookup"><span data-stu-id="f7bab-173">clientSecret</span></span>|<span data-ttu-id="f7bab-174">字符串</span><span class="sxs-lookup"><span data-stu-id="f7bab-174">String</span></span>|<span data-ttu-id="f7bab-175">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="f7bab-175">The client secret for the application.</span></span> <span data-ttu-id="f7bab-176">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="f7bab-176">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="f7bab-177">name</span><span class="sxs-lookup"><span data-stu-id="f7bab-177">name</span></span>|<span data-ttu-id="f7bab-178">字符串</span><span class="sxs-lookup"><span data-stu-id="f7bab-178">String</span></span>|<span data-ttu-id="f7bab-179">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f7bab-179">The display name of the identity provider.</span></span>|
|<span data-ttu-id="f7bab-180">type</span><span class="sxs-lookup"><span data-stu-id="f7bab-180">type</span></span>|<span data-ttu-id="f7bab-181">字符串</span><span class="sxs-lookup"><span data-stu-id="f7bab-181">String</span></span>|<span data-ttu-id="f7bab-182">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="f7bab-182">The identity provider type.</span></span> <span data-ttu-id="f7bab-183">该值必须为 `OpenIdConnect` 。</span><span class="sxs-lookup"><span data-stu-id="f7bab-183">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="f7bab-184">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="f7bab-184">claimsMapping</span></span>|[<span data-ttu-id="f7bab-185">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="f7bab-185">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="f7bab-186">在 OIDC 提供程序将 ID 令牌发送回 Azure AD 后，Azure AD 需要能够将收到的令牌中的声明映射到 Azure AD 识别和使用声明。</span><span class="sxs-lookup"><span data-stu-id="f7bab-186">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="f7bab-187">此复杂类型捕获该映射。</span><span class="sxs-lookup"><span data-stu-id="f7bab-187">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="f7bab-188">domainHint</span><span class="sxs-lookup"><span data-stu-id="f7bab-188">domainHint</span></span>|<span data-ttu-id="f7bab-189">String</span><span class="sxs-lookup"><span data-stu-id="f7bab-189">String</span></span>|<span data-ttu-id="f7bab-190">域提示可用于直接跳到指定标识提供程序的登录页，而不是让用户在可用标识提供程序的列表中进行选择。</span><span class="sxs-lookup"><span data-stu-id="f7bab-190">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="f7bab-191">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="f7bab-191">metadataUrl</span></span>|<span data-ttu-id="f7bab-192">String</span><span class="sxs-lookup"><span data-stu-id="f7bab-192">String</span></span>|<span data-ttu-id="f7bab-193">Open Id Connect 标识提供程序的元数据文档的 URL。</span><span class="sxs-lookup"><span data-stu-id="f7bab-193">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="f7bab-194">responseMode</span><span class="sxs-lookup"><span data-stu-id="f7bab-194">responseMode</span></span>|<span data-ttu-id="f7bab-195">String</span><span class="sxs-lookup"><span data-stu-id="f7bab-195">String</span></span>|<span data-ttu-id="f7bab-196">定义用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。</span><span class="sxs-lookup"><span data-stu-id="f7bab-196">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="f7bab-197">可以使用以下响应模式：</span><span class="sxs-lookup"><span data-stu-id="f7bab-197">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="f7bab-198">`form_post` ：为了获得最佳安全性，建议使用此响应模式。</span><span class="sxs-lookup"><span data-stu-id="f7bab-198">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="f7bab-199">响应通过 HTTP POST 方法传输，使用 application/x-www-form-urlencoded 格式在正文中编码代码或令牌。</span><span class="sxs-lookup"><span data-stu-id="f7bab-199">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="f7bab-200">`query` ：代码或令牌作为查询参数返回。</span><span class="sxs-lookup"><span data-stu-id="f7bab-200">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="f7bab-201">responseType</span><span class="sxs-lookup"><span data-stu-id="f7bab-201">responseType</span></span>|<span data-ttu-id="f7bab-202">String</span><span class="sxs-lookup"><span data-stu-id="f7bab-202">String</span></span>|<span data-ttu-id="f7bab-203">描述在初始调用中返回的自定义标识提供程序authorization_endpoint的信息类型。</span><span class="sxs-lookup"><span data-stu-id="f7bab-203">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="f7bab-204">可以使用以下响应类型：</span><span class="sxs-lookup"><span data-stu-id="f7bab-204">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="f7bab-205">`code` ：根据授权代码流，代码将返回到 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="f7bab-205">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="f7bab-206">Azure AD B2C 将继续调用 token_endpoint 以交换令牌的代码。</span><span class="sxs-lookup"><span data-stu-id="f7bab-206">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="f7bab-207">`id_token` ：ID 令牌从自定义标识提供程序返回回 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="f7bab-207">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="f7bab-208">`token` ：访问令牌从自定义标识提供程序返回回 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="f7bab-208">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="f7bab-209"> (Azure AD B2C 目前不支持此值) </span><span class="sxs-lookup"><span data-stu-id="f7bab-209">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="f7bab-210">scope</span><span class="sxs-lookup"><span data-stu-id="f7bab-210">scope</span></span>|<span data-ttu-id="f7bab-211">String</span><span class="sxs-lookup"><span data-stu-id="f7bab-211">String</span></span>|<span data-ttu-id="f7bab-212">范围定义要从自定义标识提供程序收集的信息和权限。</span><span class="sxs-lookup"><span data-stu-id="f7bab-212">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="f7bab-213">响应</span><span class="sxs-lookup"><span data-stu-id="f7bab-213">Response</span></span>

<span data-ttu-id="f7bab-214">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f7bab-214">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="f7bab-215">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="f7bab-215">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="f7bab-216">示例</span><span class="sxs-lookup"><span data-stu-id="f7bab-216">Examples</span></span>

### <a name="example-1-update-a-specific-identityprovider"></a><span data-ttu-id="f7bab-217">示例 1：更新特定 **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="f7bab-217">Example 1: Update a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="f7bab-218">请求</span><span class="sxs-lookup"><span data-stu-id="f7bab-218">Request</span></span>

<span data-ttu-id="f7bab-219">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7bab-219">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f7bab-220">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7bab-220">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
  "clientSecret": "1111111111111"
}
```
# <a name="c"></a>[<span data-ttu-id="f7bab-221">C#</span><span class="sxs-lookup"><span data-stu-id="f7bab-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7bab-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7bab-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7bab-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7bab-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7bab-224">Java</span><span class="sxs-lookup"><span data-stu-id="f7bab-224">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f7bab-225">响应</span><span class="sxs-lookup"><span data-stu-id="f7bab-225">Response</span></span>

<span data-ttu-id="f7bab-226">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7bab-226">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-update-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="f7bab-227">示例 2：仅为 Azure AD B2C (更新特定的 **openIDConnectProvider**) </span><span class="sxs-lookup"><span data-stu-id="f7bab-227">Example 2: Update a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="f7bab-228">请求</span><span class="sxs-lookup"><span data-stu-id="f7bab-228">Request</span></span>

<span data-ttu-id="f7bab-229">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7bab-229">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f7bab-230">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7bab-230">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identityProviders/OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a
Content-type: application/json
Content-length: 41

{
  "responseType": "id_token"
}
```
# <a name="c"></a>[<span data-ttu-id="f7bab-231">C#</span><span class="sxs-lookup"><span data-stu-id="f7bab-231">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openidconnectprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7bab-232">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7bab-232">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openidconnectprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7bab-233">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7bab-233">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openidconnectprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7bab-234">Java</span><span class="sxs-lookup"><span data-stu-id="f7bab-234">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openidconnectprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f7bab-235">响应</span><span class="sxs-lookup"><span data-stu-id="f7bab-235">Response</span></span>

<span data-ttu-id="f7bab-236">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7bab-236">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


