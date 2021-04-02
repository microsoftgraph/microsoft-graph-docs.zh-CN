---
title: builtInIdentityProvider 资源类型
description: 表示 Azure Active Directory 租户中的内置标识提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 5c806306e596a087a6c4006dc39b1804c130858a
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491098"
---
# <a name="builtinidentityprovider-resource-type"></a><span data-ttu-id="d1130-103">builtInIdentityProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1130-103">builtInIdentityProvider resource type</span></span>
<span data-ttu-id="d1130-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1130-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1130-105">表示具有 Azure Active Directory [租户](/azure/active-directory/external-identities/) 标识的内置标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="d1130-105">Represents built-in identity providers with [External Identities](/azure/active-directory/external-identities/) for an Azure Active Directory tenant.</span></span>

<span data-ttu-id="d1130-106">对于 Azure AD 租户中的 Azure AD B2B 方案，内置标识提供程序类型可以是 Azure Active Directory （AAD）、Microsoft 帐户（MSA）或电子邮件一次密码 （EmailOTP）。</span><span class="sxs-lookup"><span data-stu-id="d1130-106">For Azure AD B2B scenarios in an Azure AD tenant, the built in identity provider type can be an Azure Active Directory(AAD), Microsoft account(MSA) or email one-time passcode (EmailOTP).</span></span>

<span data-ttu-id="d1130-107">此类型将从 [identityProviderBase](../resources/identityproviderbase.md)。</span><span class="sxs-lookup"><span data-stu-id="d1130-107">This type will inherit from [identityProviderBase](../resources/identityproviderbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d1130-108">方法</span><span class="sxs-lookup"><span data-stu-id="d1130-108">Methods</span></span>

| <span data-ttu-id="d1130-109">方法</span><span class="sxs-lookup"><span data-stu-id="d1130-109">Method</span></span>       | <span data-ttu-id="d1130-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d1130-110">Return Type</span></span>  |<span data-ttu-id="d1130-111">Description</span><span class="sxs-lookup"><span data-stu-id="d1130-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d1130-112">List</span><span class="sxs-lookup"><span data-stu-id="d1130-112">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="d1130-113">[identityProviderBase](../resources/identityproviderbase.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d1130-113">[identityProviderBase](../resources/identityproviderbase.md) collection</span></span>|<span data-ttu-id="d1130-114">检索租户中配置的所有标识提供程序，包括内置标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="d1130-114">Retrieve all identity providers configured in a tenant including the built-in identity providers.</span></span>|
|[<span data-ttu-id="d1130-115">Get</span><span class="sxs-lookup"><span data-stu-id="d1130-115">Get</span></span>](../api/identityproviderbase-get.md) |<span data-ttu-id="d1130-116">builtInIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="d1130-116">builtInIdentityProvider</span></span>|<span data-ttu-id="d1130-117">检索内置标识提供程序的属性。</span><span class="sxs-lookup"><span data-stu-id="d1130-117">Retrieve properties of an built-in identity provider.</span></span>|
|[<span data-ttu-id="d1130-118">列出可用的提供程序类型</span><span class="sxs-lookup"><span data-stu-id="d1130-118">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="d1130-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="d1130-119">String collection</span></span>|<span data-ttu-id="d1130-120">检索租户中所有可用的标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="d1130-120">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="d1130-121">属性</span><span class="sxs-lookup"><span data-stu-id="d1130-121">Properties</span></span>

|<span data-ttu-id="d1130-122">属性</span><span class="sxs-lookup"><span data-stu-id="d1130-122">Property</span></span>|<span data-ttu-id="d1130-123">类型</span><span class="sxs-lookup"><span data-stu-id="d1130-123">Type</span></span>|<span data-ttu-id="d1130-124">说明</span><span class="sxs-lookup"><span data-stu-id="d1130-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1130-125">id</span><span class="sxs-lookup"><span data-stu-id="d1130-125">id</span></span>|<span data-ttu-id="d1130-126">String</span><span class="sxs-lookup"><span data-stu-id="d1130-126">String</span></span>|<span data-ttu-id="d1130-127">标识提供程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="d1130-127">The identifier of the identity provider.</span></span> <span data-ttu-id="d1130-128">继承自 [identityProviderBase](../resources/identityproviderbase.md)。</span><span class="sxs-lookup"><span data-stu-id="d1130-128">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span> <span data-ttu-id="d1130-129">只读。</span><span class="sxs-lookup"><span data-stu-id="d1130-129">Read-only.</span></span>|
|<span data-ttu-id="d1130-130">displayName</span><span class="sxs-lookup"><span data-stu-id="d1130-130">displayName</span></span>|<span data-ttu-id="d1130-131">字符串</span><span class="sxs-lookup"><span data-stu-id="d1130-131">String</span></span>|<span data-ttu-id="d1130-132">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d1130-132">The display name of the identity provider.</span></span> <span data-ttu-id="d1130-133">继承自 [identityProviderBase](../resources/identityproviderbase.md)。</span><span class="sxs-lookup"><span data-stu-id="d1130-133">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span>|
|<span data-ttu-id="d1130-134">identityProviderType</span><span class="sxs-lookup"><span data-stu-id="d1130-134">identityProviderType</span></span>|<span data-ttu-id="d1130-135">字符串</span><span class="sxs-lookup"><span data-stu-id="d1130-135">String</span></span>|<span data-ttu-id="d1130-136">标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="d1130-136">The identity provider type.</span></span> <span data-ttu-id="d1130-137">对于 B2B 方案，可能的值： `AADSignup`、 `MicrosoftAccount`、 `EmailOTP`。</span><span class="sxs-lookup"><span data-stu-id="d1130-137">For a B2B scenario, possible values: `AADSignup`, `MicrosoftAccount`, `EmailOTP`.</span></span> <span data-ttu-id="d1130-138">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="d1130-138">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1130-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1130-139">JSON representation</span></span>

<span data-ttu-id="d1130-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1130-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.builtInIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "builtinIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
