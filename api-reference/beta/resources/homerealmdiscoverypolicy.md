---
title: homeRealmDiscoveryPolicy 资源类型
description: 表示用于控制联合用户的 Azure Active Directory 身份验证行为的策略。
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 694309327fe122a0053039d527321f0f4afb0751
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635157"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="5b43d-103">homeRealmDiscoveryPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b43d-103">homeRealmDiscoveryPolicy resource type</span></span>

<span data-ttu-id="5b43d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b43d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b43d-105">表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略，尤其适用于联合域中的自动加速和用户身份验证限制。</span><span class="sxs-lookup"><span data-stu-id="5b43d-105">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="5b43d-106">您可以为组织中的所有服务主体或组织中的特定服务主体设置 homeRealmDiscoveryPolicy。</span><span class="sxs-lookup"><span data-stu-id="5b43d-106">You can set homeRealmDiscoveryPolicy for all service principals in your organization, or for specific service principals in your organization.</span></span>  <span data-ttu-id="5b43d-107">有关详细情况和策略的详细信息，请参阅使用主领域发现策略和[使用电子邮件作为备用登录 ID 登录 Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin)，为[应用程序配置 Azure AD 登录行为](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal)。</span><span class="sxs-lookup"><span data-stu-id="5b43d-107">For more scenario and policy details see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal) as well as [Sign-in to Azure Active Directory using email as an alternate login ID](/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span>

<span data-ttu-id="5b43d-108">继承自 [stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="5b43d-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5b43d-109">方法</span><span class="sxs-lookup"><span data-stu-id="5b43d-109">Methods</span></span>

| <span data-ttu-id="5b43d-110">方法</span><span class="sxs-lookup"><span data-stu-id="5b43d-110">Method</span></span>       | <span data-ttu-id="5b43d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5b43d-111">Return Type</span></span> | <span data-ttu-id="5b43d-112">说明</span><span class="sxs-lookup"><span data-stu-id="5b43d-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5b43d-113">创建 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="5b43d-113">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="5b43d-114">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="5b43d-114">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="5b43d-115">创建 homeRealmDiscoveryPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="5b43d-115">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="5b43d-116">获取 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="5b43d-116">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="5b43d-117">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="5b43d-117">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="5b43d-118">读取 homeRealmDiscoveryPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5b43d-118">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="5b43d-119">列出 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="5b43d-119">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="5b43d-120">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="5b43d-120">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="5b43d-121">读取 homeRealmDiscoveryPolicies 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5b43d-121">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="5b43d-122">更新 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="5b43d-122">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="5b43d-123">无</span><span class="sxs-lookup"><span data-stu-id="5b43d-123">None</span></span> | <span data-ttu-id="5b43d-124">更新 homeRealmDiscoveryPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="5b43d-124">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="5b43d-125">删除 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="5b43d-125">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="5b43d-126">无</span><span class="sxs-lookup"><span data-stu-id="5b43d-126">None</span></span> | <span data-ttu-id="5b43d-127">删除 homeRealmDiscoveryPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="5b43d-127">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="5b43d-128">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="5b43d-128">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="5b43d-129">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5b43d-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="5b43d-130">获取已应用此策略的 directoryObjects 的列表。</span><span class="sxs-lookup"><span data-stu-id="5b43d-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="5b43d-131">分配 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="5b43d-131">Assign homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-post-homerealmdiscoverypolicies.md) | <span data-ttu-id="5b43d-132">无</span><span class="sxs-lookup"><span data-stu-id="5b43d-132">None</span></span> | <span data-ttu-id="5b43d-133">将 homeRealmDiscoveryPolicy 对象分配给 [servicePrincipal](serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5b43d-133">Assign a homeRealmDiscoveryPolicy object to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="5b43d-134">列表已分配 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="5b43d-134">List assigned homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-list-homerealmdiscoverypolicies.md) | <span data-ttu-id="5b43d-135">[homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5b43d-135">[homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) collection</span></span> | <span data-ttu-id="5b43d-136">列出分配给 [servicePrincipal](serviceprincipal.md) 对象的 homeRealmDiscoveryPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="5b43d-136">List the homeRealmDiscoveryPolicy objects that are assigned to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="5b43d-137">删除 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="5b43d-137">Remove homeRealmDiscoveryPolicy</span></span>](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md) | <span data-ttu-id="5b43d-138">无</span><span class="sxs-lookup"><span data-stu-id="5b43d-138">None</span></span> | <span data-ttu-id="5b43d-139">从 [servicePrincipal](serviceprincipal.md) 对象中删除一个 homeRealmDiscoveryPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="5b43d-139">Remove a homeRealmDiscoveryPolicy object from a [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5b43d-140">属性</span><span class="sxs-lookup"><span data-stu-id="5b43d-140">Properties</span></span>

| <span data-ttu-id="5b43d-141">属性</span><span class="sxs-lookup"><span data-stu-id="5b43d-141">Property</span></span>     | <span data-ttu-id="5b43d-142">类型</span><span class="sxs-lookup"><span data-stu-id="5b43d-142">Type</span></span>        | <span data-ttu-id="5b43d-143">说明</span><span class="sxs-lookup"><span data-stu-id="5b43d-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5b43d-144">id</span><span class="sxs-lookup"><span data-stu-id="5b43d-144">id</span></span>|<span data-ttu-id="5b43d-145">String</span><span class="sxs-lookup"><span data-stu-id="5b43d-145">String</span></span>| <span data-ttu-id="5b43d-146">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5b43d-146">Unique identifier for this policy.</span></span> <span data-ttu-id="5b43d-147">只读。</span><span class="sxs-lookup"><span data-stu-id="5b43d-147">Read-only.</span></span>|
|<span data-ttu-id="5b43d-148">定义</span><span class="sxs-lookup"><span data-stu-id="5b43d-148">definition</span></span>|<span data-ttu-id="5b43d-149">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5b43d-149">String collection</span></span>| <span data-ttu-id="5b43d-150">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="5b43d-150">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="5b43d-151">有关此属性的 JSON 架构的更多详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="5b43d-151">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="5b43d-152">必需。</span><span class="sxs-lookup"><span data-stu-id="5b43d-152">Required.</span></span>|
|<span data-ttu-id="5b43d-153">description</span><span class="sxs-lookup"><span data-stu-id="5b43d-153">description</span></span>|<span data-ttu-id="5b43d-154">String</span><span class="sxs-lookup"><span data-stu-id="5b43d-154">String</span></span>| <span data-ttu-id="5b43d-155">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="5b43d-155">Description for this policy.</span></span>|
|<span data-ttu-id="5b43d-156">displayName</span><span class="sxs-lookup"><span data-stu-id="5b43d-156">displayName</span></span>|<span data-ttu-id="5b43d-157">String</span><span class="sxs-lookup"><span data-stu-id="5b43d-157">String</span></span>| <span data-ttu-id="5b43d-158">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5b43d-158">Display name for this policy.</span></span> <span data-ttu-id="5b43d-159">必需。</span><span class="sxs-lookup"><span data-stu-id="5b43d-159">Required.</span></span>|
|<span data-ttu-id="5b43d-160">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="5b43d-160">isOrganizationDefault</span></span>|<span data-ttu-id="5b43d-161">布尔值</span><span class="sxs-lookup"><span data-stu-id="5b43d-161">Boolean</span></span>|<span data-ttu-id="5b43d-162">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="5b43d-162">If set to true, activates this policy.</span></span> <span data-ttu-id="5b43d-163">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="5b43d-163">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="5b43d-164">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="5b43d-164">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="5b43d-165">主领域发现策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="5b43d-165">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="5b43d-166">下面的属性构成了表示令牌生存期策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5b43d-166">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="5b43d-167">此 JSON 对象必须 **转换为转义了引号的字符串** ，以将其插入到 **定义** 属性中。</span><span class="sxs-lookup"><span data-stu-id="5b43d-167">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="5b43d-168">下面以 JSON 格式显示了一个示例：</span><span class="sxs-lookup"><span data-stu-id="5b43d-168">An example is shown below in JSON format:</span></span>

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

| <span data-ttu-id="5b43d-169">属性</span><span class="sxs-lookup"><span data-stu-id="5b43d-169">Property</span></span>     | <span data-ttu-id="5b43d-170">类型</span><span class="sxs-lookup"><span data-stu-id="5b43d-170">Type</span></span>   |<span data-ttu-id="5b43d-171">说明</span><span class="sxs-lookup"><span data-stu-id="5b43d-171">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="5b43d-172">AccelerateToFederatedDomain</span><span class="sxs-lookup"><span data-stu-id="5b43d-172">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="5b43d-173">布尔值</span><span class="sxs-lookup"><span data-stu-id="5b43d-173">Boolean</span></span>| <span data-ttu-id="5b43d-174">如果设置为 `true` ，则自动加速 (绕过主页领域发现) 。</span><span class="sxs-lookup"><span data-stu-id="5b43d-174">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="5b43d-175">如果 `true` 在租户中只有一个经过验证和联合的域，则用户将直接转到联合身份提供程序 (如用于登录的 ADFS) 。</span><span class="sxs-lookup"><span data-stu-id="5b43d-175">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="5b43d-176">如果 `true` 租户中有多个已验证的域，则必须指定 **PreferredDomain** 。</span><span class="sxs-lookup"><span data-stu-id="5b43d-176">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="5b43d-177">可选。</span><span class="sxs-lookup"><span data-stu-id="5b43d-177">Optional.</span></span>|
|<span data-ttu-id="5b43d-178">PreferredDomain</span><span class="sxs-lookup"><span data-stu-id="5b43d-178">PreferredDomain</span></span>|<span data-ttu-id="5b43d-179">String</span><span class="sxs-lookup"><span data-stu-id="5b43d-179">String</span></span>| <span data-ttu-id="5b43d-180">指定要加速登录到的域。</span><span class="sxs-lookup"><span data-stu-id="5b43d-180">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="5b43d-181">如果租户只有一个联合域，则可以省略它。</span><span class="sxs-lookup"><span data-stu-id="5b43d-181">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="5b43d-182">如果省略它，并且有多个经过验证的联合域，则此策略将不起作用。</span><span class="sxs-lookup"><span data-stu-id="5b43d-182">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="5b43d-183">如果 **AccelerateToFederatedDomain** 为，则为必需 `true` 。</span><span class="sxs-lookup"><span data-stu-id="5b43d-183">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="5b43d-184">AllowCloudPasswordValidation</span><span class="sxs-lookup"><span data-stu-id="5b43d-184">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="5b43d-185">布尔值</span><span class="sxs-lookup"><span data-stu-id="5b43d-185">Boolean</span></span>| <span data-ttu-id="5b43d-186">设置为 `true` 以允许应用程序通过直接向 Azure Active Directory 令牌终结点提供用户名/密码凭据来对联合用户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="5b43d-186">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="5b43d-187">仅在启用密码哈希同步时才有效。</span><span class="sxs-lookup"><span data-stu-id="5b43d-187">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="5b43d-188">可选。</span><span class="sxs-lookup"><span data-stu-id="5b43d-188">Optional.</span></span>|
|<span data-ttu-id="5b43d-189">AlternateIdLogin</span><span class="sxs-lookup"><span data-stu-id="5b43d-189">AlternateIdLogin</span></span>| <span data-ttu-id="5b43d-190">Json</span><span class="sxs-lookup"><span data-stu-id="5b43d-190">Json</span></span> |<span data-ttu-id="5b43d-191">设置为 {"Enabled"： true} 以允许 Azure AD 登录使用电子邮件作为 [备用登录 ID](https://docs.microsoft.com/azure/active-directory/authentication/howto-authentication-use-email-signin)。</span><span class="sxs-lookup"><span data-stu-id="5b43d-191">Set to {"Enabled": true} to allow Azure AD sign-in using email as [an alternate login ID](https://docs.microsoft.com/azure/active-directory/authentication/howto-authentication-use-email-signin).</span></span> <span data-ttu-id="5b43d-192">仅在将 **IsOrganizationDefault** 设置为时起作用 `true` 。</span><span class="sxs-lookup"><span data-stu-id="5b43d-192">Only works when **IsOrganizationDefault** is set to `true`.</span></span> <span data-ttu-id="5b43d-193">可选。</span><span class="sxs-lookup"><span data-stu-id="5b43d-193">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b43d-194">关系</span><span class="sxs-lookup"><span data-stu-id="5b43d-194">Relationships</span></span>

| <span data-ttu-id="5b43d-195">关系</span><span class="sxs-lookup"><span data-stu-id="5b43d-195">Relationship</span></span> | <span data-ttu-id="5b43d-196">类型</span><span class="sxs-lookup"><span data-stu-id="5b43d-196">Type</span></span>        | <span data-ttu-id="5b43d-197">说明</span><span class="sxs-lookup"><span data-stu-id="5b43d-197">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5b43d-198">appliesTo</span><span class="sxs-lookup"><span data-stu-id="5b43d-198">appliesTo</span></span>|<span data-ttu-id="5b43d-199">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5b43d-199">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="5b43d-200">已将此策略应用于的 [directoryObject](directoryObject.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="5b43d-200">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="5b43d-201">只读。</span><span class="sxs-lookup"><span data-stu-id="5b43d-201">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b43d-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b43d-202">JSON representation</span></span>

<span data-ttu-id="5b43d-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b43d-203">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true,
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
