---
title: identityProvider 资源类型
description: 代表 Azure Active Directory 租户和  Azure AD B2C 租户中的身份提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: namkedia
ms.openlocfilehash: 1ab579ce38abea684b4174bee25f2375d722293a
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319573"
---
# <a name="identityprovider-resource-type"></a><span data-ttu-id="3b384-103">identityProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b384-103">identityProvider resource type</span></span>

<span data-ttu-id="3b384-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b384-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b384-105">对 Azure Active Directory 租户和 Azure AD B2C 租户都标识具有[外部标识](https://docs.microsoft.com/azure/active-directory/external-identities/)的身份提供程序。</span><span class="sxs-lookup"><span data-stu-id="3b384-105">Represents identity providers with [External Identities](https://docs.microsoft.com/azure/active-directory/external-identities/) for both Azure Active Directory tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="3b384-106">对于 Azure AD 租户中的 Azure AD B2B 方案，身份提供程序类型可以是 Google 或 Facebook。</span><span class="sxs-lookup"><span data-stu-id="3b384-106">For Azure AD B2B scenarios in an Azure AD tenant, the identity provider type can be Google or Facebook.</span></span>

<span data-ttu-id="3b384-107">通过在 Azure AD B2C 中配置身份提供程序，可实现新 Azure AD B2B 来宾方案。</span><span class="sxs-lookup"><span data-stu-id="3b384-107">Configuring an identity provider in your Azure AD tenant enables new Azure AD B2B guest scenarios.</span></span> <span data-ttu-id="3b384-108">例如，某组织在 Microsoft 365 中具有需要与 Gmail 用户共享的资源。</span><span class="sxs-lookup"><span data-stu-id="3b384-108">For example, an organization has resources in Microsoft 365 that need to be shared with a Gmail user.</span></span> <span data-ttu-id="3b384-109">Gmail 将使用其 Google 帐户凭据来验证和访问文档。</span><span class="sxs-lookup"><span data-stu-id="3b384-109">The Gmail user will use their Google account credentials to authenticate and access the documents.</span></span>

<span data-ttu-id="3b384-110">在 Azure AD B2C 租户中，身份提供程序类型可以是 Microsoft、Google、Facebook、Amazon、LinkedIn、Twitter 或任何 [openIdConnectProvider](../resources/openidconnectprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="3b384-110">In an Azure AD B2C tenant, the identity provider type can be Microsoft, Google, Facebook, Amazon, LinkedIn, Twitter or any [openIdConnectProvider](../resources/openidconnectprovider.md).</span></span> <span data-ttu-id="3b384-111">以下身份提供程序正处于预览阶段：微博、QQ、微信和 GitHub。</span><span class="sxs-lookup"><span data-stu-id="3b384-111">The following identity providers are in preview: Weibo, QQ, WeChat, and GitHub.</span></span>

<span data-ttu-id="3b384-112">在 Azure AD B2C 租户中配置身份提供程序，用户可在应用程序中使用社交帐户或自定义 OpenID Connect 支持的提供程序进行注册和登录。</span><span class="sxs-lookup"><span data-stu-id="3b384-112">Configuring an identity provider in your Azure AD B2C tenant enables users to sign up and sign in using a social account or a custom OpenID Connect supported provider in an application.</span></span> <span data-ttu-id="3b384-113">例如，应用程序可使用 Azure AD B2C 让用户能够通过 Facebook 帐户或他们自己的符合 OIDC 协议的自定义身份提供程序注册服务。</span><span class="sxs-lookup"><span data-stu-id="3b384-113">For example, an application can use Azure AD B2C to allow users to sign up for the service using a Facebook account or their own custom identity provider that complies with OIDC protocol.</span></span>


<span data-ttu-id="3b384-114">如果是具有 `OpenIDConnect` 且为 `type` 的自定义 OpenID Connect 身份提供程序， 则使用 [openIdConnectProvider](../resources/openidconnectprovider.md) 资源类型表示，该资源类型将继承自身份提供程序资源类型。</span><span class="sxs-lookup"><span data-stu-id="3b384-114">If it is a custom OpenID Connect identity provider with `OpenIDConnect` as `type` then it is represented using [openIdConnectProvider](../resources/openidconnectprovider.md) resource type, which will inherit from identityProvider resource type.</span></span> 

## <a name="methods"></a><span data-ttu-id="3b384-115">方法</span><span class="sxs-lookup"><span data-stu-id="3b384-115">Methods</span></span>

| <span data-ttu-id="3b384-116">方法</span><span class="sxs-lookup"><span data-stu-id="3b384-116">Method</span></span>       | <span data-ttu-id="3b384-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="3b384-117">Return Type</span></span>  |<span data-ttu-id="3b384-118">Description</span><span class="sxs-lookup"><span data-stu-id="3b384-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b384-119">List</span><span class="sxs-lookup"><span data-stu-id="3b384-119">List</span></span>](../api/identityprovider-list.md)|<span data-ttu-id="3b384-120">identityProvider 集合</span><span class="sxs-lookup"><span data-stu-id="3b384-120">identityProvider collection</span></span>|<span data-ttu-id="3b384-121">检索在租户中配置的所有标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="3b384-121">Retrieve all identity providers configured in a tenant.</span></span>|
|[<span data-ttu-id="3b384-122">创建</span><span class="sxs-lookup"><span data-stu-id="3b384-122">Create</span></span>](../api/identityprovider-post-identityproviders.md)|<span data-ttu-id="3b384-123">identityProvider</span><span class="sxs-lookup"><span data-stu-id="3b384-123">identityProvider</span></span>|<span data-ttu-id="3b384-124">新建身份提供程序。</span><span class="sxs-lookup"><span data-stu-id="3b384-124">Create a new identity provider.</span></span>|
|[<span data-ttu-id="3b384-125">获取</span><span class="sxs-lookup"><span data-stu-id="3b384-125">Get</span></span>](../api/identityprovider-get.md) |<span data-ttu-id="3b384-126">identityProvider</span><span class="sxs-lookup"><span data-stu-id="3b384-126">identityProvider</span></span>|<span data-ttu-id="3b384-127">检索身份提供程序的属性。</span><span class="sxs-lookup"><span data-stu-id="3b384-127">Retrieve properties of an identity provider.</span></span>|
|[<span data-ttu-id="3b384-128">更新</span><span class="sxs-lookup"><span data-stu-id="3b384-128">Update</span></span>](../api/identityprovider-update.md)|<span data-ttu-id="3b384-129">无</span><span class="sxs-lookup"><span data-stu-id="3b384-129">None</span></span>|<span data-ttu-id="3b384-130">更新身份提供程序。</span><span class="sxs-lookup"><span data-stu-id="3b384-130">Update an identity provider.</span></span>|
|[<span data-ttu-id="3b384-131">删除</span><span class="sxs-lookup"><span data-stu-id="3b384-131">Delete</span></span>](../api/identityprovider-delete.md)|<span data-ttu-id="3b384-132">无</span><span class="sxs-lookup"><span data-stu-id="3b384-132">None</span></span>|<span data-ttu-id="3b384-133">删除身份提供程序。</span><span class="sxs-lookup"><span data-stu-id="3b384-133">Delete an identity provider.</span></span>|
|[<span data-ttu-id="3b384-134">列出可用的提供程序类型</span><span class="sxs-lookup"><span data-stu-id="3b384-134">List available provider types</span></span>](../api/identityprovider-list-availableprovidertypes.md)|<span data-ttu-id="3b384-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="3b384-135">String collection</span></span>|<span data-ttu-id="3b384-136">检索所有可用的身份提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="3b384-136">Retrieve all available identity provider types.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b384-137">属性</span><span class="sxs-lookup"><span data-stu-id="3b384-137">Properties</span></span>

|<span data-ttu-id="3b384-138">属性</span><span class="sxs-lookup"><span data-stu-id="3b384-138">Property</span></span>|<span data-ttu-id="3b384-139">类型</span><span class="sxs-lookup"><span data-stu-id="3b384-139">Type</span></span>|<span data-ttu-id="3b384-140">说明</span><span class="sxs-lookup"><span data-stu-id="3b384-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b384-141">clientId</span><span class="sxs-lookup"><span data-stu-id="3b384-141">clientId</span></span>|<span data-ttu-id="3b384-142">字符串</span><span class="sxs-lookup"><span data-stu-id="3b384-142">String</span></span>|<span data-ttu-id="3b384-143">使用身份提供程序注册应用时获取的应用客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="3b384-143">The client ID for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="3b384-144">这是必填字段。</span><span class="sxs-lookup"><span data-stu-id="3b384-144">This is a required field.</span></span>|
|<span data-ttu-id="3b384-145">clientSecret</span><span class="sxs-lookup"><span data-stu-id="3b384-145">clientSecret</span></span>|<span data-ttu-id="3b384-146">字符串</span><span class="sxs-lookup"><span data-stu-id="3b384-146">String</span></span>|<span data-ttu-id="3b384-147">使用身份提供程序注册应用时获取的应用客户端密码。</span><span class="sxs-lookup"><span data-stu-id="3b384-147">The client secret for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="3b384-148">这是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b384-148">This is write-only.</span></span> <span data-ttu-id="3b384-149">读取操作将返回“\*\*\*\*”。</span><span class="sxs-lookup"><span data-stu-id="3b384-149">A read operation will return "\*\*\*\*".</span></span> <span data-ttu-id="3b384-150">这是必填字段。</span><span class="sxs-lookup"><span data-stu-id="3b384-150">This is a required field.</span></span>|
|<span data-ttu-id="3b384-151">id</span><span class="sxs-lookup"><span data-stu-id="3b384-151">id</span></span>|<span data-ttu-id="3b384-152">字符串</span><span class="sxs-lookup"><span data-stu-id="3b384-152">String</span></span>|<span data-ttu-id="3b384-153">标识提供程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="3b384-153">The ID of the identity provider.</span></span>|
|<span data-ttu-id="3b384-154">name</span><span class="sxs-lookup"><span data-stu-id="3b384-154">name</span></span>|<span data-ttu-id="3b384-155">字符串</span><span class="sxs-lookup"><span data-stu-id="3b384-155">String</span></span>|<span data-ttu-id="3b384-156">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3b384-156">The display name of the identity provider.</span></span>|
|<span data-ttu-id="3b384-157">type</span><span class="sxs-lookup"><span data-stu-id="3b384-157">type</span></span>|<span data-ttu-id="3b384-158">字符串</span><span class="sxs-lookup"><span data-stu-id="3b384-158">String</span></span>|<span data-ttu-id="3b384-159">身份提供程序类型是必填字段。</span><span class="sxs-lookup"><span data-stu-id="3b384-159">The identity provider type is a required field.</span></span><ul><span data-ttu-id="3b384-160">对于 B2B 方案：</span><span class="sxs-lookup"><span data-stu-id="3b384-160">For B2B scenario:</span></span><li/><span data-ttu-id="3b384-161">Google</span><span class="sxs-lookup"><span data-stu-id="3b384-161">Google</span></span><li/><span data-ttu-id="3b384-162">Facebook</span><span class="sxs-lookup"><span data-stu-id="3b384-162">Facebook</span></span></ul><ul><span data-ttu-id="3b384-163">对于 B2C 方案：</span><span class="sxs-lookup"><span data-stu-id="3b384-163">For B2C scenario:</span></span><li/><span data-ttu-id="3b384-164">Microsoft</span><span class="sxs-lookup"><span data-stu-id="3b384-164">Microsoft</span></span><li/><span data-ttu-id="3b384-165">Google</span><span class="sxs-lookup"><span data-stu-id="3b384-165">Google</span></span><li/><span data-ttu-id="3b384-166">Amazon</span><span class="sxs-lookup"><span data-stu-id="3b384-166">Amazon</span></span><li/><span data-ttu-id="3b384-167">领英</span><span class="sxs-lookup"><span data-stu-id="3b384-167">LinkedIn</span></span><li/><span data-ttu-id="3b384-168">Facebook</span><span class="sxs-lookup"><span data-stu-id="3b384-168">Facebook</span></span><li/><span data-ttu-id="3b384-169">GitHub</span><span class="sxs-lookup"><span data-stu-id="3b384-169">GitHub</span></span><li/><span data-ttu-id="3b384-170">Twitter</span><span class="sxs-lookup"><span data-stu-id="3b384-170">Twitter</span></span><li/><span data-ttu-id="3b384-171">微博</span><span class="sxs-lookup"><span data-stu-id="3b384-171">Weibo</span></span><li/><span data-ttu-id="3b384-172">QQ</span><span class="sxs-lookup"><span data-stu-id="3b384-172">QQ</span></span><li/><span data-ttu-id="3b384-173">微信</span><span class="sxs-lookup"><span data-stu-id="3b384-173">WeChat</span></span><li/><span data-ttu-id="3b384-174">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="3b384-174">OpenIDConnect</span></span></ul>|

### <a name="where-to-get-the-client-id-and-secret"></a><span data-ttu-id="3b384-175">获取客户端 ID 和密码的位置</span><span class="sxs-lookup"><span data-stu-id="3b384-175">Where to get the client ID and secret</span></span>

<span data-ttu-id="3b384-176">每个标识提供程序都有一个用于创建应用注册的进程。</span><span class="sxs-lookup"><span data-stu-id="3b384-176">Each identity provider has a process for creating an app registration.</span></span> <span data-ttu-id="3b384-177">例如，用户在 [developers.facebook.com](https://developers.facebook.com/) 处向 Facebook 创建一个应用注册。</span><span class="sxs-lookup"><span data-stu-id="3b384-177">For example, users create an app registration with Facebook at [developers.facebook.com](https://developers.facebook.com/).</span></span> <span data-ttu-id="3b384-178">生成的客户端 ID 和客户端密码可传递用于[创建 identityProvider](../api/identityprovider-post-identityproviders.md)。</span><span class="sxs-lookup"><span data-stu-id="3b384-178">The resulting client ID and client secret can be passed to [create identityProvider](../api/identityprovider-post-identityproviders.md).</span></span> <span data-ttu-id="3b384-179">然后，目录中的每个用户对象都可联合到租户的任意标识提供程序中进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="3b384-179">Then, each user object in the directory can be federated to any of the tenant's identity providers for authentication.</span></span> <span data-ttu-id="3b384-180">这样，用户即可通过在标识提供程序的登录页面上输入评估凭据来进行登录。</span><span class="sxs-lookup"><span data-stu-id="3b384-180">This enables the user to sign in by entering credentials on the identity provider's sign in page.</span></span> <span data-ttu-id="3b384-181">来自标识提供程序的令牌先由 Azure AD 进行验证，然后租户再向应用程序发出一个令牌。</span><span class="sxs-lookup"><span data-stu-id="3b384-181">The token from the identity provider is validated by Azure AD before the tenant issues a token to the application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b384-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b384-182">JSON representation</span></span>

<span data-ttu-id="3b384-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b384-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```json
{
    "id": "String",
    "type": "String",
    "name": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```
