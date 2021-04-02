---
title: identityProviderBase 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的身份提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 1a3d26697c26b803bcbac9141d7ff011575f91f7
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491104"
---
# <a name="identityproviderbase-resource-type"></a><span data-ttu-id="94d39-103">identityProviderBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="94d39-103">identityProviderBase resource type</span></span>
<span data-ttu-id="94d39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94d39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94d39-105">对 Azure Active Directory 租户和 Azure AD B2C 租户都标识具有[外部标识](/azure/active-directory/external-identities/)的身份提供程序。</span><span class="sxs-lookup"><span data-stu-id="94d39-105">Represents identity providers with [External Identities](/azure/active-directory/external-identities/) for both Azure Active Directory tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="94d39-106">对于 Azure AD 目录中的 Azure AD B2B 方案，标识提供程序可以是 [socialIdentityProvider](../resources/socialidentityprovider.md) 或 [builtinIdentityProvider](../resources/builtinidentityprovider.md)，它将从 identityProviderBase 资源类型继承。</span><span class="sxs-lookup"><span data-stu-id="94d39-106">For Azure AD B2B scenarios in an Azure AD directory, the identity provider can be a [socialIdentityProvider](../resources/socialidentityprovider.md) or a [builtinIdentityProvider](../resources/builtinidentityprovider.md), which will inherit from identityProviderBase resource type.</span></span>

<span data-ttu-id="94d39-107">通过在 Azure AD B2C 中配置身份提供程序，可实现新 Azure AD B2B 来宾方案。</span><span class="sxs-lookup"><span data-stu-id="94d39-107">Configuring an identity provider in your Azure AD directory enables new Azure AD B2B guest scenarios.</span></span> <span data-ttu-id="94d39-108">例如，某组织在 Microsoft 365 中具有需要与 Gmail 用户共享的资源。</span><span class="sxs-lookup"><span data-stu-id="94d39-108">For example, an organization has resources in Microsoft 365 that need to be shared with a Gmail user.</span></span> <span data-ttu-id="94d39-109">Gmail 将使用其 Google 帐户凭据来验证和访问文档。</span><span class="sxs-lookup"><span data-stu-id="94d39-109">The Gmail user will use their Google account credentials to authenticate and access the documents.</span></span>

<span data-ttu-id="94d39-110">在 Azure AD B2C 目录中，标识提供程序类型可以是 [socialIdentityProviders](../resources/socialidentityprovider.md)、 [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) 或 [appleIdentityProvider](../resources/appleidentityprovider.md)，它继承身份ProviderBase 资源类型。</span><span class="sxs-lookup"><span data-stu-id="94d39-110">In an Azure AD B2C directory, the identity provider type can be a [socialIdentityProviders](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or [appleIdentityProvider](../resources/appleidentityprovider.md), which will inherit from identityProviderBase resource type.</span></span>

<span data-ttu-id="94d39-111">在 Azure AD B2C 租户中配置身份提供程序，用户可在应用程序中使用社交帐户或自定义 OpenID Connect 支持的提供程序进行注册和登录。</span><span class="sxs-lookup"><span data-stu-id="94d39-111">Configuring an identity provider in your Azure AD B2C directory enables users to sign up and sign in using a social account or a custom OpenID Connect supported provider in an application.</span></span> <span data-ttu-id="94d39-112">例如，应用程序可使用 Azure AD B2C 让用户能够通过 Facebook 帐户或他们自己的符合 OIDC 协议的自定义身份提供程序注册服务。</span><span class="sxs-lookup"><span data-stu-id="94d39-112">For example, an application can use Azure AD B2C to allow users to sign up for the service using a Facebook account or their own custom identity provider that complies with OIDC protocol.</span></span>

## <a name="methods"></a><span data-ttu-id="94d39-113">方法</span><span class="sxs-lookup"><span data-stu-id="94d39-113">Methods</span></span>

| <span data-ttu-id="94d39-114">方法</span><span class="sxs-lookup"><span data-stu-id="94d39-114">Method</span></span>       | <span data-ttu-id="94d39-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="94d39-115">Return Type</span></span>  |<span data-ttu-id="94d39-116">Description</span><span class="sxs-lookup"><span data-stu-id="94d39-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94d39-117">List</span><span class="sxs-lookup"><span data-stu-id="94d39-117">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="94d39-118">identityProviderBase 集合</span><span class="sxs-lookup"><span data-stu-id="94d39-118">identityProviderBase collection</span></span>|<span data-ttu-id="94d39-119">检索在租户中配置的所有标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="94d39-119">Retrieve all identity providers configured in a tenant.</span></span>|
|[<span data-ttu-id="94d39-120">列出可用的提供程序类型</span><span class="sxs-lookup"><span data-stu-id="94d39-120">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="94d39-121">String 集合</span><span class="sxs-lookup"><span data-stu-id="94d39-121">String collection</span></span>|<span data-ttu-id="94d39-122">检索租户中所有可用的标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="94d39-122">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="94d39-123">属性</span><span class="sxs-lookup"><span data-stu-id="94d39-123">Properties</span></span>

|<span data-ttu-id="94d39-124">属性</span><span class="sxs-lookup"><span data-stu-id="94d39-124">Property</span></span>|<span data-ttu-id="94d39-125">类型</span><span class="sxs-lookup"><span data-stu-id="94d39-125">Type</span></span>|<span data-ttu-id="94d39-126">说明</span><span class="sxs-lookup"><span data-stu-id="94d39-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94d39-127">id</span><span class="sxs-lookup"><span data-stu-id="94d39-127">id</span></span>|<span data-ttu-id="94d39-128">String</span><span class="sxs-lookup"><span data-stu-id="94d39-128">String</span></span>|<span data-ttu-id="94d39-129">标识提供程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="94d39-129">The identifier of the identity provider.</span></span>|
|<span data-ttu-id="94d39-130">displayName</span><span class="sxs-lookup"><span data-stu-id="94d39-130">displayName</span></span>|<span data-ttu-id="94d39-131">字符串</span><span class="sxs-lookup"><span data-stu-id="94d39-131">String</span></span>|<span data-ttu-id="94d39-132">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="94d39-132">The display name of the identity provider.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94d39-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94d39-133">JSON representation</span></span>

<span data-ttu-id="94d39-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94d39-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```json
{
    "id": "String",
    "displayName": "String",
}
```
