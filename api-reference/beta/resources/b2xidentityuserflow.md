---
title: b2xIdentityUserFlow 资源类型
description: 表示 Azure Active Directory 租户内的用户流。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 85839539ae78963114ea7a9eaeac49307166a9ff
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406359"
---
# <a name="b2xidentityuserflow-resource-type"></a><span data-ttu-id="bcd47-103">b2xIdentityUserFlow 资源类型</span><span class="sxs-lookup"><span data-stu-id="bcd47-103">b2xIdentityUserFlow resource type</span></span>

<span data-ttu-id="bcd47-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcd47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcd47-105">表示 Azure Active Directory 租户内的用户流。</span><span class="sxs-lookup"><span data-stu-id="bcd47-105">Represents a user flow within an Azure Active Directory tenant.</span></span>

<span data-ttu-id="bcd47-106">用户流用于在应用程序上为来宾用户提供[自助注册](/azure/active-directory/external-identities/self-service-sign-up-overview)体验。</span><span class="sxs-lookup"><span data-stu-id="bcd47-106">User flows are used to enable a [self-service sign up](/azure/active-directory/external-identities/self-service-sign-up-overview) experience for guest users on an application.</span></span> <span data-ttu-id="bcd47-107">用户流定义最终用户注册时的体验，包括他们可以使用哪些[标识提供者](/azure/active-directory/external-identities/identity-providers)进行验证，以及在注册过程中收集哪些属性。</span><span class="sxs-lookup"><span data-stu-id="bcd47-107">User flows define the experience the end user sees while signing up, including which [identity providers](/azure/active-directory/external-identities/identity-providers) they can use to authenticate, along with which attributes are collected as part of the sign up process.</span></span>

## <a name="methods"></a><span data-ttu-id="bcd47-108">方法</span><span class="sxs-lookup"><span data-stu-id="bcd47-108">Methods</span></span>

| <span data-ttu-id="bcd47-109">方法</span><span class="sxs-lookup"><span data-stu-id="bcd47-109">Method</span></span>       | <span data-ttu-id="bcd47-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="bcd47-110">Return Type</span></span>  |<span data-ttu-id="bcd47-111">说明</span><span class="sxs-lookup"><span data-stu-id="bcd47-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bcd47-112">列出用户流</span><span class="sxs-lookup"><span data-stu-id="bcd47-112">List user flows</span></span>](../api/identitycontainer-list-b2xuserflows.md)|<span data-ttu-id="bcd47-113">b2xIdentityUserFlow 集合</span><span class="sxs-lookup"><span data-stu-id="bcd47-113">b2xIdentityUserFlow collection</span></span>|<span data-ttu-id="bcd47-114">检索所有 B2X 用户流。</span><span class="sxs-lookup"><span data-stu-id="bcd47-114">Retrieve all B2X user flows.</span></span>|
|[<span data-ttu-id="bcd47-115">获取用户流</span><span class="sxs-lookup"><span data-stu-id="bcd47-115">Get user flow</span></span>](../api/b2xidentityuserflow-get.md)|<span data-ttu-id="bcd47-116">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="bcd47-116">b2xIdentityUserFlow</span></span>|<span data-ttu-id="bcd47-117">检索 B2X 用户流的属性。</span><span class="sxs-lookup"><span data-stu-id="bcd47-117">Retrieve properties of a B2X user flow.</span></span>|
|[<span data-ttu-id="bcd47-118">创建用户流</span><span class="sxs-lookup"><span data-stu-id="bcd47-118">Create user flow</span></span>](../api/identitycontainer-post-b2xuserflows.md)|<span data-ttu-id="bcd47-119">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="bcd47-119">b2xIdentityUserFlow</span></span>|<span data-ttu-id="bcd47-120">新建 B2X 用户流。</span><span class="sxs-lookup"><span data-stu-id="bcd47-120">Create a new B2X user flow.</span></span>|
|[<span data-ttu-id="bcd47-121">删除用户流</span><span class="sxs-lookup"><span data-stu-id="bcd47-121">Delete user flow</span></span>](../api/b2xidentityuserflow-delete.md)|<span data-ttu-id="bcd47-122">无</span><span class="sxs-lookup"><span data-stu-id="bcd47-122">None</span></span>|<span data-ttu-id="bcd47-123">删除 B2X 用户流。</span><span class="sxs-lookup"><span data-stu-id="bcd47-123">Delete a B2X user flow.</span></span>|
|[<span data-ttu-id="bcd47-124">列出标识提供者</span><span class="sxs-lookup"><span data-stu-id="bcd47-124">List identity providers</span></span>](../api/b2xidentityuserflow-list-identityproviders.md)|<span data-ttu-id="bcd47-125">[identityProvider](../resources/identityProvider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="bcd47-125">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="bcd47-126">检索 B2X 用户流中的所有标识提供者。</span><span class="sxs-lookup"><span data-stu-id="bcd47-126">Retrieve all identity providers in a B2X user flow.</span></span>|
|[<span data-ttu-id="bcd47-127">添加标识提供者</span><span class="sxs-lookup"><span data-stu-id="bcd47-127">Add identity provider</span></span>](../api/b2xidentityuserflow-post-identityproviders.md)|<span data-ttu-id="bcd47-128">无</span><span class="sxs-lookup"><span data-stu-id="bcd47-128">None</span></span>|<span data-ttu-id="bcd47-129">向 B2X 用户流添加标识提供者。</span><span class="sxs-lookup"><span data-stu-id="bcd47-129">Add an identity provider to a B2X user flow.</span></span>|
|[<span data-ttu-id="bcd47-130">删除标识提供者</span><span class="sxs-lookup"><span data-stu-id="bcd47-130">Remove identity provider</span></span>](../api/b2xidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="bcd47-131">无</span><span class="sxs-lookup"><span data-stu-id="bcd47-131">None</span></span>|<span data-ttu-id="bcd47-132">从 B2X 用户流中删除标识提供者。</span><span class="sxs-lookup"><span data-stu-id="bcd47-132">Remove an identity provider from a B2X user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="bcd47-133">属性</span><span class="sxs-lookup"><span data-stu-id="bcd47-133">Properties</span></span>

|<span data-ttu-id="bcd47-134">属性</span><span class="sxs-lookup"><span data-stu-id="bcd47-134">Property</span></span>|<span data-ttu-id="bcd47-135">类型</span><span class="sxs-lookup"><span data-stu-id="bcd47-135">Type</span></span>|<span data-ttu-id="bcd47-136">说明</span><span class="sxs-lookup"><span data-stu-id="bcd47-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcd47-137">id</span><span class="sxs-lookup"><span data-stu-id="bcd47-137">id</span></span>|<span data-ttu-id="bcd47-138">String</span><span class="sxs-lookup"><span data-stu-id="bcd47-138">String</span></span>|<span data-ttu-id="bcd47-139">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="bcd47-139">The name of the user flow.</span></span> <span data-ttu-id="bcd47-140">这是一个必需的值且在创建之后不可变。</span><span class="sxs-lookup"><span data-stu-id="bcd47-140">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="bcd47-141">创建后，该名称将以 `B2X_1_` 的值作为前缀。</span><span class="sxs-lookup"><span data-stu-id="bcd47-141">The name will be prefixed with the value of `B2X_1_` after creation.</span></span>|
|<span data-ttu-id="bcd47-142">userFlowType</span><span class="sxs-lookup"><span data-stu-id="bcd47-142">userFlowType</span></span>|<span data-ttu-id="bcd47-143">字符串</span><span class="sxs-lookup"><span data-stu-id="bcd47-143">String</span></span>|<span data-ttu-id="bcd47-144">用户流类型。</span><span class="sxs-lookup"><span data-stu-id="bcd47-144">The type of user flow.</span></span> <span data-ttu-id="bcd47-145">对于自助注册用户流，该值在创建后只能 `signUpOrSignIn`，不能修改。</span><span class="sxs-lookup"><span data-stu-id="bcd47-145">For self-service sign up user flows, the value can only be `signUpOrSignIn` and cannot be modified after creation.</span></span>|
|<span data-ttu-id="bcd47-146">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="bcd47-146">userFlowTypeVersion</span></span>|<span data-ttu-id="bcd47-147">单一</span><span class="sxs-lookup"><span data-stu-id="bcd47-147">Single</span></span>|<span data-ttu-id="bcd47-148">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="bcd47-148">The version of the user flow.</span></span> <span data-ttu-id="bcd47-149">对于 B2X 用户流，版本始终是`1`</span><span class="sxs-lookup"><span data-stu-id="bcd47-149">For B2X user flows, the version is always `1`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcd47-150">关系</span><span class="sxs-lookup"><span data-stu-id="bcd47-150">Relationships</span></span>

| <span data-ttu-id="bcd47-151">关系</span><span class="sxs-lookup"><span data-stu-id="bcd47-151">Relationship</span></span>       | <span data-ttu-id="bcd47-152">类型</span><span class="sxs-lookup"><span data-stu-id="bcd47-152">Type</span></span>  |<span data-ttu-id="bcd47-153">说明</span><span class="sxs-lookup"><span data-stu-id="bcd47-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcd47-154">identityProviders</span><span class="sxs-lookup"><span data-stu-id="bcd47-154">identityProviders</span></span>|<span data-ttu-id="bcd47-155">[identityProvider](../resources/identityprovider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="bcd47-155">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="bcd47-156">用户流中包含的标识提供者。</span><span class="sxs-lookup"><span data-stu-id="bcd47-156">The identity providers included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bcd47-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bcd47-157">JSON representation</span></span>

<span data-ttu-id="bcd47-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcd47-158">The following is a JSON representation of the resource.</span></span>

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