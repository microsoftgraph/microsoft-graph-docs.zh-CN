---
title: 更新 identityProvider
description: 更新 identityProvider 的属性。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4056229ecb748ff9c99a3b332298d32e67fdaf66
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921225"
---
# <a name="update-identityprovider"></a><span data-ttu-id="a65c6-103">更新 identityProvider</span><span class="sxs-lookup"><span data-stu-id="a65c6-103">Update identityProvider</span></span>
<span data-ttu-id="a65c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a65c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a65c6-105">更新 Azure AD [中的 socialIdentityProvider](../resources/socialidentityprovider.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a65c6-105">Update the properties of a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="a65c6-106">对于 Azure AD B2C，更新 [socialIdentityProvider](../resources/socialidentityprovider.md) [、openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) 或 [appleIdentityProvider 对象](../resources/appleidentityprovider.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a65c6-106">For Azure AD B2C, update the properties  of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a65c6-107">权限</span><span class="sxs-lookup"><span data-stu-id="a65c6-107">Permissions</span></span>

<span data-ttu-id="a65c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a65c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a65c6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a65c6-110">Permission type</span></span>      | <span data-ttu-id="a65c6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a65c6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a65c6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a65c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a65c6-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a65c6-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="a65c6-114">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="a65c6-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a65c6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a65c6-115">Not supported.</span></span>|
|<span data-ttu-id="a65c6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a65c6-116">Application</span></span>| <span data-ttu-id="a65c6-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a65c6-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="a65c6-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="a65c6-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a65c6-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a65c6-119">Global Administrator</span></span>
* <span data-ttu-id="a65c6-120">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="a65c6-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a65c6-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a65c6-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a65c6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a65c6-122">Request headers</span></span>

|<span data-ttu-id="a65c6-123">名称</span><span class="sxs-lookup"><span data-stu-id="a65c6-123">Name</span></span>|<span data-ttu-id="a65c6-124">说明</span><span class="sxs-lookup"><span data-stu-id="a65c6-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a65c6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a65c6-125">Authorization</span></span>|<span data-ttu-id="a65c6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a65c6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a65c6-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a65c6-128">Content-Type</span></span>|<span data-ttu-id="a65c6-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a65c6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a65c6-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a65c6-131">Request body</span></span>

<span data-ttu-id="a65c6-132">在请求正文中，为 JSON 对象提供一个或多个属性，这些属性需要针对 Azure AD 租户中的 [socialIdentityProvider](../resources/socialidentityprovider.md) 对象进行更新。</span><span class="sxs-lookup"><span data-stu-id="a65c6-132">In the request body, provide a JSON object with one or more properties that need to be updated for a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD tenant.</span></span>

<span data-ttu-id="a65c6-133">在 Azure AD B2C 中，为 JSON 对象提供一个或多个属性，这些属性需要针对 socialIdentityProvider、openIdConnectIdentityProvider 或[appleIdentityProvider](../resources/appleidentityprovider.md)对象进行更新。 [](../resources/socialidentityprovider.md) [](../resources/openidconnectidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="a65c6-133">In Azure AD B2C, provide a JSON object with one or more properties that need to be updated for a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

### <a name="socialidentityprovider-object"></a><span data-ttu-id="a65c6-134">socialIdentityProvider 对象</span><span class="sxs-lookup"><span data-stu-id="a65c6-134">socialIdentityProvider object</span></span>

|<span data-ttu-id="a65c6-135">属性</span><span class="sxs-lookup"><span data-stu-id="a65c6-135">Property</span></span>|<span data-ttu-id="a65c6-136">类型</span><span class="sxs-lookup"><span data-stu-id="a65c6-136">Type</span></span>|<span data-ttu-id="a65c6-137">说明</span><span class="sxs-lookup"><span data-stu-id="a65c6-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a65c6-138">clientId</span><span class="sxs-lookup"><span data-stu-id="a65c6-138">clientId</span></span>|<span data-ttu-id="a65c6-139">字符串</span><span class="sxs-lookup"><span data-stu-id="a65c6-139">String</span></span>|<span data-ttu-id="a65c6-140">向标识提供程序注册应用程序时，获取应用程序的客户端标识符。</span><span class="sxs-lookup"><span data-stu-id="a65c6-140">The client identifier for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="a65c6-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="a65c6-141">clientSecret</span></span>|<span data-ttu-id="a65c6-142">字符串</span><span class="sxs-lookup"><span data-stu-id="a65c6-142">String</span></span>|<span data-ttu-id="a65c6-143">向标识提供程序注册时获取的应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="a65c6-143">The client secret for the application that is obtained when the application is registered with the identity provider.</span></span> <span data-ttu-id="a65c6-144">这是只读的。</span><span class="sxs-lookup"><span data-stu-id="a65c6-144">This is write-only.</span></span> <span data-ttu-id="a65c6-145">读取操作返回"\*\*\*\*"。</span><span class="sxs-lookup"><span data-stu-id="a65c6-145">A read operation returns "\*\*\*\*".</span></span>|
|<span data-ttu-id="a65c6-146">displayName</span><span class="sxs-lookup"><span data-stu-id="a65c6-146">displayName</span></span>|<span data-ttu-id="a65c6-147">字符串</span><span class="sxs-lookup"><span data-stu-id="a65c6-147">String</span></span>|<span data-ttu-id="a65c6-148">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a65c6-148">The display name of the identity provider.</span></span>|

### <a name="openidconnectidentityprovider-object"></a><span data-ttu-id="a65c6-149">openIdConnectIdentityProvider 对象</span><span class="sxs-lookup"><span data-stu-id="a65c6-149">openIdConnectIdentityProvider object</span></span>

|<span data-ttu-id="a65c6-150">属性</span><span class="sxs-lookup"><span data-stu-id="a65c6-150">Property</span></span>|<span data-ttu-id="a65c6-151">类型</span><span class="sxs-lookup"><span data-stu-id="a65c6-151">Type</span></span>|<span data-ttu-id="a65c6-152">说明</span><span class="sxs-lookup"><span data-stu-id="a65c6-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a65c6-153">clientId</span><span class="sxs-lookup"><span data-stu-id="a65c6-153">clientId</span></span>|<span data-ttu-id="a65c6-154">字符串</span><span class="sxs-lookup"><span data-stu-id="a65c6-154">String</span></span>|<span data-ttu-id="a65c6-155">向标识提供程序注册应用程序时，获取应用程序的客户端标识符。</span><span class="sxs-lookup"><span data-stu-id="a65c6-155">The client identifier for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="a65c6-156">clientSecret</span><span class="sxs-lookup"><span data-stu-id="a65c6-156">clientSecret</span></span>|<span data-ttu-id="a65c6-157">字符串</span><span class="sxs-lookup"><span data-stu-id="a65c6-157">String</span></span>|<span data-ttu-id="a65c6-158">使用身份提供程序注册应用时获取的应用客户端密码。</span><span class="sxs-lookup"><span data-stu-id="a65c6-158">The client secret for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="a65c6-159">clientSecret 依赖于 **responseType**。</span><span class="sxs-lookup"><span data-stu-id="a65c6-159">The clientSecret has a dependency on **responseType**.</span></span> <ul><li><span data-ttu-id="a65c6-160">当 **responseType** `code` 为 时，身份验证代码交换需要密码。</span><span class="sxs-lookup"><span data-stu-id="a65c6-160">When **responseType** is `code`, a secret is required for the auth code exchange.</span></span></li><li><span data-ttu-id="a65c6-161">当 **responseType** `id_token` 为密码时不是必需的，因为没有代码交换。</span><span class="sxs-lookup"><span data-stu-id="a65c6-161">When **responseType** is `id_token` the secret is not required because there is no code exchange.</span></span> <span data-ttu-id="a65c6-162">授权id_token返回授权请求。</span><span class="sxs-lookup"><span data-stu-id="a65c6-162">The id_token is returned directly from the authorization response.</span></span></li></ul>|
|<span data-ttu-id="a65c6-163">displayName</span><span class="sxs-lookup"><span data-stu-id="a65c6-163">displayName</span></span>|<span data-ttu-id="a65c6-164">字符串</span><span class="sxs-lookup"><span data-stu-id="a65c6-164">String</span></span>|<span data-ttu-id="a65c6-165">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a65c6-165">The display name of the identity provider.</span></span>|
|<span data-ttu-id="a65c6-166">domainHint</span><span class="sxs-lookup"><span data-stu-id="a65c6-166">domainHint</span></span>|<span data-ttu-id="a65c6-167">String</span><span class="sxs-lookup"><span data-stu-id="a65c6-167">String</span></span>|<span data-ttu-id="a65c6-168">域提示可用于直接跳到指定标识提供程序的登录页面，而不是让用户在可用标识提供程序列表中进行选择。</span><span class="sxs-lookup"><span data-stu-id="a65c6-168">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="a65c6-169">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="a65c6-169">claimsMapping</span></span>|[<span data-ttu-id="a65c6-170">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="a65c6-170">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="a65c6-171">OIDC 提供程序将 ID 令牌发送回 Azure AD 后，Azure AD 需要能够将收到的令牌中的声明映射到 Azure AD 识别和使用声明。</span><span class="sxs-lookup"><span data-stu-id="a65c6-171">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="a65c6-172">此复杂类型捕获该映射。</span><span class="sxs-lookup"><span data-stu-id="a65c6-172">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="a65c6-173">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="a65c6-173">metadataUrl</span></span>|<span data-ttu-id="a65c6-174">String</span><span class="sxs-lookup"><span data-stu-id="a65c6-174">String</span></span>|<span data-ttu-id="a65c6-175">OpenID Connect 标识提供程序的元数据文档的 URL。</span><span class="sxs-lookup"><span data-stu-id="a65c6-175">The URL for the metadata document of the OpenID Connect identity provider.</span></span> <span data-ttu-id="a65c6-176">每个 OpenID Connect 标识提供程序都描述一个元数据文档，该文档包含执行登录所需的大部分信息。</span><span class="sxs-lookup"><span data-stu-id="a65c6-176">Every OpenID Connect identity provider describes a metadata document that contains most of the information required to perform sign-in.</span></span> <span data-ttu-id="a65c6-177">这包括要使用的 URL 以及服务的公共签名密钥的位置等信息。</span><span class="sxs-lookup"><span data-stu-id="a65c6-177">This includes information such as the URLs to use and the location of the service's public signing keys.</span></span> <span data-ttu-id="a65c6-178">OpenID Connect 元数据文档始终位于 以 结尾的终结点 `.well-known/openid-configuration` 。</span><span class="sxs-lookup"><span data-stu-id="a65c6-178">The OpenID Connect metadata document is always located at an endpoint that ends in `.well-known/openid-configuration`.</span></span> <span data-ttu-id="a65c6-179">提供您添加的 OpenID Connect 标识提供程序的元数据 URL。</span><span class="sxs-lookup"><span data-stu-id="a65c6-179">Provide the metadata URL for the OpenID Connect identity provider you add.</span></span>|
|<span data-ttu-id="a65c6-180">responseMode</span><span class="sxs-lookup"><span data-stu-id="a65c6-180">responseMode</span></span>|<span data-ttu-id="a65c6-181">String</span><span class="sxs-lookup"><span data-stu-id="a65c6-181">String</span></span>|<span data-ttu-id="a65c6-182">响应模式定义用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。</span><span class="sxs-lookup"><span data-stu-id="a65c6-182">The response mode defines the method used to send data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="a65c6-183">可能的值 `form_post` `query` ：、。</span><span class="sxs-lookup"><span data-stu-id="a65c6-183">Possible values: `form_post`, `query`.</span></span>|
|<span data-ttu-id="a65c6-184">responseType</span><span class="sxs-lookup"><span data-stu-id="a65c6-184">responseType</span></span>|<span data-ttu-id="a65c6-185">String</span><span class="sxs-lookup"><span data-stu-id="a65c6-185">String</span></span>|<span data-ttu-id="a65c6-186">响应类型描述在初始调用中发送回自定义标识提供程序authorization_endpoint类型。</span><span class="sxs-lookup"><span data-stu-id="a65c6-186">The response type describes the type of information sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="a65c6-187">可能的值 `code` `id_token` `token` ：、、。</span><span class="sxs-lookup"><span data-stu-id="a65c6-187">Possible values: `code` , `id_token` , `token`.</span></span>|
|<span data-ttu-id="a65c6-188">scope</span><span class="sxs-lookup"><span data-stu-id="a65c6-188">scope</span></span>|<span data-ttu-id="a65c6-189">String</span><span class="sxs-lookup"><span data-stu-id="a65c6-189">String</span></span>|<span data-ttu-id="a65c6-190">范围定义要从自定义标识提供程序收集的信息和权限。</span><span class="sxs-lookup"><span data-stu-id="a65c6-190">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

### <a name="applemanagedidentityprovider-object"></a><span data-ttu-id="a65c6-191">appleManagedIdentityProvider 对象</span><span class="sxs-lookup"><span data-stu-id="a65c6-191">appleManagedIdentityProvider object</span></span>

|<span data-ttu-id="a65c6-192">属性</span><span class="sxs-lookup"><span data-stu-id="a65c6-192">Property</span></span>|<span data-ttu-id="a65c6-193">类型</span><span class="sxs-lookup"><span data-stu-id="a65c6-193">Type</span></span>|<span data-ttu-id="a65c6-194">说明</span><span class="sxs-lookup"><span data-stu-id="a65c6-194">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a65c6-195">displayName</span><span class="sxs-lookup"><span data-stu-id="a65c6-195">displayName</span></span>|<span data-ttu-id="a65c6-196">字符串</span><span class="sxs-lookup"><span data-stu-id="a65c6-196">String</span></span>|<span data-ttu-id="a65c6-197">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a65c6-197">The display name of the identity provider.</span></span>|
|<span data-ttu-id="a65c6-198">developerId</span><span class="sxs-lookup"><span data-stu-id="a65c6-198">developerId</span></span>|<span data-ttu-id="a65c6-199">String</span><span class="sxs-lookup"><span data-stu-id="a65c6-199">String</span></span>|<span data-ttu-id="a65c6-200">Apple 开发人员标识符。</span><span class="sxs-lookup"><span data-stu-id="a65c6-200">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="a65c6-201">服务 Id</span><span class="sxs-lookup"><span data-stu-id="a65c6-201">serviceId</span></span>|<span data-ttu-id="a65c6-202">String</span><span class="sxs-lookup"><span data-stu-id="a65c6-202">String</span></span>|<span data-ttu-id="a65c6-203">Apple 开发人员标识符。</span><span class="sxs-lookup"><span data-stu-id="a65c6-203">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="a65c6-204">keyId</span><span class="sxs-lookup"><span data-stu-id="a65c6-204">keyId</span></span>|<span data-ttu-id="a65c6-205">String</span><span class="sxs-lookup"><span data-stu-id="a65c6-205">String</span></span>|<span data-ttu-id="a65c6-206">Apple 密钥标识符。</span><span class="sxs-lookup"><span data-stu-id="a65c6-206">The Apple Key identifier.</span></span>|
|<span data-ttu-id="a65c6-207">certificateData</span><span class="sxs-lookup"><span data-stu-id="a65c6-207">certificateData</span></span>|<span data-ttu-id="a65c6-208">String</span><span class="sxs-lookup"><span data-stu-id="a65c6-208">String</span></span>|<span data-ttu-id="a65c6-209">证书中长文本字符串的证书数据可能是 null。</span><span class="sxs-lookup"><span data-stu-id="a65c6-209">The certificate data which is a long string of text from the certificate, can be null.</span></span>|

## <a name="response"></a><span data-ttu-id="a65c6-210">响应</span><span class="sxs-lookup"><span data-stu-id="a65c6-210">Response</span></span>

<span data-ttu-id="a65c6-211">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a65c6-211">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="a65c6-212">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="a65c6-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="a65c6-213">示例</span><span class="sxs-lookup"><span data-stu-id="a65c6-213">Examples</span></span>

### <a name="example-1-update-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a><span data-ttu-id="a65c6-214">示例 1：使用 Azure AD 或 Azure AD B2C **(特定** 社会标识) </span><span class="sxs-lookup"><span data-stu-id="a65c6-214">Example 1: Update a specific **social identity provider** (Azure AD or Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="a65c6-215">请求</span><span class="sxs-lookup"><span data-stu-id="a65c6-215">Request</span></span>

<span data-ttu-id="a65c6-216">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a65c6-216">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a65c6-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="a65c6-217">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_socialidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Amazon-OAUTH
Content-type: application/json
Content-length: 41

{
  "clientSecret": "1111111111111"
}
```
# <a name="c"></a>[<span data-ttu-id="a65c6-218">C#</span><span class="sxs-lookup"><span data-stu-id="a65c6-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-socialidentityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a65c6-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a65c6-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-socialidentityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a65c6-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a65c6-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-socialidentityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a65c6-221">Java</span><span class="sxs-lookup"><span data-stu-id="a65c6-221">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-socialidentityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="a65c6-222">响应</span><span class="sxs-lookup"><span data-stu-id="a65c6-222">Response</span></span>

<span data-ttu-id="a65c6-223">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a65c6-223">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="a65c6-224">示例 2：仅为 Azure AD B2C (特定 **OpenID Connect** 标识提供程序) </span><span class="sxs-lookup"><span data-stu-id="a65c6-224">Example 2: Update a specific **OpenID Connect identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="a65c6-225">请求</span><span class="sxs-lookup"><span data-stu-id="a65c6-225">Request</span></span>

<span data-ttu-id="a65c6-226">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a65c6-226">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a65c6-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="a65c6-227">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/OIDC-V1-Nam_AD_Test-3e393390-ed2d-4794-97f6-5c999ccc61f7
Content-type: application/json
Content-length: 41

{
  "responseType": "id_token"
}
```
# <a name="c"></a>[<span data-ttu-id="a65c6-228">C#</span><span class="sxs-lookup"><span data-stu-id="a65c6-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openidconnectprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a65c6-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a65c6-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openidconnectprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a65c6-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a65c6-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openidconnectprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a65c6-231">Java</span><span class="sxs-lookup"><span data-stu-id="a65c6-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openidconnectprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="a65c6-232">响应</span><span class="sxs-lookup"><span data-stu-id="a65c6-232">Response</span></span>

<span data-ttu-id="a65c6-233">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a65c6-233">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-a-specific-apple-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="a65c6-234">示例 3：仅为 **Azure** AD B2C (特定 Apple 标识提供程序) </span><span class="sxs-lookup"><span data-stu-id="a65c6-234">Example 3: Update a specific **Apple identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="a65c6-235">请求</span><span class="sxs-lookup"><span data-stu-id="a65c6-235">Request</span></span>

<span data-ttu-id="a65c6-236">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a65c6-236">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a65c6-237">HTTP</span><span class="sxs-lookup"><span data-stu-id="a65c6-237">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_appleidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Apple-Managed-OIDC
Content-type: application/json
Content-length: 41

{
  "displayName": "Apple"
}
```
# <a name="c"></a>[<span data-ttu-id="a65c6-238">C#</span><span class="sxs-lookup"><span data-stu-id="a65c6-238">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-appleidentityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a65c6-239">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a65c6-239">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-appleidentityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a65c6-240">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a65c6-240">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-appleidentityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a65c6-241">Java</span><span class="sxs-lookup"><span data-stu-id="a65c6-241">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-appleidentityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="a65c6-242">响应</span><span class="sxs-lookup"><span data-stu-id="a65c6-242">Response</span></span>

<span data-ttu-id="a65c6-243">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a65c6-243">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
