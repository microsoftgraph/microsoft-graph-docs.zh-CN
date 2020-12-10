---
title: b2cIdentityUserFlow 资源类型
description: 表示 Azure Active Directory B2C 租户内的用户流。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 61c3a206ee07eb7e8474e501f9064a20c6cc3840
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581087"
---
# <a name="b2cidentityuserflow-resource-type"></a><span data-ttu-id="81a4b-103">b2cIdentityUserFlow 资源类型</span><span class="sxs-lookup"><span data-stu-id="81a4b-103">b2cIdentityUserFlow resource type</span></span>

<span data-ttu-id="81a4b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81a4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81a4b-105">表示 Azure Active Directory B2C 租户内的用户流。</span><span class="sxs-lookup"><span data-stu-id="81a4b-105">Represents a user flow within an Azure Active Directory B2C tenant.</span></span>

<span data-ttu-id="81a4b-106">为帮助你为应用程序设置最常见的标识任务，Azure Active Directory B2C 包含预定义的、可配置的策略，称为[用户流](/azure/active-directory-b2c/user-flow-overview)。</span><span class="sxs-lookup"><span data-stu-id="81a4b-106">To help you set up the most common identity tasks for your applications, Azure Active Directory B2C includes predefined, configurable policies called [user flows](/azure/active-directory-b2c/user-flow-overview).</span></span> <span data-ttu-id="81a4b-107">用户流可用于确定用户在执行登录、注册、编辑配置文件或重置密码等操作时与应用程序交互的方式。</span><span class="sxs-lookup"><span data-stu-id="81a4b-107">A user flow lets you determine how users interact with your application when they do things like sign in, sign up, edit a profile, or reset a password.</span></span> <span data-ttu-id="81a4b-108">可在租户中创建许多不同类型的用户流，并根据需要在应用程序中使用它们。</span><span class="sxs-lookup"><span data-stu-id="81a4b-108">You can create many user flows of different types in your tenant and use them in your applications as needed.</span></span> <span data-ttu-id="81a4b-109">可以使用用户流控制以下功能：</span><span class="sxs-lookup"><span data-stu-id="81a4b-109">With user flows, you can control the following capabilities:</span></span>

- <span data-ttu-id="81a4b-110">用于登录的帐户类型，如 Facebook 或本地帐户等社交帐户</span><span class="sxs-lookup"><span data-stu-id="81a4b-110">Account types used for sign-in, such as social accounts like a Facebook or local account</span></span>
- <span data-ttu-id="81a4b-111">从消费者处收集的属性，例如姓名、邮政编码和鞋码</span><span class="sxs-lookup"><span data-stu-id="81a4b-111">Attributes to be collected from the consumer, such as first name, postal code, and shoe size</span></span>
- <span data-ttu-id="81a4b-112">Azure Multi-Factor Authentication</span><span class="sxs-lookup"><span data-stu-id="81a4b-112">Azure Multi-Factor Authentication</span></span>
- <span data-ttu-id="81a4b-113">自定义用户界面</span><span class="sxs-lookup"><span data-stu-id="81a4b-113">Customization of the user interface</span></span>
- <span data-ttu-id="81a4b-114">应用程序在令牌中接收的信息</span><span class="sxs-lookup"><span data-stu-id="81a4b-114">Information that the application receives in the token</span></span>

## <a name="methods"></a><span data-ttu-id="81a4b-115">方法</span><span class="sxs-lookup"><span data-stu-id="81a4b-115">Methods</span></span>

| <span data-ttu-id="81a4b-116">方法</span><span class="sxs-lookup"><span data-stu-id="81a4b-116">Method</span></span>       | <span data-ttu-id="81a4b-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="81a4b-117">Return Type</span></span>  |<span data-ttu-id="81a4b-118">说明</span><span class="sxs-lookup"><span data-stu-id="81a4b-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81a4b-119">列出用户流</span><span class="sxs-lookup"><span data-stu-id="81a4b-119">List user flows</span></span>](../api/identitycontainer-list-b2cuserflows.md)|<span data-ttu-id="81a4b-120">b2cIdentityUserFlow 集合</span><span class="sxs-lookup"><span data-stu-id="81a4b-120">b2cIdentityUserFlow collection</span></span>|<span data-ttu-id="81a4b-121">检索所 B2C 有用户流。</span><span class="sxs-lookup"><span data-stu-id="81a4b-121">Retrieve all B2C user flows.</span></span>|
|[<span data-ttu-id="81a4b-122">获取用户流</span><span class="sxs-lookup"><span data-stu-id="81a4b-122">Get user flow</span></span>](../api/b2cidentityuserflow-get.md)|<span data-ttu-id="81a4b-123">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="81a4b-123">b2cIdentityUserFlow</span></span>|<span data-ttu-id="81a4b-124">检索 B2C 用户流的属性。</span><span class="sxs-lookup"><span data-stu-id="81a4b-124">Retrieve properties of a B2C user flow.</span></span>|
|[<span data-ttu-id="81a4b-125">创建用户流</span><span class="sxs-lookup"><span data-stu-id="81a4b-125">Create user flow</span></span>](../api/identitycontainer-post-b2cuserflows.md)|<span data-ttu-id="81a4b-126">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="81a4b-126">b2cIdentityUserFlow</span></span>|<span data-ttu-id="81a4b-127">新建 B2C 用户流。</span><span class="sxs-lookup"><span data-stu-id="81a4b-127">Create a new B2C user flow.</span></span>|
|[<span data-ttu-id="81a4b-128">删除用户流</span><span class="sxs-lookup"><span data-stu-id="81a4b-128">Delete user flow</span></span>](../api/b2cidentityuserflow-delete.md)|<span data-ttu-id="81a4b-129">无</span><span class="sxs-lookup"><span data-stu-id="81a4b-129">None</span></span>|<span data-ttu-id="81a4b-130">删除 B2C 用户流。</span><span class="sxs-lookup"><span data-stu-id="81a4b-130">Delete a B2C user flow.</span></span>|
|[<span data-ttu-id="81a4b-131">列出标识提供者</span><span class="sxs-lookup"><span data-stu-id="81a4b-131">List identity providers</span></span>](../api/b2cidentityuserflow-list-identityproviders.md)|<span data-ttu-id="81a4b-132">[identityProvider](../resources/identityProvider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="81a4b-132">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="81a4b-133">检索 B2C 用户流中的所有标识提供者。</span><span class="sxs-lookup"><span data-stu-id="81a4b-133">Retrieve all identity providers in a B2C user flow.</span></span>|
|[<span data-ttu-id="81a4b-134">添加标识提供者</span><span class="sxs-lookup"><span data-stu-id="81a4b-134">Add identity provider</span></span>](../api/b2cidentityuserflow-post-identityproviders.md)|<span data-ttu-id="81a4b-135">无</span><span class="sxs-lookup"><span data-stu-id="81a4b-135">None</span></span>|<span data-ttu-id="81a4b-136">向 B2C 用户流添加标识提供者。</span><span class="sxs-lookup"><span data-stu-id="81a4b-136">Add an identity provider to a B2C user flow.</span></span>|
|[<span data-ttu-id="81a4b-137">删除标识提供者</span><span class="sxs-lookup"><span data-stu-id="81a4b-137">Remove identity provider</span></span>](../api/b2cidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="81a4b-138">无</span><span class="sxs-lookup"><span data-stu-id="81a4b-138">None</span></span>|<span data-ttu-id="81a4b-139">从 B2C 用户流中删除标识提供者。</span><span class="sxs-lookup"><span data-stu-id="81a4b-139">Remove an identity provider from a B2C user flow.</span></span>|
|[<span data-ttu-id="81a4b-140">列表用户属性作业</span><span class="sxs-lookup"><span data-stu-id="81a4b-140">List user attribute assignments</span></span>](../api/b2cidentityuserflow-list-userattributeassignments.md)|<span data-ttu-id="81a4b-141">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81a4b-141">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="81a4b-142">从 B2C 用户流中检索所有用户属性作业。</span><span class="sxs-lookup"><span data-stu-id="81a4b-142">Retrieve all user attribute assignments in a B2C user flow.</span></span>|
|[<span data-ttu-id="81a4b-143">创建用户属性作业</span><span class="sxs-lookup"><span data-stu-id="81a4b-143">Create user attribute assignment</span></span>](../api/b2cidentityuserflow-post-userattributeassignments.md)|[<span data-ttu-id="81a4b-144">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="81a4b-144">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="81a4b-145">在 B2C 用户流中创建所有用户属性作业。</span><span class="sxs-lookup"><span data-stu-id="81a4b-145">Create a user attribute assignment in a B2C user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="81a4b-146">属性</span><span class="sxs-lookup"><span data-stu-id="81a4b-146">Properties</span></span>

|<span data-ttu-id="81a4b-147">属性</span><span class="sxs-lookup"><span data-stu-id="81a4b-147">Property</span></span>|<span data-ttu-id="81a4b-148">类型</span><span class="sxs-lookup"><span data-stu-id="81a4b-148">Type</span></span>|<span data-ttu-id="81a4b-149">说明</span><span class="sxs-lookup"><span data-stu-id="81a4b-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81a4b-150">id</span><span class="sxs-lookup"><span data-stu-id="81a4b-150">id</span></span>|<span data-ttu-id="81a4b-151">String</span><span class="sxs-lookup"><span data-stu-id="81a4b-151">String</span></span>|<span data-ttu-id="81a4b-152">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="81a4b-152">The name of the user flow.</span></span> <span data-ttu-id="81a4b-153">这是一个必需的值且在创建之后不可变。</span><span class="sxs-lookup"><span data-stu-id="81a4b-153">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="81a4b-154">创建后，该名称将以 `B2C_1_` 的值作为前缀。</span><span class="sxs-lookup"><span data-stu-id="81a4b-154">The name will be prefixed with the value of `B2C_1_` after creation.</span></span>|
|<span data-ttu-id="81a4b-155">userFlowType</span><span class="sxs-lookup"><span data-stu-id="81a4b-155">userFlowType</span></span>|<span data-ttu-id="81a4b-156">字符串</span><span class="sxs-lookup"><span data-stu-id="81a4b-156">String</span></span>|<span data-ttu-id="81a4b-157">[用户流类型](/azure/active-directory-b2c/user-flow-versions)。</span><span class="sxs-lookup"><span data-stu-id="81a4b-157">The [type of user flow](/azure/active-directory-b2c/user-flow-versions).</span></span> <span data-ttu-id="81a4b-158">**userFlowType** 支持的值有：</span><span class="sxs-lookup"><span data-stu-id="81a4b-158">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|<span data-ttu-id="81a4b-159">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="81a4b-159">userFlowTypeVersion</span></span>|<span data-ttu-id="81a4b-160">单一</span><span class="sxs-lookup"><span data-stu-id="81a4b-160">Single</span></span>|<span data-ttu-id="81a4b-161">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="81a4b-161">The version of the user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81a4b-162">关系</span><span class="sxs-lookup"><span data-stu-id="81a4b-162">Relationships</span></span>

| <span data-ttu-id="81a4b-163">关系</span><span class="sxs-lookup"><span data-stu-id="81a4b-163">Relationship</span></span>       | <span data-ttu-id="81a4b-164">类型</span><span class="sxs-lookup"><span data-stu-id="81a4b-164">Type</span></span>  |<span data-ttu-id="81a4b-165">说明</span><span class="sxs-lookup"><span data-stu-id="81a4b-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81a4b-166">identityProviders</span><span class="sxs-lookup"><span data-stu-id="81a4b-166">identityProviders</span></span>|<span data-ttu-id="81a4b-167">[identityProvider](../resources/identityprovider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="81a4b-167">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="81a4b-168">用户流中包含的标识提供者。</span><span class="sxs-lookup"><span data-stu-id="81a4b-168">The identity providers included in the user flow.</span></span>|
|<span data-ttu-id="81a4b-169">userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="81a4b-169">userAttributeAssignments</span></span>|<span data-ttu-id="81a4b-170">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81a4b-170">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="81a4b-171">包含在用户流内的用户属性作业。</span><span class="sxs-lookup"><span data-stu-id="81a4b-171">The user attribute assignments included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81a4b-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81a4b-172">JSON representation</span></span>

<span data-ttu-id="81a4b-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81a4b-173">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
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
