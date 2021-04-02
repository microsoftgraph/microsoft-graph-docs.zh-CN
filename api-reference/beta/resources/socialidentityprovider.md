---
title: socialIdentityProvider 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的社交标识提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 58e08852c99c97648447e7d0acf9946ea3227122
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491090"
---
# <a name="socialidentityprovider-resource-type"></a><span data-ttu-id="d9fe5-103">socialIdentityProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9fe5-103">socialIdentityProvider resource type</span></span>
<span data-ttu-id="d9fe5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9fe5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9fe5-105">对 Azure Active Directory 租户和 Azure AD B2C 租户都标识具有[外部标识](/azure/active-directory/external-identities/)的身份提供程序。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-105">Represents social identity providers with [External Identities](/azure/active-directory/external-identities/) for both Azure Active Directory tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="d9fe5-106">此类型将从 [identityProviderBase](../resources/identityproviderbase.md)。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-106">This type will inherit from [identityProviderBase](../resources/identityproviderbase.md).</span></span>

<span data-ttu-id="d9fe5-107">对于 Azure AD 租户中的 Azure AD B2B 方案，身份提供程序类型可以是 Google 或 Facebook。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-107">For Azure AD B2B scenarios in an Azure AD tenant, the identity provider type can be Google or Facebook.</span></span>

<span data-ttu-id="d9fe5-108">通过在 Azure AD B2C 中配置身份提供程序，可实现新 Azure AD B2B 来宾方案。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-108">Configuring an identity provider in your Azure AD tenant enables new Azure AD B2B guest scenarios.</span></span> <span data-ttu-id="d9fe5-109">例如，某组织在 Microsoft 365 中具有需要与 Gmail 用户共享的资源。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-109">For example, an organization has resources in Microsoft 365 that need to be shared with a Gmail user.</span></span> <span data-ttu-id="d9fe5-110">Gmail 将使用其 Google 帐户凭据来验证和访问文档。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-110">The Gmail user will use their Google account credentials to authenticate and access the documents.</span></span>

<span data-ttu-id="d9fe5-111">在 Azure AD B2C 租户中，标识提供程序类型可以是 Microsoft、Google、Facebook、Amazon、LinkedIn或 Twitter。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-111">In an Azure AD B2C tenant, the identity provider type can be Microsoft, Google, Facebook, Amazon, LinkedIn or Twitter.</span></span> <span data-ttu-id="d9fe5-112">以下身份提供程序正处于预览阶段：微博、QQ、微信和 GitHub。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-112">The following identity providers are in preview: Weibo, QQ, WeChat, and GitHub.</span></span>

<span data-ttu-id="d9fe5-113">在 Azure AD B2C 租户中配置标识提供程序使用户可以在应用程序中使用支持的社交帐户提供程序进行注册和登录。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-113">Configuring an identity provider in your Azure AD B2C tenant enables users to sign up and sign in using a social account supported provider in an application.</span></span> <span data-ttu-id="d9fe5-114">例如，应用程序可使用 Azure AD B2C 让用户能够通过 Facebook 帐户注册服务。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-114">For example, an application can use Azure AD B2C to allow users to sign up for the service using a Facebook account.</span></span>

## <a name="methods"></a><span data-ttu-id="d9fe5-115">方法</span><span class="sxs-lookup"><span data-stu-id="d9fe5-115">Methods</span></span>

| <span data-ttu-id="d9fe5-116">方法</span><span class="sxs-lookup"><span data-stu-id="d9fe5-116">Method</span></span>       | <span data-ttu-id="d9fe5-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9fe5-117">Return Type</span></span>  |<span data-ttu-id="d9fe5-118">Description</span><span class="sxs-lookup"><span data-stu-id="d9fe5-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d9fe5-119">List</span><span class="sxs-lookup"><span data-stu-id="d9fe5-119">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="d9fe5-120">[identityProviderBase](../resources/identityproviderbase.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9fe5-120">[identityProviderBase](../resources/identityproviderbase.md) collection</span></span>|<span data-ttu-id="d9fe5-121">检索租户中配置的所有标识提供程序，包括社交标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-121">Retrieve all identity providers configured in a tenant including the social identity providers.</span></span>|
|[<span data-ttu-id="d9fe5-122">Create</span><span class="sxs-lookup"><span data-stu-id="d9fe5-122">Create</span></span>](../api/identityproviderbase-post-identityproviders.md)|<span data-ttu-id="d9fe5-123">socialidentityprovider</span><span class="sxs-lookup"><span data-stu-id="d9fe5-123">socialidentityprovider</span></span> |<span data-ttu-id="d9fe5-124">创建新的社交标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-124">Create a new social identity provider.</span></span>|
|[<span data-ttu-id="d9fe5-125">Get</span><span class="sxs-lookup"><span data-stu-id="d9fe5-125">Get</span></span>](../api/identityproviderbase-get.md) |<span data-ttu-id="d9fe5-126">socialidentityprovider</span><span class="sxs-lookup"><span data-stu-id="d9fe5-126">socialidentityprovider</span></span> |<span data-ttu-id="d9fe5-127">检索社交身份提供程序的属性。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-127">Retrieve properties of a social identity provider.</span></span>|
|[<span data-ttu-id="d9fe5-128">更新</span><span class="sxs-lookup"><span data-stu-id="d9fe5-128">Update</span></span>](../api/identityproviderbase-update.md)|<span data-ttu-id="d9fe5-129">无</span><span class="sxs-lookup"><span data-stu-id="d9fe5-129">None</span></span>|<span data-ttu-id="d9fe5-130">更新社交标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-130">Update a social identity provider.</span></span>|
|[<span data-ttu-id="d9fe5-131">删除</span><span class="sxs-lookup"><span data-stu-id="d9fe5-131">Delete</span></span>](../api/identityproviderbase-delete.md)|<span data-ttu-id="d9fe5-132">无</span><span class="sxs-lookup"><span data-stu-id="d9fe5-132">None</span></span>|<span data-ttu-id="d9fe5-133">删除社交标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-133">Delete a social  identity provider.</span></span>|
|[<span data-ttu-id="d9fe5-134">列出可用的提供程序类型</span><span class="sxs-lookup"><span data-stu-id="d9fe5-134">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="d9fe5-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="d9fe5-135">String collection</span></span>|<span data-ttu-id="d9fe5-136">检索租户中所有可用的标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-136">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9fe5-137">属性</span><span class="sxs-lookup"><span data-stu-id="d9fe5-137">Properties</span></span>

|<span data-ttu-id="d9fe5-138">属性</span><span class="sxs-lookup"><span data-stu-id="d9fe5-138">Property</span></span>|<span data-ttu-id="d9fe5-139">类型</span><span class="sxs-lookup"><span data-stu-id="d9fe5-139">Type</span></span>|<span data-ttu-id="d9fe5-140">说明</span><span class="sxs-lookup"><span data-stu-id="d9fe5-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9fe5-141">clientId</span><span class="sxs-lookup"><span data-stu-id="d9fe5-141">clientId</span></span>|<span data-ttu-id="d9fe5-142">字符串</span><span class="sxs-lookup"><span data-stu-id="d9fe5-142">String</span></span>|<span data-ttu-id="d9fe5-143">向标识提供程序注册应用程序时，获取应用程序的客户端标识符。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-143">The client identifier for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="d9fe5-144">必填。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-144">Required.</span></span>|
|<span data-ttu-id="d9fe5-145">clientSecret</span><span class="sxs-lookup"><span data-stu-id="d9fe5-145">clientSecret</span></span>|<span data-ttu-id="d9fe5-146">字符串</span><span class="sxs-lookup"><span data-stu-id="d9fe5-146">String</span></span>|<span data-ttu-id="d9fe5-147">向标识提供程序注册时获取的应用程序的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-147">The client secret for the application that is obtained when the application is registered with the identity provider.</span></span> <span data-ttu-id="d9fe5-148">这是只读的。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-148">This is write-only.</span></span> <span data-ttu-id="d9fe5-149">读取操作返回"\*\*\*\*"。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-149">A read operation returns "\*\*\*\*".</span></span> <span data-ttu-id="d9fe5-150">必需。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-150">Required.</span></span>|
|<span data-ttu-id="d9fe5-151">id</span><span class="sxs-lookup"><span data-stu-id="d9fe5-151">id</span></span>|<span data-ttu-id="d9fe5-152">String</span><span class="sxs-lookup"><span data-stu-id="d9fe5-152">String</span></span>|<span data-ttu-id="d9fe5-153">标识提供程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-153">The identifier of the identity provider.</span></span> <span data-ttu-id="d9fe5-154">继承自 [identityProviderBase](../resources/identityproviderbase.md)。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-154">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span> <span data-ttu-id="d9fe5-155">只读。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-155">Read-only.</span></span>|
|<span data-ttu-id="d9fe5-156">displayName</span><span class="sxs-lookup"><span data-stu-id="d9fe5-156">displayName</span></span>|<span data-ttu-id="d9fe5-157">字符串</span><span class="sxs-lookup"><span data-stu-id="d9fe5-157">String</span></span>|<span data-ttu-id="d9fe5-158">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-158">The display name of the identity provider.</span></span> <span data-ttu-id="d9fe5-159">继承自 [identityProviderBase](../resources/identityproviderbase.md)。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-159">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span>|
|<span data-ttu-id="d9fe5-160">identityProviderType</span><span class="sxs-lookup"><span data-stu-id="d9fe5-160">identityProviderType</span></span>|<span data-ttu-id="d9fe5-161">String</span><span class="sxs-lookup"><span data-stu-id="d9fe5-161">String</span></span>|<span data-ttu-id="d9fe5-162">对于 B2B 方案，可能的值为： `Google`、 `Facebook`。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-162">For a B2B scenario, possible values: `Google`, `Facebook`.</span></span> <span data-ttu-id="d9fe5-163">对于 B2C 方案，可能的值： `Microsoft`、 `Google`、 `Amazon`、 `LinkedIn`、 `Facebook`、 `GitHub`、 `Twitter`、 `Weibo`、 `QQ`、 `WeChat`。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-163">For a B2C scenario, possible values: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.</span></span> <span data-ttu-id="d9fe5-164">必填。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-164">Required.</span></span>|

### <a name="where-to-get-the-client-identifier-and-secret"></a><span data-ttu-id="d9fe5-165">在何处获取客户端标识符和密码</span><span class="sxs-lookup"><span data-stu-id="d9fe5-165">Where to get the client identifier and secret</span></span>

<span data-ttu-id="d9fe5-166">每个标识提供程序都有一个用于创建应用注册的进程。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-166">Each identity provider has a process for creating an app registration.</span></span> <span data-ttu-id="d9fe5-167">例如，用户在 [developers.facebook.com](https://developers.facebook.com/) 处向 Facebook 创建一个应用注册。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-167">For example, users create an app registration with Facebook at [developers.facebook.com](https://developers.facebook.com/).</span></span> <span data-ttu-id="d9fe5-168">生成的客户端 ID 和客户端密码可传递用于[创建 identityProvider](../api/identityproviderbase-post-identityproviders.md)。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-168">The resulting client identifier and client secret can be passed to [create identityProvider](../api/identityproviderbase-post-identityproviders.md).</span></span> <span data-ttu-id="d9fe5-169">然后，目录中的每个用户对象都可联合到租户的任意标识提供程序中进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-169">Then, each user object in the directory can be federated to any of the tenant's identity providers for authentication.</span></span> <span data-ttu-id="d9fe5-170">这样，用户即可通过在标识提供程序的登录页面上输入评估凭据来进行登录。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-170">This enables the user to sign in by entering credentials on the identity provider's sign-in page.</span></span> <span data-ttu-id="d9fe5-171">来自标识提供程序的令牌先由 Azure AD 进行验证，然后租户再向应用程序发出一个令牌。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-171">The token from the identity provider is validated by Azure AD before the tenant issues a token to the application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9fe5-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9fe5-172">JSON representation</span></span>

<span data-ttu-id="d9fe5-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9fe5-173">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "socialIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
