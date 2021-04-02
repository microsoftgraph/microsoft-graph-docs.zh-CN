---
title: 创建 identityProvider
description: 创建新的 identityProvider 对象。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 5fe99410b965f6cabae171c713a7207fc2c7ea18
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508832"
---
# <a name="create-identityprovider-deprecated"></a><span data-ttu-id="637f0-103">创建 identityProvider (已弃) </span><span class="sxs-lookup"><span data-stu-id="637f0-103">Create identityProvider (deprecated)</span></span>

<span data-ttu-id="637f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="637f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="637f0-105">创建新的 [identityProvider](../resources/identityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="637f0-105">Create a new [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="637f0-106">权限</span><span class="sxs-lookup"><span data-stu-id="637f0-106">Permissions</span></span>

<span data-ttu-id="637f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="637f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="637f0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="637f0-109">Permission type</span></span>      | <span data-ttu-id="637f0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="637f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="637f0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="637f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="637f0-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="637f0-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="637f0-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="637f0-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="637f0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="637f0-114">Not supported.</span></span>|
|<span data-ttu-id="637f0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="637f0-115">Application</span></span>|<span data-ttu-id="637f0-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="637f0-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="637f0-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="637f0-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="637f0-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="637f0-118">Global Administrator</span></span>
* <span data-ttu-id="637f0-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="637f0-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="637f0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="637f0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="637f0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="637f0-121">Request headers</span></span>

|<span data-ttu-id="637f0-122">名称</span><span class="sxs-lookup"><span data-stu-id="637f0-122">Name</span></span>|<span data-ttu-id="637f0-123">说明</span><span class="sxs-lookup"><span data-stu-id="637f0-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="637f0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="637f0-124">Authorization</span></span>|<span data-ttu-id="637f0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="637f0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="637f0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="637f0-127">Content-Type</span></span>|<span data-ttu-id="637f0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="637f0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="637f0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="637f0-130">Request body</span></span>

<span data-ttu-id="637f0-131">在请求正文中，仅为 Azure AD B2C (提供 [identityProvider](../resources/identityprovider.md) 或 [openIdConnectProvider](../resources/openidconnectprovider.md)) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="637f0-131">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span> <span data-ttu-id="637f0-132">下表中列出的所有属性均未必需属性。</span><span class="sxs-lookup"><span data-stu-id="637f0-132">All the properties listed in the following table are required.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="637f0-133">identityProvider 对象</span><span class="sxs-lookup"><span data-stu-id="637f0-133">identityProvider object</span></span>

|<span data-ttu-id="637f0-134">属性</span><span class="sxs-lookup"><span data-stu-id="637f0-134">Property</span></span>|<span data-ttu-id="637f0-135">类型</span><span class="sxs-lookup"><span data-stu-id="637f0-135">Type</span></span>|<span data-ttu-id="637f0-136">说明</span><span class="sxs-lookup"><span data-stu-id="637f0-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="637f0-137">clientId</span><span class="sxs-lookup"><span data-stu-id="637f0-137">clientId</span></span>|<span data-ttu-id="637f0-138">字符串</span><span class="sxs-lookup"><span data-stu-id="637f0-138">String</span></span>|<span data-ttu-id="637f0-139">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="637f0-139">The client ID for the application.</span></span> <span data-ttu-id="637f0-140">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="637f0-140">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="637f0-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="637f0-141">clientSecret</span></span>|<span data-ttu-id="637f0-142">字符串</span><span class="sxs-lookup"><span data-stu-id="637f0-142">String</span></span>|<span data-ttu-id="637f0-143">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="637f0-143">The client secret for the application.</span></span> <span data-ttu-id="637f0-144">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="637f0-144">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="637f0-145">name</span><span class="sxs-lookup"><span data-stu-id="637f0-145">name</span></span>|<span data-ttu-id="637f0-146">字符串</span><span class="sxs-lookup"><span data-stu-id="637f0-146">String</span></span>|<span data-ttu-id="637f0-147">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="637f0-147">The display name of the identity provider.</span></span>|
|<span data-ttu-id="637f0-148">type</span><span class="sxs-lookup"><span data-stu-id="637f0-148">type</span></span>|<span data-ttu-id="637f0-149">字符串</span><span class="sxs-lookup"><span data-stu-id="637f0-149">String</span></span>|<span data-ttu-id="637f0-150">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="637f0-150">The identity provider type.</span></span> <ul><span data-ttu-id="637f0-151">对于 B2B 方案：</span><span class="sxs-lookup"><span data-stu-id="637f0-151">For B2B scenario:</span></span><li/><span data-ttu-id="637f0-152">Google</span><span class="sxs-lookup"><span data-stu-id="637f0-152">Google</span></span><li/><span data-ttu-id="637f0-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="637f0-153">Facebook</span></span></ul><ul><span data-ttu-id="637f0-154">对于 B2C 方案：</span><span class="sxs-lookup"><span data-stu-id="637f0-154">For B2C scenario:</span></span><li/><span data-ttu-id="637f0-155">Microsoft</span><span class="sxs-lookup"><span data-stu-id="637f0-155">Microsoft</span></span><li/><span data-ttu-id="637f0-156">Google</span><span class="sxs-lookup"><span data-stu-id="637f0-156">Google</span></span><li/><span data-ttu-id="637f0-157">Amazon</span><span class="sxs-lookup"><span data-stu-id="637f0-157">Amazon</span></span><li/><span data-ttu-id="637f0-158">领英</span><span class="sxs-lookup"><span data-stu-id="637f0-158">LinkedIn</span></span><li/><span data-ttu-id="637f0-159">Facebook</span><span class="sxs-lookup"><span data-stu-id="637f0-159">Facebook</span></span><li/><span data-ttu-id="637f0-160">GitHub</span><span class="sxs-lookup"><span data-stu-id="637f0-160">GitHub</span></span><li/><span data-ttu-id="637f0-161">Twitter</span><span class="sxs-lookup"><span data-stu-id="637f0-161">Twitter</span></span><li/><span data-ttu-id="637f0-162">微博</span><span class="sxs-lookup"><span data-stu-id="637f0-162">Weibo</span></span><li/><span data-ttu-id="637f0-163">QQ</span><span class="sxs-lookup"><span data-stu-id="637f0-163">QQ</span></span><li/><span data-ttu-id="637f0-164">微信</span><span class="sxs-lookup"><span data-stu-id="637f0-164">WeChat</span></span><li/><span data-ttu-id="637f0-165">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="637f0-165">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="637f0-166">openIdConnectProvider 对象</span><span class="sxs-lookup"><span data-stu-id="637f0-166">openIdConnectProvider object</span></span>

|<span data-ttu-id="637f0-167">属性</span><span class="sxs-lookup"><span data-stu-id="637f0-167">Property</span></span>|<span data-ttu-id="637f0-168">类型</span><span class="sxs-lookup"><span data-stu-id="637f0-168">Type</span></span>|<span data-ttu-id="637f0-169">说明</span><span class="sxs-lookup"><span data-stu-id="637f0-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="637f0-170">clientId</span><span class="sxs-lookup"><span data-stu-id="637f0-170">clientId</span></span>|<span data-ttu-id="637f0-171">字符串</span><span class="sxs-lookup"><span data-stu-id="637f0-171">String</span></span>|<span data-ttu-id="637f0-172">应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="637f0-172">The client ID for the application.</span></span> <span data-ttu-id="637f0-173">这是向标识提供程序注册应用程序时获取的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="637f0-173">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="637f0-174">clientSecret</span><span class="sxs-lookup"><span data-stu-id="637f0-174">clientSecret</span></span>|<span data-ttu-id="637f0-175">字符串</span><span class="sxs-lookup"><span data-stu-id="637f0-175">String</span></span>|<span data-ttu-id="637f0-176">应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="637f0-176">The client secret for the application.</span></span> <span data-ttu-id="637f0-177">这是向标识提供程序注册应用程序时获取的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="637f0-177">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="637f0-178">name</span><span class="sxs-lookup"><span data-stu-id="637f0-178">name</span></span>|<span data-ttu-id="637f0-179">字符串</span><span class="sxs-lookup"><span data-stu-id="637f0-179">String</span></span>|<span data-ttu-id="637f0-180">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="637f0-180">The display name of the identity provider.</span></span>|
|<span data-ttu-id="637f0-181">type</span><span class="sxs-lookup"><span data-stu-id="637f0-181">type</span></span>|<span data-ttu-id="637f0-182">字符串</span><span class="sxs-lookup"><span data-stu-id="637f0-182">String</span></span>|<span data-ttu-id="637f0-183">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="637f0-183">The identity provider type.</span></span> <span data-ttu-id="637f0-184">值必须为 `OpenIdConnect` 。</span><span class="sxs-lookup"><span data-stu-id="637f0-184">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="637f0-185">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="637f0-185">claimsMapping</span></span>|[<span data-ttu-id="637f0-186">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="637f0-186">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="637f0-187">和 `userId` `displayname` 属性在 claimsMapping 对象中是必需的。</span><span class="sxs-lookup"><span data-stu-id="637f0-187">The `userId` and `displayname` properties are required in the claimsMapping object.</span></span>|
|<span data-ttu-id="637f0-188">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="637f0-188">metadataUrl</span></span>|<span data-ttu-id="637f0-189">字符串</span><span class="sxs-lookup"><span data-stu-id="637f0-189">String</span></span>|<span data-ttu-id="637f0-190">Open Id Connect 标识提供程序的元数据文档的 URL。</span><span class="sxs-lookup"><span data-stu-id="637f0-190">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="637f0-191">responseMode</span><span class="sxs-lookup"><span data-stu-id="637f0-191">responseMode</span></span>|<span data-ttu-id="637f0-192">字符串</span><span class="sxs-lookup"><span data-stu-id="637f0-192">String</span></span>|<span data-ttu-id="637f0-193">定义用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。</span><span class="sxs-lookup"><span data-stu-id="637f0-193">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="637f0-194">可以使用以下响应模式：</span><span class="sxs-lookup"><span data-stu-id="637f0-194">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="637f0-195">`form_post` ：建议采用此响应模式，以获得最佳安全性。</span><span class="sxs-lookup"><span data-stu-id="637f0-195">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="637f0-196">响应通过 HTTP POST 方法传输，使用 application/x-www-form-urlencoded 格式在正文中编码代码或令牌。</span><span class="sxs-lookup"><span data-stu-id="637f0-196">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="637f0-197">`query` ：代码或令牌作为查询参数返回。</span><span class="sxs-lookup"><span data-stu-id="637f0-197">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="637f0-198">responseType</span><span class="sxs-lookup"><span data-stu-id="637f0-198">responseType</span></span>|<span data-ttu-id="637f0-199">字符串</span><span class="sxs-lookup"><span data-stu-id="637f0-199">String</span></span>|<span data-ttu-id="637f0-200">描述在初始调用自定义标识提供程序的 authorization_endpoint发送回的信息类型。</span><span class="sxs-lookup"><span data-stu-id="637f0-200">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="637f0-201">可以使用以下响应类型：</span><span class="sxs-lookup"><span data-stu-id="637f0-201">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="637f0-202">`code` ：根据授权代码流，代码将返回到 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="637f0-202">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="637f0-203">Azure AD B2C 继续调用 token_endpoint 以交换令牌代码。</span><span class="sxs-lookup"><span data-stu-id="637f0-203">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="637f0-204">`id_token` ：ID 令牌从自定义标识提供程序返回回 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="637f0-204">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="637f0-205">`token` ：访问令牌从自定义标识提供程序返回回 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="637f0-205">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="637f0-206"> (当前 Azure AD B2C 不支持) </span><span class="sxs-lookup"><span data-stu-id="637f0-206">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="637f0-207">scope</span><span class="sxs-lookup"><span data-stu-id="637f0-207">scope</span></span>|<span data-ttu-id="637f0-208">String</span><span class="sxs-lookup"><span data-stu-id="637f0-208">String</span></span>|<span data-ttu-id="637f0-209">范围定义要从自定义标识提供程序收集的信息和权限。</span><span class="sxs-lookup"><span data-stu-id="637f0-209">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="637f0-210">响应</span><span class="sxs-lookup"><span data-stu-id="637f0-210">Response</span></span>

<span data-ttu-id="637f0-211">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [identityProvider](../resources/identityprovider.md) 或 [openIdConnectProvider](../resources/openidconnectprovider.md) (仅适用于 Azure AD B2C) 对象。</span><span class="sxs-lookup"><span data-stu-id="637f0-211">If successful, this method returns a `201 Created` response code and [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object in the response body.</span></span> <span data-ttu-id="637f0-212">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="637f0-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="637f0-213">示例</span><span class="sxs-lookup"><span data-stu-id="637f0-213">Examples</span></span>

### <a name="example-1-create-a-specific-identityprovider"></a><span data-ttu-id="637f0-214">示例 1：创建特定 **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="637f0-214">Example 1: Create a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="637f0-215">请求</span><span class="sxs-lookup"><span data-stu-id="637f0-215">Request</span></span>

<span data-ttu-id="637f0-216">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="637f0-216">The following is an example of the request.</span></span>

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

# <a name="java"></a>[<span data-ttu-id="637f0-217">Java</span><span class="sxs-lookup"><span data-stu-id="637f0-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="637f0-218">C#</span><span class="sxs-lookup"><span data-stu-id="637f0-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="637f0-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="637f0-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="637f0-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="637f0-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="637f0-221">响应</span><span class="sxs-lookup"><span data-stu-id="637f0-221">Response</span></span>

<span data-ttu-id="637f0-222">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="637f0-222">The following is an example of the response.</span></span>

<span data-ttu-id="637f0-223">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="637f0-223">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="637f0-224">示例 2：仅为 Azure AD B2C (创建特定的 **openIDConnectProvider**) </span><span class="sxs-lookup"><span data-stu-id="637f0-224">Example 2: Create a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="637f0-225">请求</span><span class="sxs-lookup"><span data-stu-id="637f0-225">Request</span></span>

<span data-ttu-id="637f0-226">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="637f0-226">The following is an example of the request.</span></span>

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

# <a name="java"></a>[<span data-ttu-id="637f0-227">Java</span><span class="sxs-lookup"><span data-stu-id="637f0-227">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-openidconnectprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="637f0-228">C#</span><span class="sxs-lookup"><span data-stu-id="637f0-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-openidconnectprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="637f0-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="637f0-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-openidconnectprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="637f0-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="637f0-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-openidconnectprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="637f0-231">响应</span><span class="sxs-lookup"><span data-stu-id="637f0-231">Response</span></span>

<span data-ttu-id="637f0-232">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="637f0-232">The following is an example of the response.</span></span>

<span data-ttu-id="637f0-233">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="637f0-233">**Note:** The response object shown here might be shortened for readability.</span></span>

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
