---
title: b2xIdentityUserFlow 资源类型
description: 表示 Azure Active Directory 租户内的用户流。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: f20e02c5f75e4133beb40315bcc4b6fc3b0712c1
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705819"
---
# <a name="b2xidentityuserflow-resource-type"></a><span data-ttu-id="a444d-103">b2xIdentityUserFlow 资源类型</span><span class="sxs-lookup"><span data-stu-id="a444d-103">b2xIdentityUserFlow resource type</span></span>

<span data-ttu-id="a444d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a444d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a444d-105">表示 Azure Active Directory 租户内的用户流。</span><span class="sxs-lookup"><span data-stu-id="a444d-105">Represents a user flow within an Azure Active Directory tenant.</span></span>

<span data-ttu-id="a444d-106">用户流用于在应用程序上为来宾用户提供[自助注册](/azure/active-directory/external-identities/self-service-sign-up-overview)体验。</span><span class="sxs-lookup"><span data-stu-id="a444d-106">User flows are used to enable a [self-service sign up](/azure/active-directory/external-identities/self-service-sign-up-overview) experience for guest users on an application.</span></span> <span data-ttu-id="a444d-107">用户流定义最终用户注册时的体验，包括他们可以使用哪些[标识提供者](/azure/active-directory/external-identities/identity-providers)进行验证，以及在注册过程中收集哪些属性。</span><span class="sxs-lookup"><span data-stu-id="a444d-107">User flows define the experience the end user sees while signing up, including which [identity providers](/azure/active-directory/external-identities/identity-providers) they can use to authenticate, along with which attributes are collected as part of the sign up process.</span></span>

## <a name="methods"></a><span data-ttu-id="a444d-108">方法</span><span class="sxs-lookup"><span data-stu-id="a444d-108">Methods</span></span>

| <span data-ttu-id="a444d-109">方法</span><span class="sxs-lookup"><span data-stu-id="a444d-109">Method</span></span>       | <span data-ttu-id="a444d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a444d-110">Return Type</span></span>  |<span data-ttu-id="a444d-111">说明</span><span class="sxs-lookup"><span data-stu-id="a444d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a444d-112">列出用户流</span><span class="sxs-lookup"><span data-stu-id="a444d-112">List user flows</span></span>](../api/identitycontainer-list-b2xuserflows.md)|<span data-ttu-id="a444d-113">b2xIdentityUserFlow 集合</span><span class="sxs-lookup"><span data-stu-id="a444d-113">b2xIdentityUserFlow collection</span></span>|<span data-ttu-id="a444d-114">检索所有 B2X 用户流。</span><span class="sxs-lookup"><span data-stu-id="a444d-114">Retrieve all B2X user flows.</span></span>|
|[<span data-ttu-id="a444d-115">获取用户流</span><span class="sxs-lookup"><span data-stu-id="a444d-115">Get user flow</span></span>](../api/b2xidentityuserflow-get.md)|<span data-ttu-id="a444d-116">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="a444d-116">b2xIdentityUserFlow</span></span>|<span data-ttu-id="a444d-117">检索 B2X 用户流的属性。</span><span class="sxs-lookup"><span data-stu-id="a444d-117">Retrieve properties of a B2X user flow.</span></span>|
|[<span data-ttu-id="a444d-118">创建用户流</span><span class="sxs-lookup"><span data-stu-id="a444d-118">Create user flow</span></span>](../api/identitycontainer-post-b2xuserflows.md)|<span data-ttu-id="a444d-119">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="a444d-119">b2xIdentityUserFlow</span></span>|<span data-ttu-id="a444d-120">新建 B2X 用户流。</span><span class="sxs-lookup"><span data-stu-id="a444d-120">Create a new B2X user flow.</span></span>|
|[<span data-ttu-id="a444d-121">删除用户流</span><span class="sxs-lookup"><span data-stu-id="a444d-121">Delete user flow</span></span>](../api/b2xidentityuserflow-delete.md)|<span data-ttu-id="a444d-122">无</span><span class="sxs-lookup"><span data-stu-id="a444d-122">None</span></span>|<span data-ttu-id="a444d-123">删除 B2X 用户流。</span><span class="sxs-lookup"><span data-stu-id="a444d-123">Delete a B2X user flow.</span></span>|
|[<span data-ttu-id="a444d-124">列出标识提供者</span><span class="sxs-lookup"><span data-stu-id="a444d-124">List identity providers</span></span>](../api/b2xidentityuserflow-list-identityproviders.md)|<span data-ttu-id="a444d-125">[identityProvider](../resources/identityProvider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="a444d-125">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="a444d-126">检索 B2X 用户流中的所有标识提供者。</span><span class="sxs-lookup"><span data-stu-id="a444d-126">Retrieve all identity providers in a B2X user flow.</span></span>|
|[<span data-ttu-id="a444d-127">添加标识提供者</span><span class="sxs-lookup"><span data-stu-id="a444d-127">Add identity provider</span></span>](../api/b2xidentityuserflow-post-identityproviders.md)|<span data-ttu-id="a444d-128">无</span><span class="sxs-lookup"><span data-stu-id="a444d-128">None</span></span>|<span data-ttu-id="a444d-129">向 B2X 用户流添加标识提供者。</span><span class="sxs-lookup"><span data-stu-id="a444d-129">Add an identity provider to a B2X user flow.</span></span>|
|[<span data-ttu-id="a444d-130">删除标识提供者</span><span class="sxs-lookup"><span data-stu-id="a444d-130">Remove identity provider</span></span>](../api/b2xidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="a444d-131">无</span><span class="sxs-lookup"><span data-stu-id="a444d-131">None</span></span>|<span data-ttu-id="a444d-132">从 B2X 用户流中删除标识提供者。</span><span class="sxs-lookup"><span data-stu-id="a444d-132">Remove an identity provider from a B2X user flow.</span></span>|
|[<span data-ttu-id="a444d-133">列出用户属性作业</span><span class="sxs-lookup"><span data-stu-id="a444d-133">List user attribute assignments</span></span>](../api/b2xidentityuserflow-list-userattributeassignments.md)|<span data-ttu-id="a444d-134">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a444d-134">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="a444d-135">从 B2C 用户流中检索所有用户属性作业。</span><span class="sxs-lookup"><span data-stu-id="a444d-135">Retrieve all user attribute assignments in a B2X user flow.</span></span>|
|[<span data-ttu-id="a444d-136">创建用户属性作业</span><span class="sxs-lookup"><span data-stu-id="a444d-136">Create user attribute assignment</span></span>](../api/b2xidentityuserflow-post-userattributeassignments.md)|[<span data-ttu-id="a444d-137">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="a444d-137">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="a444d-138">在 B2C 用户流中创建一个用户属性作业。</span><span class="sxs-lookup"><span data-stu-id="a444d-138">Create a user attribute assignment in a B2X user flow.</span></span>|
|[<span data-ttu-id="a444d-139">列表语言</span><span class="sxs-lookup"><span data-stu-id="a444d-139">List languages</span></span>](../api/b2xidentityuserflow-list-languages.md)|<span data-ttu-id="a444d-140">[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a444d-140">[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) collection</span></span>|<span data-ttu-id="a444d-141">检索 B2X 用户流中的所有语言。</span><span class="sxs-lookup"><span data-stu-id="a444d-141">Retrieve all languages within a B2X user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="a444d-142">属性</span><span class="sxs-lookup"><span data-stu-id="a444d-142">Properties</span></span>

|<span data-ttu-id="a444d-143">属性</span><span class="sxs-lookup"><span data-stu-id="a444d-143">Property</span></span>|<span data-ttu-id="a444d-144">类型</span><span class="sxs-lookup"><span data-stu-id="a444d-144">Type</span></span>|<span data-ttu-id="a444d-145">说明</span><span class="sxs-lookup"><span data-stu-id="a444d-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a444d-146">id</span><span class="sxs-lookup"><span data-stu-id="a444d-146">id</span></span>|<span data-ttu-id="a444d-147">String</span><span class="sxs-lookup"><span data-stu-id="a444d-147">String</span></span>|<span data-ttu-id="a444d-148">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="a444d-148">The name of the user flow.</span></span> <span data-ttu-id="a444d-149">这是一个必需的值且在创建之后不可变。</span><span class="sxs-lookup"><span data-stu-id="a444d-149">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="a444d-150">创建后，该名称将以 `B2X_1_` 的值作为前缀。</span><span class="sxs-lookup"><span data-stu-id="a444d-150">The name will be prefixed with the value of `B2X_1_` after creation.</span></span>|
|<span data-ttu-id="a444d-151">userFlowType</span><span class="sxs-lookup"><span data-stu-id="a444d-151">userFlowType</span></span>|<span data-ttu-id="a444d-152">userFlowType</span><span class="sxs-lookup"><span data-stu-id="a444d-152">userFlowType</span></span>|<span data-ttu-id="a444d-153">用户流类型。</span><span class="sxs-lookup"><span data-stu-id="a444d-153">The type of user flow.</span></span> <span data-ttu-id="a444d-154">对于自助注册用户流，该值在创建后只能 `signUpOrSignIn`，不能修改。</span><span class="sxs-lookup"><span data-stu-id="a444d-154">For self-service sign up user flows, the value can only be `signUpOrSignIn` and cannot be modified after creation.</span></span>|
|<span data-ttu-id="a444d-155">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="a444d-155">userFlowTypeVersion</span></span>|<span data-ttu-id="a444d-156">单一</span><span class="sxs-lookup"><span data-stu-id="a444d-156">Single</span></span>|<span data-ttu-id="a444d-157">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="a444d-157">The version of the user flow.</span></span> <span data-ttu-id="a444d-158">对于 B2X 用户流，版本始终是`1`</span><span class="sxs-lookup"><span data-stu-id="a444d-158">For B2X user flows, the version is always `1`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a444d-159">关系</span><span class="sxs-lookup"><span data-stu-id="a444d-159">Relationships</span></span>

| <span data-ttu-id="a444d-160">关系</span><span class="sxs-lookup"><span data-stu-id="a444d-160">Relationship</span></span>       | <span data-ttu-id="a444d-161">类型</span><span class="sxs-lookup"><span data-stu-id="a444d-161">Type</span></span>  |<span data-ttu-id="a444d-162">说明</span><span class="sxs-lookup"><span data-stu-id="a444d-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a444d-163">identityProviders</span><span class="sxs-lookup"><span data-stu-id="a444d-163">identityProviders</span></span>|<span data-ttu-id="a444d-164">[identityProvider](../resources/identityprovider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="a444d-164">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="a444d-165">用户流中包含的标识提供者。</span><span class="sxs-lookup"><span data-stu-id="a444d-165">The identity providers included in the user flow.</span></span>|
|<span data-ttu-id="a444d-166">userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="a444d-166">userAttributeAssignments</span></span>|<span data-ttu-id="a444d-167">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a444d-167">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="a444d-168">包含在用户流内的用户属性作业。</span><span class="sxs-lookup"><span data-stu-id="a444d-168">The user attribute assignments included in the user flow.</span></span>|
|<span data-ttu-id="a444d-169">languages</span><span class="sxs-lookup"><span data-stu-id="a444d-169">languages</span></span>|<span data-ttu-id="a444d-170">[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a444d-170">[userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) collection</span></span>|<span data-ttu-id="a444d-171">用户流中的自定义项所支持语言。</span><span class="sxs-lookup"><span data-stu-id="a444d-171">The languages supported for customization within the user flow.</span></span> <span data-ttu-id="a444d-172">默认情况下，将在 B2X 用户流中启用语言自定义项。</span><span class="sxs-lookup"><span data-stu-id="a444d-172">Language customization is enabled by default in B2X user flow.</span></span> <span data-ttu-id="a444d-173">无法在 B2X 用户流中创建自定义语言。</span><span class="sxs-lookup"><span data-stu-id="a444d-173">You cannot create custom languages in B2X user flows.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a444d-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a444d-174">JSON representation</span></span>

<span data-ttu-id="a444d-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a444d-175">The following is a JSON representation of the resource.</span></span>

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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}],
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}],
    "languages": [{"@odata.type": "microsoft.graph.userFlowLanguageConfiguration"}]
}
```
