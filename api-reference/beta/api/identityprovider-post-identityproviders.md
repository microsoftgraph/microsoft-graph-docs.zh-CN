---
title: 创建 identityProvider
description: 创建新的 identityProvider 对象。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 93a59a479adae11840f967aaa9745f20828cdce6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435446"
---
# <a name="create-identityprovider"></a><span data-ttu-id="b01af-103">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="b01af-103">Create identityProvider</span></span>

<span data-ttu-id="b01af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b01af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b01af-105">创建新的 [identityProvider](../resources/identityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b01af-105">Create a new [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b01af-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b01af-106">Permissions</span></span>

<span data-ttu-id="b01af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b01af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b01af-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b01af-109">Permission type</span></span>      | <span data-ttu-id="b01af-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b01af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b01af-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b01af-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b01af-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b01af-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b01af-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="b01af-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b01af-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b01af-114">Not supported.</span></span>|
|<span data-ttu-id="b01af-115">Application</span><span class="sxs-lookup"><span data-stu-id="b01af-115">Application</span></span>|<span data-ttu-id="b01af-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b01af-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="b01af-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="b01af-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="b01af-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b01af-118">Global administrator</span></span>
* <span data-ttu-id="b01af-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="b01af-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="b01af-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b01af-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="b01af-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b01af-121">Request headers</span></span>

|<span data-ttu-id="b01af-122">名称</span><span class="sxs-lookup"><span data-stu-id="b01af-122">Name</span></span>|<span data-ttu-id="b01af-123">说明</span><span class="sxs-lookup"><span data-stu-id="b01af-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b01af-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b01af-124">Authorization</span></span>|<span data-ttu-id="b01af-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b01af-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b01af-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b01af-127">Content-Type</span></span>|<span data-ttu-id="b01af-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b01af-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b01af-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b01af-130">Request body</span></span>

<span data-ttu-id="b01af-131">在请求正文中，提供 [identityProvider](../resources/identityprovider.md) 或 [openIdConnectProvider](../resources/openidconnectprovider.md) (仅针对 Azure AD B2C) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b01af-131">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span> <span data-ttu-id="b01af-132">下表中列出的所有属性均未必需属性。</span><span class="sxs-lookup"><span data-stu-id="b01af-132">All the properties listed in the following table are required.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="b01af-133">identityProvider 对象</span><span class="sxs-lookup"><span data-stu-id="b01af-133">identityProvider object</span></span>

|<span data-ttu-id="b01af-134">属性</span><span class="sxs-lookup"><span data-stu-id="b01af-134">Property</span></span>|<span data-ttu-id="b01af-135">类型</span><span class="sxs-lookup"><span data-stu-id="b01af-135">Type</span></span>|<span data-ttu-id="b01af-136">说明</span><span class="sxs-lookup"><span data-stu-id="b01af-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b01af-137">clientId</span><span class="sxs-lookup"><span data-stu-id="b01af-137">clientId</span></span>|<span data-ttu-id="b01af-138">字符串</span><span class="sxs-lookup"><span data-stu-id="b01af-138">String</span></span>|<span data-ttu-id="b01af-139">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="b01af-139">The client ID for the application.</span></span> <span data-ttu-id="b01af-140">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="b01af-140">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="b01af-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="b01af-141">clientSecret</span></span>|<span data-ttu-id="b01af-142">字符串</span><span class="sxs-lookup"><span data-stu-id="b01af-142">String</span></span>|<span data-ttu-id="b01af-143">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="b01af-143">The client secret for the application.</span></span> <span data-ttu-id="b01af-144">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="b01af-144">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="b01af-145">name</span><span class="sxs-lookup"><span data-stu-id="b01af-145">name</span></span>|<span data-ttu-id="b01af-146">字符串</span><span class="sxs-lookup"><span data-stu-id="b01af-146">String</span></span>|<span data-ttu-id="b01af-147">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b01af-147">The display name of the identity provider.</span></span>|
|<span data-ttu-id="b01af-148">type</span><span class="sxs-lookup"><span data-stu-id="b01af-148">type</span></span>|<span data-ttu-id="b01af-149">字符串</span><span class="sxs-lookup"><span data-stu-id="b01af-149">String</span></span>|<span data-ttu-id="b01af-150">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="b01af-150">The identity provider type.</span></span> <ul><span data-ttu-id="b01af-151">对于 B2B 方案：</span><span class="sxs-lookup"><span data-stu-id="b01af-151">For B2B scenario:</span></span><li/><span data-ttu-id="b01af-152">Google</span><span class="sxs-lookup"><span data-stu-id="b01af-152">Google</span></span><li/><span data-ttu-id="b01af-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="b01af-153">Facebook</span></span></ul><ul><span data-ttu-id="b01af-154">对于 B2C 方案：</span><span class="sxs-lookup"><span data-stu-id="b01af-154">For B2C scenario:</span></span><li/><span data-ttu-id="b01af-155">Microsoft</span><span class="sxs-lookup"><span data-stu-id="b01af-155">Microsoft</span></span><li/><span data-ttu-id="b01af-156">Google</span><span class="sxs-lookup"><span data-stu-id="b01af-156">Google</span></span><li/><span data-ttu-id="b01af-157">Amazon</span><span class="sxs-lookup"><span data-stu-id="b01af-157">Amazon</span></span><li/><span data-ttu-id="b01af-158">领英</span><span class="sxs-lookup"><span data-stu-id="b01af-158">LinkedIn</span></span><li/><span data-ttu-id="b01af-159">Facebook</span><span class="sxs-lookup"><span data-stu-id="b01af-159">Facebook</span></span><li/><span data-ttu-id="b01af-160">GitHub</span><span class="sxs-lookup"><span data-stu-id="b01af-160">GitHub</span></span><li/><span data-ttu-id="b01af-161">Twitter</span><span class="sxs-lookup"><span data-stu-id="b01af-161">Twitter</span></span><li/><span data-ttu-id="b01af-162">微博</span><span class="sxs-lookup"><span data-stu-id="b01af-162">Weibo</span></span><li/><span data-ttu-id="b01af-163">QQ</span><span class="sxs-lookup"><span data-stu-id="b01af-163">QQ</span></span><li/><span data-ttu-id="b01af-164">微信</span><span class="sxs-lookup"><span data-stu-id="b01af-164">WeChat</span></span><li/><span data-ttu-id="b01af-165">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="b01af-165">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="b01af-166">openIdConnectProvider 对象</span><span class="sxs-lookup"><span data-stu-id="b01af-166">openIdConnectProvider object</span></span>

|<span data-ttu-id="b01af-167">属性</span><span class="sxs-lookup"><span data-stu-id="b01af-167">Property</span></span>|<span data-ttu-id="b01af-168">类型</span><span class="sxs-lookup"><span data-stu-id="b01af-168">Type</span></span>|<span data-ttu-id="b01af-169">说明</span><span class="sxs-lookup"><span data-stu-id="b01af-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b01af-170">clientId</span><span class="sxs-lookup"><span data-stu-id="b01af-170">clientId</span></span>|<span data-ttu-id="b01af-171">字符串</span><span class="sxs-lookup"><span data-stu-id="b01af-171">String</span></span>|<span data-ttu-id="b01af-172">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="b01af-172">The client ID for the application.</span></span> <span data-ttu-id="b01af-173">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="b01af-173">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="b01af-174">clientSecret</span><span class="sxs-lookup"><span data-stu-id="b01af-174">clientSecret</span></span>|<span data-ttu-id="b01af-175">字符串</span><span class="sxs-lookup"><span data-stu-id="b01af-175">String</span></span>|<span data-ttu-id="b01af-176">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="b01af-176">The client secret for the application.</span></span> <span data-ttu-id="b01af-177">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="b01af-177">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="b01af-178">name</span><span class="sxs-lookup"><span data-stu-id="b01af-178">name</span></span>|<span data-ttu-id="b01af-179">字符串</span><span class="sxs-lookup"><span data-stu-id="b01af-179">String</span></span>|<span data-ttu-id="b01af-180">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b01af-180">The display name of the identity provider.</span></span>|
|<span data-ttu-id="b01af-181">type</span><span class="sxs-lookup"><span data-stu-id="b01af-181">type</span></span>|<span data-ttu-id="b01af-182">字符串</span><span class="sxs-lookup"><span data-stu-id="b01af-182">String</span></span>|<span data-ttu-id="b01af-183">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="b01af-183">The identity provider type.</span></span> <span data-ttu-id="b01af-184">该值必须为 `OpenIdConnect` 。</span><span class="sxs-lookup"><span data-stu-id="b01af-184">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="b01af-185">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="b01af-185">claimsMapping</span></span>|[<span data-ttu-id="b01af-186">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="b01af-186">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="b01af-187">和 `userId` `displayname` 属性在 claimsMapping 对象中是必需的。</span><span class="sxs-lookup"><span data-stu-id="b01af-187">The `userId` and `displayname` properties are required in the claimsMapping object.</span></span>|
|<span data-ttu-id="b01af-188">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="b01af-188">metadataUrl</span></span>|<span data-ttu-id="b01af-189">String</span><span class="sxs-lookup"><span data-stu-id="b01af-189">String</span></span>|<span data-ttu-id="b01af-190">Open Id Connect 标识提供程序的元数据文档的 URL。</span><span class="sxs-lookup"><span data-stu-id="b01af-190">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="b01af-191">responseMode</span><span class="sxs-lookup"><span data-stu-id="b01af-191">responseMode</span></span>|<span data-ttu-id="b01af-192">String</span><span class="sxs-lookup"><span data-stu-id="b01af-192">String</span></span>|<span data-ttu-id="b01af-193">定义用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。</span><span class="sxs-lookup"><span data-stu-id="b01af-193">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="b01af-194">可以使用以下响应模式：</span><span class="sxs-lookup"><span data-stu-id="b01af-194">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="b01af-195">`form_post` ：为了获得最佳安全性，建议使用此响应模式。</span><span class="sxs-lookup"><span data-stu-id="b01af-195">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="b01af-196">响应通过 HTTP POST 方法传输，使用 application/x-www-form-urlencoded 格式在正文中编码代码或令牌。</span><span class="sxs-lookup"><span data-stu-id="b01af-196">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="b01af-197">`query` ：代码或令牌作为查询参数返回。</span><span class="sxs-lookup"><span data-stu-id="b01af-197">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="b01af-198">responseType</span><span class="sxs-lookup"><span data-stu-id="b01af-198">responseType</span></span>|<span data-ttu-id="b01af-199">String</span><span class="sxs-lookup"><span data-stu-id="b01af-199">String</span></span>|<span data-ttu-id="b01af-200">描述在初始调用中返回的自定义标识提供程序authorization_endpoint的信息类型。</span><span class="sxs-lookup"><span data-stu-id="b01af-200">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="b01af-201">可以使用以下响应类型：</span><span class="sxs-lookup"><span data-stu-id="b01af-201">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="b01af-202">`code` ：根据授权代码流，代码将返回到 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="b01af-202">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="b01af-203">Azure AD B2C 继续调用 token_endpoint 以交换令牌的代码。</span><span class="sxs-lookup"><span data-stu-id="b01af-203">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="b01af-204">`id_token` ：ID 令牌从自定义标识提供程序返回回 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="b01af-204">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="b01af-205">`token` ：访问令牌从自定义标识提供程序返回回 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="b01af-205">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="b01af-206"> (Azure AD B2C 目前不支持此值) </span><span class="sxs-lookup"><span data-stu-id="b01af-206">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="b01af-207">scope</span><span class="sxs-lookup"><span data-stu-id="b01af-207">scope</span></span>|<span data-ttu-id="b01af-208">String</span><span class="sxs-lookup"><span data-stu-id="b01af-208">String</span></span>|<span data-ttu-id="b01af-209">范围定义要从自定义标识提供程序收集的信息和权限。</span><span class="sxs-lookup"><span data-stu-id="b01af-209">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="b01af-210">响应</span><span class="sxs-lookup"><span data-stu-id="b01af-210">Response</span></span>

<span data-ttu-id="b01af-211">如果成功，此方法仅在响应正文中为 `201 Created` Azure AD B2C (返回响应代码和 [identityProvider](../resources/identityprovider.md) 或 [openIdConnectProvider](../resources/openidconnectprovider.md)) 对象。</span><span class="sxs-lookup"><span data-stu-id="b01af-211">If successful, this method returns a `201 Created` response code and [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object in the response body.</span></span> <span data-ttu-id="b01af-212">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="b01af-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="b01af-213">示例</span><span class="sxs-lookup"><span data-stu-id="b01af-213">Examples</span></span>

### <a name="example-1-create-a-specific-identityprovider"></a><span data-ttu-id="b01af-214">示例 1：创建特定 **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="b01af-214">Example 1: Create a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="b01af-215">请求</span><span class="sxs-lookup"><span data-stu-id="b01af-215">Request</span></span>

<span data-ttu-id="b01af-216">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b01af-216">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b01af-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="b01af-217">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.identityProvider",
  "name": "Login with Amazon",
  "type": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="b01af-218">C#</span><span class="sxs-lookup"><span data-stu-id="b01af-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b01af-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b01af-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b01af-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b01af-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b01af-221">Java</span><span class="sxs-lookup"><span data-stu-id="b01af-221">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b01af-222">响应</span><span class="sxs-lookup"><span data-stu-id="b01af-222">Response</span></span>

<span data-ttu-id="b01af-223">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b01af-223">The following is an example of the response.</span></span>

<span data-ttu-id="b01af-224">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b01af-224">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "@odata.type": "microsoft.graph.identityProvider",
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
### <a name="example-2-create-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="b01af-225">示例 2：仅为 Azure AD B2C (创建特定的 **openIDConnectProvider**) </span><span class="sxs-lookup"><span data-stu-id="b01af-225">Example 2: Create a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="b01af-226">请求</span><span class="sxs-lookup"><span data-stu-id="b01af-226">Request</span></span>

<span data-ttu-id="b01af-227">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b01af-227">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b01af-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="b01af-228">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_openidconnectprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
    "name": "Login with the Contoso identity provider",
    "type": "OpenIDConnect",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "12345",
    "claimsMapping": {
        "userId": "myUserId",
        "givenName": "myGivenName",
        "surname": "mySurname",
        "email": "myEmail",
        "displayName": "myDisplayName"
    },
    "domainHint": "mycustomoidc",
    "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
    "responseMode": "form_post",
    "responseType": "code",
    "scope": "openid"
}

```
# <a name="c"></a>[<span data-ttu-id="b01af-229">C#</span><span class="sxs-lookup"><span data-stu-id="b01af-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-openidconnectprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b01af-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b01af-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-openidconnectprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b01af-231">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b01af-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-openidconnectprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b01af-232">Java</span><span class="sxs-lookup"><span data-stu-id="b01af-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-openidconnectprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b01af-233">响应</span><span class="sxs-lookup"><span data-stu-id="b01af-233">Response</span></span>

<span data-ttu-id="b01af-234">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b01af-234">The following is an example of the response.</span></span>

<span data-ttu-id="b01af-235">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b01af-235">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "name": "Login with the Contoso identity provider",
  "type": "OpenIDConnect",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "12345",
  "claimsMapping": {
      "userId": "myUserId",
      "givenName": "myGivenName",
      "surname": "mySurname",
      "email": "myEmail",
      "displayName": "myDisplayName"
  },
  "domainHint": "mycustomoidc",
  "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
  "responseMode": "form_post",
  "responseType": "code",
  "scope": "openid"
}
```


