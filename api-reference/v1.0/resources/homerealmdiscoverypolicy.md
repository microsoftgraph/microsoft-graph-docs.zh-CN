---
title: homeRealmDiscoveryPolicy 资源类型
description: 表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略。
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 78fee8908291619a819b1d62108d149c39b0ae68
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444411"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="d9789-103">homeRealmDiscoveryPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9789-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="d9789-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9789-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9789-105">表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略，尤其是针对联合域中的自动加速和用户身份验证限制。</span><span class="sxs-lookup"><span data-stu-id="d9789-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="d9789-106">您可以为组织的所有服务主体或组织中特定的服务主体设置 **homeRealmDiscoveryPolicy。**</span><span class="sxs-lookup"><span data-stu-id="d9789-106">You can set **homeRealmDiscoveryPolicy** for all service principals in your organization, or for specific service principals in your organization.</span></span> <span data-ttu-id="d9789-107">有关更多方案和策略详细信息，请参阅使用家庭领域发现策略为应用程序配置[Azure AD](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal)登录行为，以及使用电子邮件作为备用登录 ID 登录[Azure Active Directory。](/azure/active-directory/authentication/howto-authentication-use-email-signin)</span><span class="sxs-lookup"><span data-stu-id="d9789-107">For more scenario and policy details, see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) as well as [Sign-in to Azure Active Directory using email as an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span>

<span data-ttu-id="d9789-108">继承自 [stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="d9789-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d9789-109">Methods</span><span class="sxs-lookup"><span data-stu-id="d9789-109">Methods</span></span>

| <span data-ttu-id="d9789-110">方法</span><span class="sxs-lookup"><span data-stu-id="d9789-110">Method</span></span>       | <span data-ttu-id="d9789-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9789-111">Return Type</span></span> | <span data-ttu-id="d9789-112">说明</span><span class="sxs-lookup"><span data-stu-id="d9789-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d9789-113">列出 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="d9789-113">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="d9789-114">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="d9789-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="d9789-115">读取 homeRealmDiscoveryPolicies 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9789-115">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="d9789-116">创建 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="d9789-116">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="d9789-117">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="d9789-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="d9789-118">创建 homeRealmDiscoveryPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="d9789-118">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="d9789-119">获取 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="d9789-119">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="d9789-120">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="d9789-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="d9789-121">读取 homeRealmDiscoveryPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9789-121">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="d9789-122">更新 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="d9789-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="d9789-123">无</span><span class="sxs-lookup"><span data-stu-id="d9789-123">None</span></span> | <span data-ttu-id="d9789-124">更新 homeRealmDiscoveryPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="d9789-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="d9789-125">删除 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="d9789-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="d9789-126">无</span><span class="sxs-lookup"><span data-stu-id="d9789-126">None</span></span> | <span data-ttu-id="d9789-127">删除 homeRealmDiscoveryPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="d9789-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="d9789-128">List appliesTo</span><span class="sxs-lookup"><span data-stu-id="d9789-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="d9789-129">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="d9789-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="d9789-130">获取已应用此策略的 directoryObjects 列表。</span><span class="sxs-lookup"><span data-stu-id="d9789-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="d9789-131">属性</span><span class="sxs-lookup"><span data-stu-id="d9789-131">Properties</span></span>

| <span data-ttu-id="d9789-132">属性</span><span class="sxs-lookup"><span data-stu-id="d9789-132">Property</span></span>     | <span data-ttu-id="d9789-133">类型</span><span class="sxs-lookup"><span data-stu-id="d9789-133">Type</span></span>        | <span data-ttu-id="d9789-134">说明</span><span class="sxs-lookup"><span data-stu-id="d9789-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9789-135">id</span><span class="sxs-lookup"><span data-stu-id="d9789-135">id</span></span>|<span data-ttu-id="d9789-136">String</span><span class="sxs-lookup"><span data-stu-id="d9789-136">String</span></span>| <span data-ttu-id="d9789-137">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d9789-137">Unique identifier for this policy.</span></span> <span data-ttu-id="d9789-138">只读。</span><span class="sxs-lookup"><span data-stu-id="d9789-138">Read-only.</span></span>|
|<span data-ttu-id="d9789-139">definition</span><span class="sxs-lookup"><span data-stu-id="d9789-139">definition</span></span>|<span data-ttu-id="d9789-140">String collection</span><span class="sxs-lookup"><span data-stu-id="d9789-140">String collection</span></span>| <span data-ttu-id="d9789-141">包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="d9789-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="d9789-142">有关此属性的 JSON 架构的详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="d9789-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="d9789-143">必需。</span><span class="sxs-lookup"><span data-stu-id="d9789-143">Required.</span></span>|
|<span data-ttu-id="d9789-144">description</span><span class="sxs-lookup"><span data-stu-id="d9789-144">description</span></span>|<span data-ttu-id="d9789-145">String</span><span class="sxs-lookup"><span data-stu-id="d9789-145">String</span></span>| <span data-ttu-id="d9789-146">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="d9789-146">Description for this policy.</span></span>|
|<span data-ttu-id="d9789-147">displayName</span><span class="sxs-lookup"><span data-stu-id="d9789-147">displayName</span></span>|<span data-ttu-id="d9789-148">String</span><span class="sxs-lookup"><span data-stu-id="d9789-148">String</span></span>| <span data-ttu-id="d9789-149">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d9789-149">Display name for this policy.</span></span> <span data-ttu-id="d9789-150">必填。</span><span class="sxs-lookup"><span data-stu-id="d9789-150">Required.</span></span>|
|<span data-ttu-id="d9789-151">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="d9789-151">isOrganizationDefault</span></span>|<span data-ttu-id="d9789-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9789-152">Boolean</span></span>|<span data-ttu-id="d9789-153">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="d9789-153">If set to true, activates this policy.</span></span> <span data-ttu-id="d9789-154">同一策略类型可以有很多策略，但只有一个策略可以激活为组织默认设置。</span><span class="sxs-lookup"><span data-stu-id="d9789-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="d9789-155">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="d9789-155">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="d9789-156">主领域发现策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="d9789-156">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="d9789-157">下面的属性构成表示令牌生存期策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d9789-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="d9789-158">此 JSON 对象 **必须转换为带** 转义引号的字符串，以插入到 **定义** 属性中。</span><span class="sxs-lookup"><span data-stu-id="d9789-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="d9789-159">下面显示了 JSON 格式的示例：</span><span class="sxs-lookup"><span data-stu-id="d9789-159">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"HomeRealmDiscoveryPolicy\":
     {\"AccelerateToFederatedDomain\":true,
      \"PreferredDomain\":\"federated.example.edu\",
      \"AlternateIdLogin\":{\"Enabled\":true}}}"
  ]
```

| <span data-ttu-id="d9789-160">属性</span><span class="sxs-lookup"><span data-stu-id="d9789-160">Property</span></span>     | <span data-ttu-id="d9789-161">类型</span><span class="sxs-lookup"><span data-stu-id="d9789-161">Type</span></span>   |<span data-ttu-id="d9789-162">说明</span><span class="sxs-lookup"><span data-stu-id="d9789-162">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="d9789-163">AccelerateToFederatedDomain</span><span class="sxs-lookup"><span data-stu-id="d9789-163">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="d9789-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9789-164">Boolean</span></span>| <span data-ttu-id="d9789-165">设置为 `true` 自动加速 (绕过主领域发现) 。</span><span class="sxs-lookup"><span data-stu-id="d9789-165">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="d9789-166">如果租户中只有一个已验证和联合域，用户将直接进入联合标识提供程序 (例如 `true` ADFS) 登录。</span><span class="sxs-lookup"><span data-stu-id="d9789-166">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="d9789-167">如果 `true` 租户中存在多个已验证域，则必须指定 **PreferredDomain。**</span><span class="sxs-lookup"><span data-stu-id="d9789-167">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="d9789-168">可选。</span><span class="sxs-lookup"><span data-stu-id="d9789-168">Optional.</span></span>|
|<span data-ttu-id="d9789-169">PreferredDomain</span><span class="sxs-lookup"><span data-stu-id="d9789-169">PreferredDomain</span></span>|<span data-ttu-id="d9789-170">String</span><span class="sxs-lookup"><span data-stu-id="d9789-170">String</span></span>| <span data-ttu-id="d9789-171">指定要加速登录的域。</span><span class="sxs-lookup"><span data-stu-id="d9789-171">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="d9789-172">如果租户只有一个联合域，可以省略它。</span><span class="sxs-lookup"><span data-stu-id="d9789-172">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="d9789-173">如果省略它，并且存在多个已验证的联合域，则此策略无效。</span><span class="sxs-lookup"><span data-stu-id="d9789-173">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="d9789-174">如果 **AccelerateToFederatedDomain** 为 ，则必需 `true` 。</span><span class="sxs-lookup"><span data-stu-id="d9789-174">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="d9789-175">AllowCloudPasswordValidation</span><span class="sxs-lookup"><span data-stu-id="d9789-175">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="d9789-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9789-176">Boolean</span></span>| <span data-ttu-id="d9789-177">设置为允许应用程序通过直接向 Azure Active Directory 令牌终结点显示用户名/密码凭据来 `true` 对联盟用户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d9789-177">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="d9789-178">仅在启用密码哈希同步时有效。</span><span class="sxs-lookup"><span data-stu-id="d9789-178">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="d9789-179">可选。</span><span class="sxs-lookup"><span data-stu-id="d9789-179">Optional.</span></span>|
|<span data-ttu-id="d9789-180">AlternateIdLogin</span><span class="sxs-lookup"><span data-stu-id="d9789-180">AlternateIdLogin</span></span>| <span data-ttu-id="d9789-181">Json</span><span class="sxs-lookup"><span data-stu-id="d9789-181">Json</span></span> |<span data-ttu-id="d9789-182">设置为 {"Enabled"： true} 以允许使用电子邮件作为备用登录 [ID 进行](/azure/active-directory/authentication/howto-authentication-use-email-signin)Azure AD 登录。</span><span class="sxs-lookup"><span data-stu-id="d9789-182">Set to {"Enabled": true} to allow Azure AD sign-in using email as [an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span> <span data-ttu-id="d9789-183">仅在 **IsOrganizationDefault 设置为** 时有效 `true` 。</span><span class="sxs-lookup"><span data-stu-id="d9789-183">Only works when **IsOrganizationDefault** is set to `true`.</span></span> <span data-ttu-id="d9789-184">可选。</span><span class="sxs-lookup"><span data-stu-id="d9789-184">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9789-185">关系</span><span class="sxs-lookup"><span data-stu-id="d9789-185">Relationships</span></span>

| <span data-ttu-id="d9789-186">关系</span><span class="sxs-lookup"><span data-stu-id="d9789-186">Relationship</span></span> | <span data-ttu-id="d9789-187">类型</span><span class="sxs-lookup"><span data-stu-id="d9789-187">Type</span></span>        | <span data-ttu-id="d9789-188">说明</span><span class="sxs-lookup"><span data-stu-id="d9789-188">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9789-189">appliesTo</span><span class="sxs-lookup"><span data-stu-id="d9789-189">appliesTo</span></span>|<span data-ttu-id="d9789-190">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="d9789-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d9789-191">已应用此策略的 [directoryObject](directoryObject.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="d9789-191">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="d9789-192">只读。</span><span class="sxs-lookup"><span data-stu-id="d9789-192">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9789-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9789-193">JSON representation</span></span>

<span data-ttu-id="d9789-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9789-194">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "homeRealmDiscoveryPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
