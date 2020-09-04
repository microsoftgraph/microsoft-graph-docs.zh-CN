---
title: b2xUserFlows 资源类型
description: 表示 Azure Active Directory 租户内的用户流。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 8f25f99ec54f1db6b68bf5617518d90cc51d3ecc
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319690"
---
# <a name="b2xuserflows-resource-type"></a><span data-ttu-id="6b2fa-103">b2xUserFlows 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b2fa-103">b2xUserFlows resource type</span></span>

<span data-ttu-id="6b2fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b2fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b2fa-105">表示 Azure Active Directory 租户内的用户流。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-105">Represents a user flow within an Azure Active Directory tenant.</span></span>

<span data-ttu-id="6b2fa-106">用户流用于在应用程序上为来宾用户提供[自助注册](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview)体验。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-106">User flows are used to enable a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) experience for guest users on an application.</span></span> <span data-ttu-id="6b2fa-107">用户流定义最终用户注册时的体验，包括他们可以使用哪些[标识提供者](https://docs.microsoft.com/azure/active-directory/external-identities/identity-providers)进行验证，以及在注册过程中收集哪些属性。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-107">User flows define the experience the end user sees while signing up, including which [identity providers](https://docs.microsoft.com/azure/active-directory/external-identities/identity-providers) they can use to authenticate, along with which attributes are collected as part of the sign up process.</span></span>

## <a name="methods"></a><span data-ttu-id="6b2fa-108">方法</span><span class="sxs-lookup"><span data-stu-id="6b2fa-108">Methods</span></span>

| <span data-ttu-id="6b2fa-109">方法</span><span class="sxs-lookup"><span data-stu-id="6b2fa-109">Method</span></span>       | <span data-ttu-id="6b2fa-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6b2fa-110">Return Type</span></span>  |<span data-ttu-id="6b2fa-111">说明</span><span class="sxs-lookup"><span data-stu-id="6b2fa-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6b2fa-112">列出用户流</span><span class="sxs-lookup"><span data-stu-id="6b2fa-112">List user flows</span></span>](../api/b2xuserflows-list.md)|<span data-ttu-id="6b2fa-113">b2xUserFlow 集合</span><span class="sxs-lookup"><span data-stu-id="6b2fa-113">b2xUserFlow collection</span></span>|<span data-ttu-id="6b2fa-114">检索所有用户流。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-114">Retrieve all user flows.</span></span>|
|[<span data-ttu-id="6b2fa-115">获取用户流</span><span class="sxs-lookup"><span data-stu-id="6b2fa-115">Get user flow</span></span>](../api/b2xuserflows-get.md)|<span data-ttu-id="6b2fa-116">b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="6b2fa-116">b2xUserFlow</span></span>|<span data-ttu-id="6b2fa-117">检索用户流的属性。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-117">Retrieve properties of a user flow.</span></span>|
|[<span data-ttu-id="6b2fa-118">创建用户流</span><span class="sxs-lookup"><span data-stu-id="6b2fa-118">Create user flow</span></span>](../api/b2xuserflow-post-b2xuserflows.md)|<span data-ttu-id="6b2fa-119">b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="6b2fa-119">b2xUserFlow</span></span>|<span data-ttu-id="6b2fa-120">新建用户流。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-120">Create a new user flow.</span></span>|
|[<span data-ttu-id="6b2fa-121">删除用户流</span><span class="sxs-lookup"><span data-stu-id="6b2fa-121">Delete user flow</span></span>](../api/b2xuserflows-delete.md)|<span data-ttu-id="6b2fa-122">无</span><span class="sxs-lookup"><span data-stu-id="6b2fa-122">None</span></span>|<span data-ttu-id="6b2fa-123">删除用户流。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-123">Delete a user flow.</span></span>|
|[<span data-ttu-id="6b2fa-124">列出标识提供者</span><span class="sxs-lookup"><span data-stu-id="6b2fa-124">List identity providers</span></span>](../api/b2xuserflows-list-identityproviders.md)|<span data-ttu-id="6b2fa-125">[identityProvider](../resources/identityProvider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="6b2fa-125">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="6b2fa-126">检索用户流中的所有标识提供者。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-126">Retrieve all identity providers in a user flow.</span></span>|
|[<span data-ttu-id="6b2fa-127">添加标识提供者</span><span class="sxs-lookup"><span data-stu-id="6b2fa-127">Add identity provider</span></span>](../api/b2xuserflows-update-identityprovider.md)|<span data-ttu-id="6b2fa-128">无</span><span class="sxs-lookup"><span data-stu-id="6b2fa-128">None</span></span>|<span data-ttu-id="6b2fa-129">向用户流添加标识提供者。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-129">Add an identity provider to a user flow.</span></span>|
|[<span data-ttu-id="6b2fa-130">删除标识提供者</span><span class="sxs-lookup"><span data-stu-id="6b2fa-130">Delete identity provider</span></span>](../api/b2xuserflows-delete-identityprovider.md)|<span data-ttu-id="6b2fa-131">无</span><span class="sxs-lookup"><span data-stu-id="6b2fa-131">None</span></span>|<span data-ttu-id="6b2fa-132">从用户流中删除标识提供者。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-132">Delete an identity provider from a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="6b2fa-133">属性</span><span class="sxs-lookup"><span data-stu-id="6b2fa-133">Properties</span></span>

|<span data-ttu-id="6b2fa-134">属性</span><span class="sxs-lookup"><span data-stu-id="6b2fa-134">Property</span></span>|<span data-ttu-id="6b2fa-135">类型</span><span class="sxs-lookup"><span data-stu-id="6b2fa-135">Type</span></span>|<span data-ttu-id="6b2fa-136">说明</span><span class="sxs-lookup"><span data-stu-id="6b2fa-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b2fa-137">id</span><span class="sxs-lookup"><span data-stu-id="6b2fa-137">id</span></span>|<span data-ttu-id="6b2fa-138">String</span><span class="sxs-lookup"><span data-stu-id="6b2fa-138">String</span></span>|<span data-ttu-id="6b2fa-139">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-139">The name of the user flow.</span></span> <span data-ttu-id="6b2fa-140">这是一个必需的值且在创建之后不可变。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-140">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="6b2fa-141">创建后，该名称将以 `B2X_1_` 的值作为前缀。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-141">The name will be prefixed with the value of `B2X_1_` after creation.</span></span>|
|<span data-ttu-id="6b2fa-142">userFlowType</span><span class="sxs-lookup"><span data-stu-id="6b2fa-142">userFlowType</span></span>|<span data-ttu-id="6b2fa-143">字符串</span><span class="sxs-lookup"><span data-stu-id="6b2fa-143">String</span></span>|<span data-ttu-id="6b2fa-144">用户流类型。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-144">The type of user flow.</span></span> <span data-ttu-id="6b2fa-145">对于自助注册用户流，该值在创建后只能 `signUpOrSignIn`，不能修改。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-145">For self-service sign up user flows, the value can only be `signUpOrSignIn` and cannot be modified after creation.</span></span>|
|<span data-ttu-id="6b2fa-146">userFlowVersion</span><span class="sxs-lookup"><span data-stu-id="6b2fa-146">userFlowVersion</span></span>|<span data-ttu-id="6b2fa-147">单一</span><span class="sxs-lookup"><span data-stu-id="6b2fa-147">Single</span></span>|<span data-ttu-id="6b2fa-148">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-148">The version of the user flow.</span></span> <span data-ttu-id="6b2fa-149">对于 B2X 用户流，版本始终是`1`</span><span class="sxs-lookup"><span data-stu-id="6b2fa-149">For B2X user flows, the version is always `1`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b2fa-150">关系</span><span class="sxs-lookup"><span data-stu-id="6b2fa-150">Relationships</span></span>

| <span data-ttu-id="6b2fa-151">关系</span><span class="sxs-lookup"><span data-stu-id="6b2fa-151">Relationship</span></span>       | <span data-ttu-id="6b2fa-152">类型</span><span class="sxs-lookup"><span data-stu-id="6b2fa-152">Type</span></span>  |<span data-ttu-id="6b2fa-153">说明</span><span class="sxs-lookup"><span data-stu-id="6b2fa-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b2fa-154">identityProviders</span><span class="sxs-lookup"><span data-stu-id="6b2fa-154">identityProviders</span></span>|<span data-ttu-id="6b2fa-155">[identityProvider](../resources/identityprovider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="6b2fa-155">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="6b2fa-156">用户流中包含的标识提供者。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-156">The identity providers included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b2fa-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b2fa-157">JSON representation</span></span>

<span data-ttu-id="6b2fa-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b2fa-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "optionalProperties": [],
  "keyProperty": "id"
} -->

```json
{
    "id": "String (identifier)",
    "userFlowType": "String",
    "userFlowTypeVersion": "Single",
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}]
}
```
