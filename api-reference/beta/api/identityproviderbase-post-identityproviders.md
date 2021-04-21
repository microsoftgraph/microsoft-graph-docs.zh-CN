---
title: 创建 identityProvider
description: 创建新的 identityProvider 对象。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 5d35265374a15cf8235d04d0fdc9c05447a6e4ad
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921308"
---
# <a name="create-identityprovider"></a><span data-ttu-id="abeda-103">创建 identityProvider</span><span class="sxs-lookup"><span data-stu-id="abeda-103">Create identityProvider</span></span>

<span data-ttu-id="abeda-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abeda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abeda-105">在 Azure AD [中创建新的 socialIdentityProvider](../resources/socialidentityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="abeda-105">Create a new [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="abeda-106">在 Azure AD B2C 中，创建新的 [socialIdentityProvider](../resources/socialidentityprovider.md) [、openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) 或 [appleIdentityProvider](../resources/appleidentityprovider.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="abeda-106">In Azure AD B2C create a new [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="abeda-107">权限</span><span class="sxs-lookup"><span data-stu-id="abeda-107">Permissions</span></span>

<span data-ttu-id="abeda-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abeda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abeda-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="abeda-110">Permission type</span></span>      | <span data-ttu-id="abeda-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="abeda-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abeda-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abeda-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abeda-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abeda-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="abeda-114">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="abeda-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="abeda-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="abeda-115">Not supported.</span></span>|
|<span data-ttu-id="abeda-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="abeda-116">Application</span></span>|<span data-ttu-id="abeda-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abeda-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="abeda-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="abeda-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="abeda-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="abeda-119">Global Administrator</span></span>
* <span data-ttu-id="abeda-120">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="abeda-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="abeda-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abeda-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="abeda-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="abeda-122">Request headers</span></span>

|<span data-ttu-id="abeda-123">名称</span><span class="sxs-lookup"><span data-stu-id="abeda-123">Name</span></span>|<span data-ttu-id="abeda-124">说明</span><span class="sxs-lookup"><span data-stu-id="abeda-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="abeda-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="abeda-125">Authorization</span></span>|<span data-ttu-id="abeda-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="abeda-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="abeda-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="abeda-128">Content-Type</span></span>|<span data-ttu-id="abeda-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="abeda-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="abeda-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="abeda-131">Request body</span></span>

<span data-ttu-id="abeda-132">在请求正文中，提供 Azure AD [中的 socialIdentityProvider](../resources/socialidentityprovider.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abeda-132">In the request body, provide a JSON representation of [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="abeda-133">在 Azure AD B2C 中，提供 [socialIdentityProvider](../resources/socialidentityprovider.md) [、openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) 或 [appleIdentityProvider](../resources/appleidentityprovider.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abeda-133">In Azure AD B2C provide a JSON representation of [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

<span data-ttu-id="abeda-134">下表中列出的所有属性均未必需属性。</span><span class="sxs-lookup"><span data-stu-id="abeda-134">All the properties listed in the following table are required.</span></span>

### <a name="socialidentityprovider-object"></a><span data-ttu-id="abeda-135">socialIdentityProvider 对象</span><span class="sxs-lookup"><span data-stu-id="abeda-135">socialIdentityProvider object</span></span>

|<span data-ttu-id="abeda-136">属性</span><span class="sxs-lookup"><span data-stu-id="abeda-136">Property</span></span>|<span data-ttu-id="abeda-137">类型</span><span class="sxs-lookup"><span data-stu-id="abeda-137">Type</span></span>|<span data-ttu-id="abeda-138">说明</span><span class="sxs-lookup"><span data-stu-id="abeda-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abeda-139">clientId</span><span class="sxs-lookup"><span data-stu-id="abeda-139">clientId</span></span>|<span data-ttu-id="abeda-140">字符串</span><span class="sxs-lookup"><span data-stu-id="abeda-140">String</span></span>|<span data-ttu-id="abeda-141">向标识提供程序注册应用程序时，获取应用程序的客户端标识符。</span><span class="sxs-lookup"><span data-stu-id="abeda-141">The client identifier for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="abeda-142">clientSecret</span><span class="sxs-lookup"><span data-stu-id="abeda-142">clientSecret</span></span>|<span data-ttu-id="abeda-143">字符串</span><span class="sxs-lookup"><span data-stu-id="abeda-143">String</span></span>|<span data-ttu-id="abeda-144">向标识提供程序注册时获取的应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="abeda-144">The client secret for the application that is obtained when the application is registered with the identity provider.</span></span> <span data-ttu-id="abeda-145">这是只读的。</span><span class="sxs-lookup"><span data-stu-id="abeda-145">This is write-only.</span></span> <span data-ttu-id="abeda-146">读取操作返回"\*\*\*\*"。</span><span class="sxs-lookup"><span data-stu-id="abeda-146">A read operation returns "\*\*\*\*".</span></span>|
|<span data-ttu-id="abeda-147">displayName</span><span class="sxs-lookup"><span data-stu-id="abeda-147">displayName</span></span>|<span data-ttu-id="abeda-148">字符串</span><span class="sxs-lookup"><span data-stu-id="abeda-148">String</span></span>|<span data-ttu-id="abeda-149">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="abeda-149">The display name of the identity provider.</span></span>|
|<span data-ttu-id="abeda-150">identityProviderType</span><span class="sxs-lookup"><span data-stu-id="abeda-150">identityProviderType</span></span>|<span data-ttu-id="abeda-151">String</span><span class="sxs-lookup"><span data-stu-id="abeda-151">String</span></span>|<span data-ttu-id="abeda-152">对于 B2B 方案，可能的值为： `Google`、 `Facebook`。</span><span class="sxs-lookup"><span data-stu-id="abeda-152">For a B2B scenario, possible values: `Google`, `Facebook`.</span></span> <span data-ttu-id="abeda-153">对于 B2C 方案，可能的值： `Microsoft`、 `Google`、 `Amazon`、 `LinkedIn`、 `Facebook`、 `GitHub`、 `Twitter`、 `Weibo`、 `QQ`、 `WeChat`。</span><span class="sxs-lookup"><span data-stu-id="abeda-153">For a B2C scenario, possible values: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.</span></span>|

### <a name="openidconnectidentityprovider-object"></a><span data-ttu-id="abeda-154">openIdConnectIdentityProvider 对象</span><span class="sxs-lookup"><span data-stu-id="abeda-154">openIdConnectIdentityProvider object</span></span>

|<span data-ttu-id="abeda-155">属性</span><span class="sxs-lookup"><span data-stu-id="abeda-155">Property</span></span>|<span data-ttu-id="abeda-156">类型</span><span class="sxs-lookup"><span data-stu-id="abeda-156">Type</span></span>|<span data-ttu-id="abeda-157">说明</span><span class="sxs-lookup"><span data-stu-id="abeda-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abeda-158">clientId</span><span class="sxs-lookup"><span data-stu-id="abeda-158">clientId</span></span>|<span data-ttu-id="abeda-159">字符串</span><span class="sxs-lookup"><span data-stu-id="abeda-159">String</span></span>|<span data-ttu-id="abeda-160">使用身份提供程序注册应用时获取的应用客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="abeda-160">The client ID for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="abeda-161">clientSecret</span><span class="sxs-lookup"><span data-stu-id="abeda-161">clientSecret</span></span>|<span data-ttu-id="abeda-162">字符串</span><span class="sxs-lookup"><span data-stu-id="abeda-162">String</span></span>|<span data-ttu-id="abeda-163">使用身份提供程序注册应用时获取的应用客户端密码。</span><span class="sxs-lookup"><span data-stu-id="abeda-163">The client secret for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="abeda-164">clientSecret 依赖于 **responseType**。</span><span class="sxs-lookup"><span data-stu-id="abeda-164">The clientSecret has a dependency on **responseType**.</span></span> <ul><li><span data-ttu-id="abeda-165">当 **responseType** `code` 为 时，身份验证代码交换需要密码。</span><span class="sxs-lookup"><span data-stu-id="abeda-165">When **responseType** is `code`, a secret is required for the auth code exchange.</span></span></li><li><span data-ttu-id="abeda-166">当 **responseType** 为密码时，由于没有代码交换，id_token直接从授权响应 `id_token` 返回密码。</span><span class="sxs-lookup"><span data-stu-id="abeda-166">When **responseType** is `id_token` the secret is not required because there is no code exchange—the id_token is returned directly from the authorization response.</span></span></li></ul>|
|<span data-ttu-id="abeda-167">displayName</span><span class="sxs-lookup"><span data-stu-id="abeda-167">displayName</span></span>|<span data-ttu-id="abeda-168">字符串</span><span class="sxs-lookup"><span data-stu-id="abeda-168">String</span></span>|<span data-ttu-id="abeda-169">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="abeda-169">The display name of the identity provider.</span></span>|
|<span data-ttu-id="abeda-170">domainHint</span><span class="sxs-lookup"><span data-stu-id="abeda-170">domainHint</span></span>|<span data-ttu-id="abeda-171">String</span><span class="sxs-lookup"><span data-stu-id="abeda-171">String</span></span>|<span data-ttu-id="abeda-172">域提示可用于直接跳到指定标识提供程序的登录页面，而不是让用户在可用标识提供程序列表中进行选择。</span><span class="sxs-lookup"><span data-stu-id="abeda-172">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="abeda-173">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="abeda-173">claimsMapping</span></span>|[<span data-ttu-id="abeda-174">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="abeda-174">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="abeda-175">OIDC 提供程序将 ID 令牌发送回 Azure AD 后，Azure AD 需要能够将收到的令牌中的声明映射到 Azure AD 识别和使用声明。</span><span class="sxs-lookup"><span data-stu-id="abeda-175">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="abeda-176">此复杂类型捕获该映射。</span><span class="sxs-lookup"><span data-stu-id="abeda-176">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="abeda-177">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="abeda-177">metadataUrl</span></span>|<span data-ttu-id="abeda-178">String</span><span class="sxs-lookup"><span data-stu-id="abeda-178">String</span></span>|<span data-ttu-id="abeda-179">OpenID Connect 标识提供程序的元数据文档的 URL。</span><span class="sxs-lookup"><span data-stu-id="abeda-179">The URL for the metadata document of the OpenID Connect identity provider.</span></span> <span data-ttu-id="abeda-180">每个 OpenID Connect 标识提供程序都描述一个元数据文档，该文档包含执行登录所需的大部分信息。</span><span class="sxs-lookup"><span data-stu-id="abeda-180">Every OpenID Connect identity provider describes a metadata document that contains most of the information required to perform sign-in.</span></span> <span data-ttu-id="abeda-181">这包括要使用的 URL 以及服务的公共签名密钥的位置等信息。</span><span class="sxs-lookup"><span data-stu-id="abeda-181">This includes information such as the URLs to use and the location of the service's public signing keys.</span></span> <span data-ttu-id="abeda-182">OpenID Connect 元数据文档始终位于 以 结尾的终结点 `.well-known/openid-configuration` 。</span><span class="sxs-lookup"><span data-stu-id="abeda-182">The OpenID Connect metadata document is always located at an endpoint that ends in `.well-known/openid-configuration`.</span></span> <span data-ttu-id="abeda-183">提供您添加的 OpenID Connect 标识提供程序的元数据 URL。</span><span class="sxs-lookup"><span data-stu-id="abeda-183">Provide the metadata URL for the OpenID Connect identity provider you add.</span></span>|
|<span data-ttu-id="abeda-184">responseMode</span><span class="sxs-lookup"><span data-stu-id="abeda-184">responseMode</span></span>|<span data-ttu-id="abeda-185">String</span><span class="sxs-lookup"><span data-stu-id="abeda-185">String</span></span>|<span data-ttu-id="abeda-186">响应模式定义用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。</span><span class="sxs-lookup"><span data-stu-id="abeda-186">The response mode defines the method used to send data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="abeda-187">可能的值 `form_post` `query` ：、。</span><span class="sxs-lookup"><span data-stu-id="abeda-187">Possible values: `form_post`, `query`.</span></span>|
|<span data-ttu-id="abeda-188">responseType</span><span class="sxs-lookup"><span data-stu-id="abeda-188">responseType</span></span>|<span data-ttu-id="abeda-189">String</span><span class="sxs-lookup"><span data-stu-id="abeda-189">String</span></span>|<span data-ttu-id="abeda-190">响应类型描述在初始调用中发送回自定义标识提供程序authorization_endpoint类型。</span><span class="sxs-lookup"><span data-stu-id="abeda-190">The response type describes the type of information sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="abeda-191">可能的值 `code` `id_token` `token` ：、、。</span><span class="sxs-lookup"><span data-stu-id="abeda-191">Possible values: `code` , `id_token` , `token`.</span></span>|
|<span data-ttu-id="abeda-192">scope</span><span class="sxs-lookup"><span data-stu-id="abeda-192">scope</span></span>|<span data-ttu-id="abeda-193">String</span><span class="sxs-lookup"><span data-stu-id="abeda-193">String</span></span>|<span data-ttu-id="abeda-194">范围定义要从自定义标识提供程序收集的信息和权限。</span><span class="sxs-lookup"><span data-stu-id="abeda-194">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

### <a name="appleidentityprovider-object"></a><span data-ttu-id="abeda-195">appleIdentityProvider 对象</span><span class="sxs-lookup"><span data-stu-id="abeda-195">appleIdentityProvider object</span></span>

|<span data-ttu-id="abeda-196">属性</span><span class="sxs-lookup"><span data-stu-id="abeda-196">Property</span></span>|<span data-ttu-id="abeda-197">类型</span><span class="sxs-lookup"><span data-stu-id="abeda-197">Type</span></span>|<span data-ttu-id="abeda-198">说明</span><span class="sxs-lookup"><span data-stu-id="abeda-198">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abeda-199">displayName</span><span class="sxs-lookup"><span data-stu-id="abeda-199">displayName</span></span>|<span data-ttu-id="abeda-200">字符串</span><span class="sxs-lookup"><span data-stu-id="abeda-200">String</span></span>|<span data-ttu-id="abeda-201">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="abeda-201">The display name of the identity provider.</span></span>|
|<span data-ttu-id="abeda-202">developerId</span><span class="sxs-lookup"><span data-stu-id="abeda-202">developerId</span></span>|<span data-ttu-id="abeda-203">String</span><span class="sxs-lookup"><span data-stu-id="abeda-203">String</span></span>|<span data-ttu-id="abeda-204">Apple 开发人员标识符。</span><span class="sxs-lookup"><span data-stu-id="abeda-204">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="abeda-205">服务 Id</span><span class="sxs-lookup"><span data-stu-id="abeda-205">serviceId</span></span>|<span data-ttu-id="abeda-206">String</span><span class="sxs-lookup"><span data-stu-id="abeda-206">String</span></span>|<span data-ttu-id="abeda-207">Apple 开发人员标识符。</span><span class="sxs-lookup"><span data-stu-id="abeda-207">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="abeda-208">keyId</span><span class="sxs-lookup"><span data-stu-id="abeda-208">keyId</span></span>|<span data-ttu-id="abeda-209">String</span><span class="sxs-lookup"><span data-stu-id="abeda-209">String</span></span>|<span data-ttu-id="abeda-210">Apple 密钥标识符。</span><span class="sxs-lookup"><span data-stu-id="abeda-210">The Apple Key identifier.</span></span>|
|<span data-ttu-id="abeda-211">certificateData</span><span class="sxs-lookup"><span data-stu-id="abeda-211">certificateData</span></span>|<span data-ttu-id="abeda-212">String</span><span class="sxs-lookup"><span data-stu-id="abeda-212">String</span></span>|<span data-ttu-id="abeda-213">证书中长文本字符串的证书数据可能是 null。</span><span class="sxs-lookup"><span data-stu-id="abeda-213">The certificate data which is a long string of text from the certificate, can be null.</span></span>|

## <a name="response"></a><span data-ttu-id="abeda-214">响应</span><span class="sxs-lookup"><span data-stu-id="abeda-214">Response</span></span>

<span data-ttu-id="abeda-215">如果成功，此方法在 Azure AD 租户的响应正文中返回 `201 Created` [socialIdentityProvider](../resources/socialidentityprovider.md) 对象的 响应代码和 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abeda-215">If successful, this method returns a `201 Created` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md) object in the response body for an Azure AD tenant.</span></span>

<span data-ttu-id="abeda-216">对于 Azure AD B2C 租户，此方法在响应正文中返回 响应代码和 `201 Created` [socialIdentityProvider](../resources/socialidentityprovider.md) [、openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) 或 [appleIdentityProvider](../resources/appleidentityprovider.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abeda-216">For an Azure AD B2C tenant, this method returns a `201 Created` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object in the response body.</span></span>

<span data-ttu-id="abeda-217">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="abeda-217">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="abeda-218">示例</span><span class="sxs-lookup"><span data-stu-id="abeda-218">Examples</span></span>

### <a name="example-1-create-a-specific-social-identity-provider-azure-ad-and-azure-ad-b2c"></a><span data-ttu-id="abeda-219">示例 1：在Azure AD 和 Azure AD B2C (创建特定的社会标识) </span><span class="sxs-lookup"><span data-stu-id="abeda-219">Example 1: Create a specific **social identity provider** (Azure AD and Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="abeda-220">请求</span><span class="sxs-lookup"><span data-stu-id="abeda-220">Request</span></span>

<span data-ttu-id="abeda-221">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="abeda-221">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="abeda-222">HTTP</span><span class="sxs-lookup"><span data-stu-id="abeda-222">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_socialidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.socialIdentityProvider",
  "displayName": "Login with Amazon",
  "identityProviderType": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="abeda-223">C#</span><span class="sxs-lookup"><span data-stu-id="abeda-223">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-socialidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abeda-224">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abeda-224">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-socialidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abeda-225">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abeda-225">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-socialidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="abeda-226">Java</span><span class="sxs-lookup"><span data-stu-id="abeda-226">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-socialidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="abeda-227">响应</span><span class="sxs-lookup"><span data-stu-id="abeda-227">Response</span></span>

<span data-ttu-id="abeda-228">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="abeda-228">The following is an example of the response.</span></span>

<span data-ttu-id="abeda-229">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="abeda-229">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.type": "microsoft.graph.socialIdentityProvider",
    "id": "Amazon-OAUTH",
    "displayName": "Login with Amazon",
    "identityProviderType": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

### <a name="example-2-create-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="abeda-230">示例 2：仅为 Azure AD B2C (创建特定的 **OpenID Connect** 标识) </span><span class="sxs-lookup"><span data-stu-id="abeda-230">Example 2: Create a specific **OpenID Connect identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="abeda-231">请求</span><span class="sxs-lookup"><span data-stu-id="abeda-231">Request</span></span>

<span data-ttu-id="abeda-232">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="abeda-232">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="abeda-233">HTTP</span><span class="sxs-lookup"><span data-stu-id="abeda-233">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_openidconnectidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
    "displayName": "Login with the Contoso identity provider",
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
# <a name="c"></a>[<span data-ttu-id="abeda-234">C#</span><span class="sxs-lookup"><span data-stu-id="abeda-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-openidconnectidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abeda-235">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abeda-235">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-openidconnectidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abeda-236">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abeda-236">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-openidconnectidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="abeda-237">Java</span><span class="sxs-lookup"><span data-stu-id="abeda-237">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-openidconnectidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="abeda-238">响应</span><span class="sxs-lookup"><span data-stu-id="abeda-238">Response</span></span>

<span data-ttu-id="abeda-239">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="abeda-239">The following is an example of the response.</span></span>

<span data-ttu-id="abeda-240">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="abeda-240">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "displayName": "Login with the Contoso identity provider",
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

### <a name="example-3-retrieves-apple-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="abeda-241">示例 3：仅为 Azure AD B2C (检索 Apple 标识) </span><span class="sxs-lookup"><span data-stu-id="abeda-241">Example 3: Retrieves Apple identity provider (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="abeda-242">请求</span><span class="sxs-lookup"><span data-stu-id="abeda-242">Request</span></span>

<span data-ttu-id="abeda-243">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="abeda-243">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="abeda-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="abeda-244">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_applemanagedidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
  "displayName": "Sign in with Apple",
  "developerId": "UBF8T346G9",
  "serviceId": "com.microsoft.rts.b2c.test.client",
  "keyId": "99P6D879C4",
  "certificateData": "******"
}
```
# <a name="javascript"></a>[<span data-ttu-id="abeda-245">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abeda-245">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-applemanagedidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abeda-246">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abeda-246">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-applemanagedidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="abeda-247">响应</span><span class="sxs-lookup"><span data-stu-id="abeda-247">Response</span></span>

<span data-ttu-id="abeda-248">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="abeda-248">The following is an example of the response.</span></span>

<span data-ttu-id="abeda-249">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="abeda-249">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
  "id": "Apple-Managed-OIDC",
  "displayName": "Sign in with Apple",
  "developerId": "UBF8T346G9",
  "serviceId": "com.microsoft.rts.b2c.test.client",
  "keyId": "99P6D879C4",
  "certificateData": "******"
}
```
