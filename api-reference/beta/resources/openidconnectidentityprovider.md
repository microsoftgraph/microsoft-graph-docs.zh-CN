---
title: openIdConnectIdentityProvider 资源类型
description: 表示 Azure Active Directory B2C 租户中的 OpenIDConnect 标识提供程序。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 990deba52cc4c3ff66f4dd36f0fb795497b97af4
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491101"
---
# <a name="openidconnectidentityprovider-resource-type"></a><span data-ttu-id="35b4c-103">openIdConnectIdentityProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="35b4c-103">openIdConnectIdentityProvider resource type</span></span>
<span data-ttu-id="35b4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35b4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35b4c-105">表示 Azure Active Directory B2C 租户中的 OpenID Connect 标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="35b4c-105">Represents OpenID Connect identity providers in an Azure Active Directory B2C tenant.</span></span>

<span data-ttu-id="35b4c-106">通过配置 B2C 租户中的 OpenID Connect 提供程序，用户可以在应用程序中使用其自定义标识提供程序进行注册和登录。</span><span class="sxs-lookup"><span data-stu-id="35b4c-106">Configuring an OpenID Connect provider in a B2C tenant enables users to sign up and sign in using their custom identity provider in an application.</span></span>

<span data-ttu-id="35b4c-107">此类型将继承自 [identityProviderBase](../resources/identityproviderbase.md)。</span><span class="sxs-lookup"><span data-stu-id="35b4c-107">This type will inherit from [identityProviderBase](../resources/identityproviderbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="35b4c-108">方法</span><span class="sxs-lookup"><span data-stu-id="35b4c-108">Methods</span></span>

| <span data-ttu-id="35b4c-109">方法</span><span class="sxs-lookup"><span data-stu-id="35b4c-109">Method</span></span>       | <span data-ttu-id="35b4c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="35b4c-110">Return Type</span></span>  |<span data-ttu-id="35b4c-111">Description</span><span class="sxs-lookup"><span data-stu-id="35b4c-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35b4c-112">List</span><span class="sxs-lookup"><span data-stu-id="35b4c-112">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="35b4c-113">[identityProviderBase](../resources/identityproviderbase.md)  集合</span><span class="sxs-lookup"><span data-stu-id="35b4c-113">[identityProviderBase](../resources/identityproviderbase.md)  collection</span></span>|<span data-ttu-id="35b4c-114">检索在租户中配置的所有标识提供程序，包括 OpenID Connect 标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="35b4c-114">Retrieve all identity providers configured in a tenant including the OpenID Connect identity providers.</span></span>|
|[<span data-ttu-id="35b4c-115">创建</span><span class="sxs-lookup"><span data-stu-id="35b4c-115">Create</span></span>](../api/identityproviderbase-post-identityproviders.md)|<span data-ttu-id="35b4c-116">openIdConnectIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="35b4c-116">openIdConnectIdentityProvider</span></span>|<span data-ttu-id="35b4c-117">创建新的 OpenID Connect 标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="35b4c-117">Create a new OpenID Connect identity provider.</span></span>|
|[<span data-ttu-id="35b4c-118">获取</span><span class="sxs-lookup"><span data-stu-id="35b4c-118">Get</span></span>](../api/identityproviderbase-get.md) |<span data-ttu-id="35b4c-119">openIdConnectIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="35b4c-119">openIdConnectIdentityProvider</span></span>|<span data-ttu-id="35b4c-120">检索 OpenID Connect 标识提供程序的属性。</span><span class="sxs-lookup"><span data-stu-id="35b4c-120">Retrieve properties of an OpenID Connect identity provider.</span></span>|
|[<span data-ttu-id="35b4c-121">更新</span><span class="sxs-lookup"><span data-stu-id="35b4c-121">Update</span></span>](../api/identityproviderbase-update.md)|<span data-ttu-id="35b4c-122">无</span><span class="sxs-lookup"><span data-stu-id="35b4c-122">None</span></span>|<span data-ttu-id="35b4c-123">更新 OpenID Connect 标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="35b4c-123">Update an OpenID Connect identity provider.</span></span>|
|[<span data-ttu-id="35b4c-124">删除</span><span class="sxs-lookup"><span data-stu-id="35b4c-124">Delete</span></span>](../api/identityproviderbase-delete.md)|<span data-ttu-id="35b4c-125">无</span><span class="sxs-lookup"><span data-stu-id="35b4c-125">None</span></span>|<span data-ttu-id="35b4c-126">删除 OpenID Connect 标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="35b4c-126">Delete an OpenID Connect identity provider.</span></span>|
|[<span data-ttu-id="35b4c-127">列出可用的提供程序类型</span><span class="sxs-lookup"><span data-stu-id="35b4c-127">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="35b4c-128">String 集合</span><span class="sxs-lookup"><span data-stu-id="35b4c-128">String collection</span></span>|<span data-ttu-id="35b4c-129">检索租户中所有可用的标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="35b4c-129">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="35b4c-130">属性</span><span class="sxs-lookup"><span data-stu-id="35b4c-130">Properties</span></span>

|<span data-ttu-id="35b4c-131">属性</span><span class="sxs-lookup"><span data-stu-id="35b4c-131">Property</span></span>|<span data-ttu-id="35b4c-132">类型</span><span class="sxs-lookup"><span data-stu-id="35b4c-132">Type</span></span>|<span data-ttu-id="35b4c-133">说明</span><span class="sxs-lookup"><span data-stu-id="35b4c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35b4c-134">clientId</span><span class="sxs-lookup"><span data-stu-id="35b4c-134">clientId</span></span>|<span data-ttu-id="35b4c-135">字符串</span><span class="sxs-lookup"><span data-stu-id="35b4c-135">String</span></span>|<span data-ttu-id="35b4c-136">使用身份提供程序注册应用时获取的应用客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="35b4c-136">The client ID for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="35b4c-137">必需。</span><span class="sxs-lookup"><span data-stu-id="35b4c-137">Required.</span></span>|
|<span data-ttu-id="35b4c-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="35b4c-138">clientSecret</span></span>|<span data-ttu-id="35b4c-139">字符串</span><span class="sxs-lookup"><span data-stu-id="35b4c-139">String</span></span>|<span data-ttu-id="35b4c-140">使用身份提供程序注册应用时获取的应用客户端密码。</span><span class="sxs-lookup"><span data-stu-id="35b4c-140">The client secret for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="35b4c-141">clientSecret 依赖于 **responseType**。</span><span class="sxs-lookup"><span data-stu-id="35b4c-141">The clientSecret has a dependency on **responseType**.</span></span> <ul><li><span data-ttu-id="35b4c-142">当 **responseType** `code` 为 时，身份验证代码交换需要密码。</span><span class="sxs-lookup"><span data-stu-id="35b4c-142">When **responseType** is `code`, a secret is required for the auth code exchange.</span></span></li><li><span data-ttu-id="35b4c-143">当 **responseType** `id_token` 为密码时不是必需的，因为没有代码交换。</span><span class="sxs-lookup"><span data-stu-id="35b4c-143">When **responseType** is `id_token` the secret is not required because there is no code exchange.</span></span> <span data-ttu-id="35b4c-144">授权id_token返回授权请求。</span><span class="sxs-lookup"><span data-stu-id="35b4c-144">The id_token is returned directly from the authorization response.</span></span></li></ul> <span data-ttu-id="35b4c-145">这是只读的。</span><span class="sxs-lookup"><span data-stu-id="35b4c-145">This is write-only.</span></span> <span data-ttu-id="35b4c-146">读取操作返回" \* \* \* \* "。</span><span class="sxs-lookup"><span data-stu-id="35b4c-146">A read operation returns "\*\*\*\*".</span></span>|
|<span data-ttu-id="35b4c-147">id</span><span class="sxs-lookup"><span data-stu-id="35b4c-147">id</span></span>|<span data-ttu-id="35b4c-148">String</span><span class="sxs-lookup"><span data-stu-id="35b4c-148">String</span></span>|<span data-ttu-id="35b4c-149">标识提供程序的标识符。必填。</span><span class="sxs-lookup"><span data-stu-id="35b4c-149">The identifier of the identity provider.Required.</span></span> <span data-ttu-id="35b4c-150">继承自 [identityProviderBase](../resources/identityproviderbase.md)。</span><span class="sxs-lookup"><span data-stu-id="35b4c-150">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span> <span data-ttu-id="35b4c-151">只读。</span><span class="sxs-lookup"><span data-stu-id="35b4c-151">Read-only.</span></span>|
|<span data-ttu-id="35b4c-152">displayName</span><span class="sxs-lookup"><span data-stu-id="35b4c-152">displayName</span></span>|<span data-ttu-id="35b4c-153">字符串</span><span class="sxs-lookup"><span data-stu-id="35b4c-153">String</span></span>|<span data-ttu-id="35b4c-154">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="35b4c-154">The display name of the identity provider.</span></span> |
|<span data-ttu-id="35b4c-155">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="35b4c-155">claimsMapping</span></span>|[<span data-ttu-id="35b4c-156">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="35b4c-156">claimsMapping</span></span>](claimsmapping.md)|<span data-ttu-id="35b4c-157">OIDC 提供程序将 ID 令牌发送回 Azure AD 后，Azure AD 需要能够将收到的令牌中的声明映射到 Azure AD 识别和使用声明。</span><span class="sxs-lookup"><span data-stu-id="35b4c-157">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="35b4c-158">此复杂类型捕获该映射。</span><span class="sxs-lookup"><span data-stu-id="35b4c-158">This complex type captures that mapping.</span></span> <span data-ttu-id="35b4c-159">必需。</span><span class="sxs-lookup"><span data-stu-id="35b4c-159">Required.</span></span>|
|<span data-ttu-id="35b4c-160">domainHint</span><span class="sxs-lookup"><span data-stu-id="35b4c-160">domainHint</span></span>|<span data-ttu-id="35b4c-161">String</span><span class="sxs-lookup"><span data-stu-id="35b4c-161">String</span></span>|<span data-ttu-id="35b4c-162">域提示可用于直接跳到指定标识提供程序的登录页面，而不是让用户在可用标识提供程序列表中进行选择。</span><span class="sxs-lookup"><span data-stu-id="35b4c-162">The domain hint can be used to skip directly to the sign-in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="35b4c-163">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="35b4c-163">metadataUrl</span></span>|<span data-ttu-id="35b4c-164">String</span><span class="sxs-lookup"><span data-stu-id="35b4c-164">String</span></span>|<span data-ttu-id="35b4c-165">OpenID Connect 标识提供程序的元数据文档的 URL。</span><span class="sxs-lookup"><span data-stu-id="35b4c-165">The URL for the metadata document of the OpenID Connect identity provider.</span></span> <span data-ttu-id="35b4c-166">每个 OpenID Connect 标识提供程序都描述一个元数据文档，该文档包含执行登录所需的大部分信息。</span><span class="sxs-lookup"><span data-stu-id="35b4c-166">Every OpenID Connect identity provider describes a metadata document that contains most of the information required to perform sign-in.</span></span> <span data-ttu-id="35b4c-167">这包括要使用的 URL 以及服务的公共签名密钥的位置等信息。</span><span class="sxs-lookup"><span data-stu-id="35b4c-167">This includes information such as the URLs to use and the location of the service's public signing keys.</span></span> <span data-ttu-id="35b4c-168">OpenID Connect 元数据文档始终位于 以 结尾的终结点 `.well-known/openid-configuration` 。</span><span class="sxs-lookup"><span data-stu-id="35b4c-168">The OpenID Connect metadata document is always located at an endpoint that ends in `.well-known/openid-configuration`.</span></span> <span data-ttu-id="35b4c-169">提供您添加的 OpenID Connect 标识提供程序的元数据 URL。</span><span class="sxs-lookup"><span data-stu-id="35b4c-169">Provide the metadata URL for the OpenID Connect identity provider you add.</span></span> <span data-ttu-id="35b4c-170">只读。</span><span class="sxs-lookup"><span data-stu-id="35b4c-170">Read-only.</span></span> <span data-ttu-id="35b4c-171">必需。</span><span class="sxs-lookup"><span data-stu-id="35b4c-171">Required.</span></span>|
|<span data-ttu-id="35b4c-172">responseMode</span><span class="sxs-lookup"><span data-stu-id="35b4c-172">responseMode</span></span>|<span data-ttu-id="35b4c-173">String</span><span class="sxs-lookup"><span data-stu-id="35b4c-173">String</span></span>|<span data-ttu-id="35b4c-174">响应模式定义用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。</span><span class="sxs-lookup"><span data-stu-id="35b4c-174">The response mode defines the method used to send data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="35b4c-175">可能的值 `form_post` `query` ：、。</span><span class="sxs-lookup"><span data-stu-id="35b4c-175">Possible values: `form_post`, `query`.</span></span> <span data-ttu-id="35b4c-176">必需。</span><span class="sxs-lookup"><span data-stu-id="35b4c-176">Required.</span></span>|
|<span data-ttu-id="35b4c-177">responseType</span><span class="sxs-lookup"><span data-stu-id="35b4c-177">responseType</span></span>|<span data-ttu-id="35b4c-178">String</span><span class="sxs-lookup"><span data-stu-id="35b4c-178">String</span></span>|<span data-ttu-id="35b4c-179">响应类型描述在初始调用中发送回自定义标识提供程序authorization_endpoint类型。</span><span class="sxs-lookup"><span data-stu-id="35b4c-179">The response type describes the type of information sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="35b4c-180">可能的值 `code` `id_token` `token` ：、、。</span><span class="sxs-lookup"><span data-stu-id="35b4c-180">Possible values: `code` , `id_token` , `token`.</span></span>  <span data-ttu-id="35b4c-181">必需。</span><span class="sxs-lookup"><span data-stu-id="35b4c-181">Required.</span></span>|
|<span data-ttu-id="35b4c-182">scope</span><span class="sxs-lookup"><span data-stu-id="35b4c-182">scope</span></span>|<span data-ttu-id="35b4c-183">String</span><span class="sxs-lookup"><span data-stu-id="35b4c-183">String</span></span>|<span data-ttu-id="35b4c-184">范围定义要从自定义标识提供程序收集的信息和权限。</span><span class="sxs-lookup"><span data-stu-id="35b4c-184">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span> <span data-ttu-id="35b4c-185">OpenID Connect 请求必须包含 openid 范围值才能从标识提供程序接收 ID 令牌。</span><span class="sxs-lookup"><span data-stu-id="35b4c-185">OpenID Connect requests must contain the openid scope value in order to receive the ID token from the identity provider.</span></span> <span data-ttu-id="35b4c-186">如果没有 ID 令牌，用户将无法使用自定义标识提供程序登录到 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="35b4c-186">Without the ID token, users are not able to sign in to Azure AD B2C using the custom identity provider.</span></span> <span data-ttu-id="35b4c-187">其他范围可以追加，用空格分隔。</span><span class="sxs-lookup"><span data-stu-id="35b4c-187">Other scopes can be appended, separated by a space.</span></span> <span data-ttu-id="35b4c-188">有关范围限制的更多详细信息，请参阅 [RFC6749 第 3.3 节](https://tools.ietf.org/html/rfc6749#section-3.3)。</span><span class="sxs-lookup"><span data-stu-id="35b4c-188">For more details about the scope limitations see [RFC6749 Section 3.3](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> <span data-ttu-id="35b4c-189">必需。</span><span class="sxs-lookup"><span data-stu-id="35b4c-189">Required.</span></span>|

### <a name="responsemode-value"></a><span data-ttu-id="35b4c-190">responseMode 值</span><span class="sxs-lookup"><span data-stu-id="35b4c-190">responseMode value</span></span>
|<span data-ttu-id="35b4c-191">值</span><span class="sxs-lookup"><span data-stu-id="35b4c-191">Value</span></span>|<span data-ttu-id="35b4c-192">说明</span><span class="sxs-lookup"><span data-stu-id="35b4c-192">Description</span></span>|
:--------|:----------|
|<span data-ttu-id="35b4c-193">form_post</span><span class="sxs-lookup"><span data-stu-id="35b4c-193">form_post</span></span>|<span data-ttu-id="35b4c-194">为获得最佳安全性，建议采用此响应模式。</span><span class="sxs-lookup"><span data-stu-id="35b4c-194">This response mode is recommended for best security.</span></span> <span data-ttu-id="35b4c-195">响应通过 HTTP POST 方法传输，使用 application/x-www-form-urlencoded 格式在正文中编码代码或令牌。</span><span class="sxs-lookup"><span data-stu-id="35b4c-195">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span>|
|<span data-ttu-id="35b4c-196">查询</span><span class="sxs-lookup"><span data-stu-id="35b4c-196">query</span></span>|<span data-ttu-id="35b4c-197">代码或令牌作为查询参数返回。</span><span class="sxs-lookup"><span data-stu-id="35b4c-197">The code or token is returned as a query parameter.</span></span>|

### <a name="responsetype-value"></a><span data-ttu-id="35b4c-198">responseType 值</span><span class="sxs-lookup"><span data-stu-id="35b4c-198">responseType value</span></span>
|<span data-ttu-id="35b4c-199">值</span><span class="sxs-lookup"><span data-stu-id="35b4c-199">Value</span></span>|<span data-ttu-id="35b4c-200">说明</span><span class="sxs-lookup"><span data-stu-id="35b4c-200">Description</span></span>|
:--------|:----------|
|<span data-ttu-id="35b4c-201">code</span><span class="sxs-lookup"><span data-stu-id="35b4c-201">code</span></span>|<span data-ttu-id="35b4c-202">根据授权代码流，代码将返回到 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="35b4c-202">As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="35b4c-203">Azure AD B2C 继续调用 token_endpoint 以交换令牌代码。</span><span class="sxs-lookup"><span data-stu-id="35b4c-203">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span>|
|<span data-ttu-id="35b4c-204">id_token</span><span class="sxs-lookup"><span data-stu-id="35b4c-204">id_token</span></span>|<span data-ttu-id="35b4c-205">ID 令牌从自定义标识提供程序返回回 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="35b4c-205">An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span>|
|<span data-ttu-id="35b4c-206">令牌</span><span class="sxs-lookup"><span data-stu-id="35b4c-206">token</span></span>|<span data-ttu-id="35b4c-207">访问令牌从自定义标识提供程序返回回 Azure AD B2C。</span><span class="sxs-lookup"><span data-stu-id="35b4c-207">An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="35b4c-208"> (当前 Azure AD B2C 不支持) </span><span class="sxs-lookup"><span data-stu-id="35b4c-208">(This value is not supported by Azure AD B2C at the moment)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35b4c-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35b4c-209">JSON representation</span></span>

<span data-ttu-id="35b4c-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35b4c-210">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```json
{
  "id": "String",
  "displayName": "String",
  "clientId": "String",
  "clientSecret": "String",
  "claimsMapping": {
      "@odata.type": "#microsoft.graph.claimsMapping",
      "userId": "String",
      "givenName": "String",
      "surname": "String",
      "email": "String",
      "displayName": "String"
  },
  "domainHint": "String",
  "metadataUrl": "String",
  "responseMode": "String",
  "responseType": "String",
  "scope": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "openidconnectIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
