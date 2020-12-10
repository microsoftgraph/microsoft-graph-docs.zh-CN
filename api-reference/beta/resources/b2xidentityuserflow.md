---
title: b2xIdentityUserFlow 资源类型
description: 表示 Azure Active Directory 租户内的用户流。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: e1051d60681e42012fd9df3fd8655a9e4cc745cd
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49580961"
---
# <a name="b2xidentityuserflow-resource-type"></a><span data-ttu-id="374b0-103">b2xIdentityUserFlow 资源类型</span><span class="sxs-lookup"><span data-stu-id="374b0-103">b2xIdentityUserFlow resource type</span></span>

<span data-ttu-id="374b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="374b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="374b0-105">表示 Azure Active Directory 租户内的用户流。</span><span class="sxs-lookup"><span data-stu-id="374b0-105">Represents a user flow within an Azure Active Directory tenant.</span></span>

<span data-ttu-id="374b0-106">用户流用于在应用程序上为来宾用户提供[自助注册](/azure/active-directory/external-identities/self-service-sign-up-overview)体验。</span><span class="sxs-lookup"><span data-stu-id="374b0-106">User flows are used to enable a [self-service sign up](/azure/active-directory/external-identities/self-service-sign-up-overview) experience for guest users on an application.</span></span> <span data-ttu-id="374b0-107">用户流定义最终用户注册时的体验，包括他们可以使用哪些[标识提供者](/azure/active-directory/external-identities/identity-providers)进行验证，以及在注册过程中收集哪些属性。</span><span class="sxs-lookup"><span data-stu-id="374b0-107">User flows define the experience the end user sees while signing up, including which [identity providers](/azure/active-directory/external-identities/identity-providers) they can use to authenticate, along with which attributes are collected as part of the sign up process.</span></span>

## <a name="methods"></a><span data-ttu-id="374b0-108">方法</span><span class="sxs-lookup"><span data-stu-id="374b0-108">Methods</span></span>

| <span data-ttu-id="374b0-109">方法</span><span class="sxs-lookup"><span data-stu-id="374b0-109">Method</span></span>       | <span data-ttu-id="374b0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="374b0-110">Return Type</span></span>  |<span data-ttu-id="374b0-111">说明</span><span class="sxs-lookup"><span data-stu-id="374b0-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="374b0-112">列出用户流</span><span class="sxs-lookup"><span data-stu-id="374b0-112">List user flows</span></span>](../api/identitycontainer-list-b2xuserflows.md)|<span data-ttu-id="374b0-113">b2xIdentityUserFlow 集合</span><span class="sxs-lookup"><span data-stu-id="374b0-113">b2xIdentityUserFlow collection</span></span>|<span data-ttu-id="374b0-114">检索所有 B2X 用户流。</span><span class="sxs-lookup"><span data-stu-id="374b0-114">Retrieve all B2X user flows.</span></span>|
|[<span data-ttu-id="374b0-115">获取用户流</span><span class="sxs-lookup"><span data-stu-id="374b0-115">Get user flow</span></span>](../api/b2xidentityuserflow-get.md)|<span data-ttu-id="374b0-116">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="374b0-116">b2xIdentityUserFlow</span></span>|<span data-ttu-id="374b0-117">检索 B2X 用户流的属性。</span><span class="sxs-lookup"><span data-stu-id="374b0-117">Retrieve properties of a B2X user flow.</span></span>|
|[<span data-ttu-id="374b0-118">创建用户流</span><span class="sxs-lookup"><span data-stu-id="374b0-118">Create user flow</span></span>](../api/identitycontainer-post-b2xuserflows.md)|<span data-ttu-id="374b0-119">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="374b0-119">b2xIdentityUserFlow</span></span>|<span data-ttu-id="374b0-120">新建 B2X 用户流。</span><span class="sxs-lookup"><span data-stu-id="374b0-120">Create a new B2X user flow.</span></span>|
|[<span data-ttu-id="374b0-121">删除用户流</span><span class="sxs-lookup"><span data-stu-id="374b0-121">Delete user flow</span></span>](../api/b2xidentityuserflow-delete.md)|<span data-ttu-id="374b0-122">无</span><span class="sxs-lookup"><span data-stu-id="374b0-122">None</span></span>|<span data-ttu-id="374b0-123">删除 B2X 用户流。</span><span class="sxs-lookup"><span data-stu-id="374b0-123">Delete a B2X user flow.</span></span>|
|[<span data-ttu-id="374b0-124">列出标识提供者</span><span class="sxs-lookup"><span data-stu-id="374b0-124">List identity providers</span></span>](../api/b2xidentityuserflow-list-identityproviders.md)|<span data-ttu-id="374b0-125">[identityProvider](../resources/identityProvider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="374b0-125">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="374b0-126">检索 B2X 用户流中的所有标识提供者。</span><span class="sxs-lookup"><span data-stu-id="374b0-126">Retrieve all identity providers in a B2X user flow.</span></span>|
|[<span data-ttu-id="374b0-127">添加标识提供者</span><span class="sxs-lookup"><span data-stu-id="374b0-127">Add identity provider</span></span>](../api/b2xidentityuserflow-post-identityproviders.md)|<span data-ttu-id="374b0-128">无</span><span class="sxs-lookup"><span data-stu-id="374b0-128">None</span></span>|<span data-ttu-id="374b0-129">向 B2X 用户流添加标识提供者。</span><span class="sxs-lookup"><span data-stu-id="374b0-129">Add an identity provider to a B2X user flow.</span></span>|
|[<span data-ttu-id="374b0-130">删除标识提供者</span><span class="sxs-lookup"><span data-stu-id="374b0-130">Remove identity provider</span></span>](../api/b2xidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="374b0-131">无</span><span class="sxs-lookup"><span data-stu-id="374b0-131">None</span></span>|<span data-ttu-id="374b0-132">从 B2X 用户流中删除标识提供者。</span><span class="sxs-lookup"><span data-stu-id="374b0-132">Remove an identity provider from a B2X user flow.</span></span>|
|[<span data-ttu-id="374b0-133">列出用户属性作业</span><span class="sxs-lookup"><span data-stu-id="374b0-133">List user attribute assignments</span></span>](../api/b2xidentityuserflow-list-userattributeassignments.md)|<span data-ttu-id="374b0-134">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="374b0-134">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="374b0-135">从 B2C 用户流中检索所有用户属性作业。</span><span class="sxs-lookup"><span data-stu-id="374b0-135">Retrieve all user attribute assignments in a B2X user flow.</span></span>|
|[<span data-ttu-id="374b0-136">创建用户属性作业</span><span class="sxs-lookup"><span data-stu-id="374b0-136">Create user attribute assignment</span></span>](../api/b2xidentityuserflow-post-userattributeassignments.md)|[<span data-ttu-id="374b0-137">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="374b0-137">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="374b0-138">在 B2C 用户流中创建一个用户属性作业。</span><span class="sxs-lookup"><span data-stu-id="374b0-138">Create a user attribute assignment in a B2X user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="374b0-139">属性</span><span class="sxs-lookup"><span data-stu-id="374b0-139">Properties</span></span>

|<span data-ttu-id="374b0-140">属性</span><span class="sxs-lookup"><span data-stu-id="374b0-140">Property</span></span>|<span data-ttu-id="374b0-141">类型</span><span class="sxs-lookup"><span data-stu-id="374b0-141">Type</span></span>|<span data-ttu-id="374b0-142">说明</span><span class="sxs-lookup"><span data-stu-id="374b0-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="374b0-143">id</span><span class="sxs-lookup"><span data-stu-id="374b0-143">id</span></span>|<span data-ttu-id="374b0-144">String</span><span class="sxs-lookup"><span data-stu-id="374b0-144">String</span></span>|<span data-ttu-id="374b0-145">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="374b0-145">The name of the user flow.</span></span> <span data-ttu-id="374b0-146">这是一个必需的值且在创建之后不可变。</span><span class="sxs-lookup"><span data-stu-id="374b0-146">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="374b0-147">创建后，该名称将以 `B2X_1_` 的值作为前缀。</span><span class="sxs-lookup"><span data-stu-id="374b0-147">The name will be prefixed with the value of `B2X_1_` after creation.</span></span>|
|<span data-ttu-id="374b0-148">userFlowType</span><span class="sxs-lookup"><span data-stu-id="374b0-148">userFlowType</span></span>|<span data-ttu-id="374b0-149">字符串</span><span class="sxs-lookup"><span data-stu-id="374b0-149">String</span></span>|<span data-ttu-id="374b0-150">用户流类型。</span><span class="sxs-lookup"><span data-stu-id="374b0-150">The type of user flow.</span></span> <span data-ttu-id="374b0-151">对于自助注册用户流，该值在创建后只能 `signUpOrSignIn`，不能修改。</span><span class="sxs-lookup"><span data-stu-id="374b0-151">For self-service sign up user flows, the value can only be `signUpOrSignIn` and cannot be modified after creation.</span></span>|
|<span data-ttu-id="374b0-152">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="374b0-152">userFlowTypeVersion</span></span>|<span data-ttu-id="374b0-153">单一</span><span class="sxs-lookup"><span data-stu-id="374b0-153">Single</span></span>|<span data-ttu-id="374b0-154">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="374b0-154">The version of the user flow.</span></span> <span data-ttu-id="374b0-155">对于 B2X 用户流，版本始终是`1`</span><span class="sxs-lookup"><span data-stu-id="374b0-155">For B2X user flows, the version is always `1`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="374b0-156">关系</span><span class="sxs-lookup"><span data-stu-id="374b0-156">Relationships</span></span>

| <span data-ttu-id="374b0-157">关系</span><span class="sxs-lookup"><span data-stu-id="374b0-157">Relationship</span></span>       | <span data-ttu-id="374b0-158">类型</span><span class="sxs-lookup"><span data-stu-id="374b0-158">Type</span></span>  |<span data-ttu-id="374b0-159">说明</span><span class="sxs-lookup"><span data-stu-id="374b0-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="374b0-160">identityProviders</span><span class="sxs-lookup"><span data-stu-id="374b0-160">identityProviders</span></span>|<span data-ttu-id="374b0-161">[identityProvider](../resources/identityprovider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="374b0-161">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="374b0-162">用户流中包含的标识提供者。</span><span class="sxs-lookup"><span data-stu-id="374b0-162">The identity providers included in the user flow.</span></span>|
|<span data-ttu-id="374b0-163">userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="374b0-163">userAttributeAssignments</span></span>|<span data-ttu-id="374b0-164">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="374b0-164">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="374b0-165">包含在用户流内的用户属性作业。</span><span class="sxs-lookup"><span data-stu-id="374b0-165">The user attribute assignments included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="374b0-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="374b0-166">JSON representation</span></span>

<span data-ttu-id="374b0-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="374b0-167">The following is a JSON representation of the resource.</span></span>

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
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}]
}
```
