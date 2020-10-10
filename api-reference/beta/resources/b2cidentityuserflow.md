---
title: b2cIdentityUserFlow 资源类型
description: 表示 Azure Active Directory B2C 租户内的用户流。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: af29926d77c8888cadc67c4cd7e7558fe47062d6
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406360"
---
# <a name="b2cidentityuserflow-resource-type"></a><span data-ttu-id="0c397-103">b2cIdentityUserFlow 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c397-103">b2cIdentityUserFlow resource type</span></span>

<span data-ttu-id="0c397-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c397-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c397-105">表示 Azure Active Directory B2C 租户内的用户流。</span><span class="sxs-lookup"><span data-stu-id="0c397-105">Represents a user flow within an Azure Active Directory B2C tenant.</span></span>

<span data-ttu-id="0c397-106">为帮助你为应用程序设置最常见的标识任务，Azure Active Directory B2C 包含预定义的、可配置的策略，称为[用户流](/azure/active-directory-b2c/user-flow-overview)。</span><span class="sxs-lookup"><span data-stu-id="0c397-106">To help you set up the most common identity tasks for your applications, Azure Active Directory B2C includes predefined, configurable policies called [user flows](/azure/active-directory-b2c/user-flow-overview).</span></span> <span data-ttu-id="0c397-107">用户流可用于确定用户在执行登录、注册、编辑配置文件或重置密码等操作时与应用程序交互的方式。</span><span class="sxs-lookup"><span data-stu-id="0c397-107">A user flow lets you determine how users interact with your application when they do things like sign in, sign up, edit a profile, or reset a password.</span></span> <span data-ttu-id="0c397-108">可在租户中创建许多不同类型的用户流，并根据需要在应用程序中使用它们。</span><span class="sxs-lookup"><span data-stu-id="0c397-108">You can create many user flows of different types in your tenant and use them in your applications as needed.</span></span> <span data-ttu-id="0c397-109">可以使用用户流控制以下功能：</span><span class="sxs-lookup"><span data-stu-id="0c397-109">With user flows, you can control the following capabilities:</span></span>

- <span data-ttu-id="0c397-110">用于登录的帐户类型，如 Facebook 或本地帐户等社交帐户</span><span class="sxs-lookup"><span data-stu-id="0c397-110">Account types used for sign-in, such as social accounts like a Facebook or local account</span></span>
- <span data-ttu-id="0c397-111">从消费者处收集的属性，例如姓名、邮政编码和鞋码</span><span class="sxs-lookup"><span data-stu-id="0c397-111">Attributes to be collected from the consumer, such as first name, postal code, and shoe size</span></span>
- <span data-ttu-id="0c397-112">Azure Multi-Factor Authentication</span><span class="sxs-lookup"><span data-stu-id="0c397-112">Azure Multi-Factor Authentication</span></span>
- <span data-ttu-id="0c397-113">自定义用户界面</span><span class="sxs-lookup"><span data-stu-id="0c397-113">Customization of the user interface</span></span>
- <span data-ttu-id="0c397-114">应用程序在令牌中接收的信息</span><span class="sxs-lookup"><span data-stu-id="0c397-114">Information that the application receives in the token</span></span>

## <a name="methods"></a><span data-ttu-id="0c397-115">方法</span><span class="sxs-lookup"><span data-stu-id="0c397-115">Methods</span></span>

| <span data-ttu-id="0c397-116">方法</span><span class="sxs-lookup"><span data-stu-id="0c397-116">Method</span></span>       | <span data-ttu-id="0c397-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="0c397-117">Return Type</span></span>  |<span data-ttu-id="0c397-118">说明</span><span class="sxs-lookup"><span data-stu-id="0c397-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c397-119">列出用户流</span><span class="sxs-lookup"><span data-stu-id="0c397-119">List user flows</span></span>](../api/identitycontainer-list-b2cuserflows.md)|<span data-ttu-id="0c397-120">b2cIdentityUserFlow 集合</span><span class="sxs-lookup"><span data-stu-id="0c397-120">b2cIdentityUserFlow collection</span></span>|<span data-ttu-id="0c397-121">检索所 B2C 有用户流。</span><span class="sxs-lookup"><span data-stu-id="0c397-121">Retrieve all B2C user flows.</span></span>|
|[<span data-ttu-id="0c397-122">获取用户流</span><span class="sxs-lookup"><span data-stu-id="0c397-122">Get user flow</span></span>](../api/b2cidentityuserflow-get.md)|<span data-ttu-id="0c397-123">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="0c397-123">b2cIdentityUserFlow</span></span>|<span data-ttu-id="0c397-124">检索 B2C 用户流的属性。</span><span class="sxs-lookup"><span data-stu-id="0c397-124">Retrieve properties of a B2C user flow.</span></span>|
|[<span data-ttu-id="0c397-125">创建用户流</span><span class="sxs-lookup"><span data-stu-id="0c397-125">Create user flow</span></span>](../api/identitycontainer-post-b2cuserflows.md)|<span data-ttu-id="0c397-126">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="0c397-126">b2cIdentityUserFlow</span></span>|<span data-ttu-id="0c397-127">新建 B2C 用户流。</span><span class="sxs-lookup"><span data-stu-id="0c397-127">Create a new B2C user flow.</span></span>|
|[<span data-ttu-id="0c397-128">删除用户流</span><span class="sxs-lookup"><span data-stu-id="0c397-128">Delete user flow</span></span>](../api/b2cidentityuserflow-delete.md)|<span data-ttu-id="0c397-129">无</span><span class="sxs-lookup"><span data-stu-id="0c397-129">None</span></span>|<span data-ttu-id="0c397-130">删除 B2C 用户流。</span><span class="sxs-lookup"><span data-stu-id="0c397-130">Delete a B2C user flow.</span></span>|
|[<span data-ttu-id="0c397-131">列出标识提供者</span><span class="sxs-lookup"><span data-stu-id="0c397-131">List identity providers</span></span>](../api/b2cidentityuserflow-list-identityproviders.md)|<span data-ttu-id="0c397-132">[identityProvider](../resources/identityProvider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="0c397-132">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="0c397-133">检索 B2C 用户流中的所有标识提供者。</span><span class="sxs-lookup"><span data-stu-id="0c397-133">Retrieve all identity providers in a B2C user flow.</span></span>|
|[<span data-ttu-id="0c397-134">添加标识提供者</span><span class="sxs-lookup"><span data-stu-id="0c397-134">Add identity provider</span></span>](../api/b2cidentityuserflow-post-identityproviders.md)|<span data-ttu-id="0c397-135">无</span><span class="sxs-lookup"><span data-stu-id="0c397-135">None</span></span>|<span data-ttu-id="0c397-136">向 B2C 用户流添加标识提供者。</span><span class="sxs-lookup"><span data-stu-id="0c397-136">Add an identity provider to a B2C user flow.</span></span>|
|[<span data-ttu-id="0c397-137">删除标识提供者</span><span class="sxs-lookup"><span data-stu-id="0c397-137">Remove identity provider</span></span>](../api/b2cidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="0c397-138">无</span><span class="sxs-lookup"><span data-stu-id="0c397-138">None</span></span>|<span data-ttu-id="0c397-139">从 B2C 用户流中删除标识提供者。</span><span class="sxs-lookup"><span data-stu-id="0c397-139">Remove an identity provider from a B2C user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c397-140">属性</span><span class="sxs-lookup"><span data-stu-id="0c397-140">Properties</span></span>

|<span data-ttu-id="0c397-141">属性</span><span class="sxs-lookup"><span data-stu-id="0c397-141">Property</span></span>|<span data-ttu-id="0c397-142">类型</span><span class="sxs-lookup"><span data-stu-id="0c397-142">Type</span></span>|<span data-ttu-id="0c397-143">说明</span><span class="sxs-lookup"><span data-stu-id="0c397-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c397-144">id</span><span class="sxs-lookup"><span data-stu-id="0c397-144">id</span></span>|<span data-ttu-id="0c397-145">String</span><span class="sxs-lookup"><span data-stu-id="0c397-145">String</span></span>|<span data-ttu-id="0c397-146">用户流名称。</span><span class="sxs-lookup"><span data-stu-id="0c397-146">The name of the user flow.</span></span> <span data-ttu-id="0c397-147">这是一个必需的值且在创建之后不可变。</span><span class="sxs-lookup"><span data-stu-id="0c397-147">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="0c397-148">创建后，该名称将以 `B2C_1_` 的值作为前缀。</span><span class="sxs-lookup"><span data-stu-id="0c397-148">The name will be prefixed with the value of `B2C_1_` after creation.</span></span>|
|<span data-ttu-id="0c397-149">userFlowType</span><span class="sxs-lookup"><span data-stu-id="0c397-149">userFlowType</span></span>|<span data-ttu-id="0c397-150">字符串</span><span class="sxs-lookup"><span data-stu-id="0c397-150">String</span></span>|<span data-ttu-id="0c397-151">[用户流类型](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions)。</span><span class="sxs-lookup"><span data-stu-id="0c397-151">The [type of user flow](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions).</span></span> <span data-ttu-id="0c397-152">**userFlowType** 支持的值有：</span><span class="sxs-lookup"><span data-stu-id="0c397-152">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|<span data-ttu-id="0c397-153">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="0c397-153">userFlowTypeVersion</span></span>|<span data-ttu-id="0c397-154">单一</span><span class="sxs-lookup"><span data-stu-id="0c397-154">Single</span></span>|<span data-ttu-id="0c397-155">用户流版本。</span><span class="sxs-lookup"><span data-stu-id="0c397-155">The version of the user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c397-156">关系</span><span class="sxs-lookup"><span data-stu-id="0c397-156">Relationships</span></span>

| <span data-ttu-id="0c397-157">关系</span><span class="sxs-lookup"><span data-stu-id="0c397-157">Relationship</span></span>       | <span data-ttu-id="0c397-158">类型</span><span class="sxs-lookup"><span data-stu-id="0c397-158">Type</span></span>  |<span data-ttu-id="0c397-159">说明</span><span class="sxs-lookup"><span data-stu-id="0c397-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c397-160">identityProviders</span><span class="sxs-lookup"><span data-stu-id="0c397-160">identityProviders</span></span>|<span data-ttu-id="0c397-161">[identityProvider](../resources/identityprovider.md)集合 </span><span class="sxs-lookup"><span data-stu-id="0c397-161">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="0c397-162">用户流中包含的标识提供者。</span><span class="sxs-lookup"><span data-stu-id="0c397-162">The identity providers included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c397-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c397-163">JSON representation</span></span>

<span data-ttu-id="0c397-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c397-164">The following is a JSON representation of the resource.</span></span>

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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}]
}
```