---
title: homeRealmDiscoveryPolicy 资源类型
description: 表示用于控制联合用户的 Azure Active Directory 身份验证行为的策略。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62b0735fbf7d927cf7ee417a81a54a8cb5eb2473
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234197"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a><span data-ttu-id="b7d18-103">homeRealmDiscoveryPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7d18-103">homeRealmDiscoveryPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7d18-104">表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略，尤其适用于联合域中的自动加速和用户身份验证限制。</span><span class="sxs-lookup"><span data-stu-id="b7d18-104">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span> <span data-ttu-id="b7d18-105">您可以为组织中的所有服务主体或组织中的特定服务主体设置 homeRealmDiscoveryPolicy。</span><span class="sxs-lookup"><span data-stu-id="b7d18-105">You can set homeRealmDiscoveryPolicy for all service principals in your organization, or for specific service principals in your organization.</span></span>  <span data-ttu-id="b7d18-106">有关详细方案和策略的详细信息，请参阅[使用主领域发现策略为应用程序配置 AZURE AD 登录行为](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal)。</span><span class="sxs-lookup"><span data-stu-id="b7d18-106">For more scenario and policy details see [Configure Azure AD sign in behavior for an application by using a Home Realm Discovery policy](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).</span></span>

<span data-ttu-id="b7d18-107">继承自[stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="b7d18-107">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b7d18-108">方法</span><span class="sxs-lookup"><span data-stu-id="b7d18-108">Methods</span></span>

| <span data-ttu-id="b7d18-109">方法</span><span class="sxs-lookup"><span data-stu-id="b7d18-109">Method</span></span>       | <span data-ttu-id="b7d18-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b7d18-110">Return Type</span></span> | <span data-ttu-id="b7d18-111">说明</span><span class="sxs-lookup"><span data-stu-id="b7d18-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b7d18-112">创建 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b7d18-112">Create homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [<span data-ttu-id="b7d18-113">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b7d18-113">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="b7d18-114">创建 homeRealmDiscoveryPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="b7d18-114">Create a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b7d18-115">获取 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b7d18-115">Get homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-get.md) | [<span data-ttu-id="b7d18-116">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b7d18-116">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="b7d18-117">读取 homeRealmDiscoveryPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7d18-117">Read properties and relationships of a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b7d18-118">列出 homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="b7d18-118">List homeRealmDiscoveryPolicies</span></span>](../api/homerealmdiscoverypolicy-list.md) | [<span data-ttu-id="b7d18-119">homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b7d18-119">homeRealmDiscoveryPolicy</span></span>](homerealmdiscoverypolicy.md) | <span data-ttu-id="b7d18-120">读取 homeRealmDiscoveryPolicies 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7d18-120">Read properties and relationships of homeRealmDiscoveryPolicies objects.</span></span> |
| [<span data-ttu-id="b7d18-121">更新 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b7d18-121">Update homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-update.md) | <span data-ttu-id="b7d18-122">无</span><span class="sxs-lookup"><span data-stu-id="b7d18-122">None</span></span> | <span data-ttu-id="b7d18-123">更新 homeRealmDiscoveryPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="b7d18-123">Update a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b7d18-124">删除 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b7d18-124">Delete homeRealmDiscoveryPolicy</span></span>](../api/homerealmdiscoverypolicy-delete.md) | <span data-ttu-id="b7d18-125">无</span><span class="sxs-lookup"><span data-stu-id="b7d18-125">None</span></span> | <span data-ttu-id="b7d18-126">删除 homeRealmDiscoveryPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="b7d18-126">Delete a homeRealmDiscoveryPolicy object.</span></span> |
| [<span data-ttu-id="b7d18-127">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="b7d18-127">List appliesTo</span></span>](../api/homerealmdiscoverypolicy-list-appliesto.md) | <span data-ttu-id="b7d18-128">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="b7d18-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="b7d18-129">获取已应用此策略的 directoryObjects 的列表。</span><span class="sxs-lookup"><span data-stu-id="b7d18-129">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="b7d18-130">属性</span><span class="sxs-lookup"><span data-stu-id="b7d18-130">Properties</span></span>

| <span data-ttu-id="b7d18-131">属性</span><span class="sxs-lookup"><span data-stu-id="b7d18-131">Property</span></span>     | <span data-ttu-id="b7d18-132">类型</span><span class="sxs-lookup"><span data-stu-id="b7d18-132">Type</span></span>        | <span data-ttu-id="b7d18-133">说明</span><span class="sxs-lookup"><span data-stu-id="b7d18-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b7d18-134">id</span><span class="sxs-lookup"><span data-stu-id="b7d18-134">id</span></span>|<span data-ttu-id="b7d18-135">字符串</span><span class="sxs-lookup"><span data-stu-id="b7d18-135">String</span></span>| <span data-ttu-id="b7d18-136">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b7d18-136">Unique identifier for this policy.</span></span> <span data-ttu-id="b7d18-137">只读。</span><span class="sxs-lookup"><span data-stu-id="b7d18-137">Read-only.</span></span>|
|<span data-ttu-id="b7d18-138">定义</span><span class="sxs-lookup"><span data-stu-id="b7d18-138">definition</span></span>|<span data-ttu-id="b7d18-139">String collection</span><span class="sxs-lookup"><span data-stu-id="b7d18-139">String collection</span></span>| <span data-ttu-id="b7d18-140">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="b7d18-140">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="b7d18-141">有关此属性的 JSON 架构的更多详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="b7d18-141">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="b7d18-142">必需。</span><span class="sxs-lookup"><span data-stu-id="b7d18-142">Required.</span></span>|
|<span data-ttu-id="b7d18-143">description</span><span class="sxs-lookup"><span data-stu-id="b7d18-143">description</span></span>|<span data-ttu-id="b7d18-144">String</span><span class="sxs-lookup"><span data-stu-id="b7d18-144">String</span></span>| <span data-ttu-id="b7d18-145">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="b7d18-145">Description for this policy.</span></span>|
|<span data-ttu-id="b7d18-146">displayName</span><span class="sxs-lookup"><span data-stu-id="b7d18-146">displayName</span></span>|<span data-ttu-id="b7d18-147">String</span><span class="sxs-lookup"><span data-stu-id="b7d18-147">String</span></span>| <span data-ttu-id="b7d18-148">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b7d18-148">Display name for this policy.</span></span> <span data-ttu-id="b7d18-149">必需。</span><span class="sxs-lookup"><span data-stu-id="b7d18-149">Required.</span></span>|
|<span data-ttu-id="b7d18-150">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="b7d18-150">isOrganizationDefault</span></span>|<span data-ttu-id="b7d18-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7d18-151">Boolean</span></span>|<span data-ttu-id="b7d18-152">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="b7d18-152">If set to true, activates this policy.</span></span> <span data-ttu-id="b7d18-153">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="b7d18-153">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="b7d18-154">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="b7d18-154">Optional, default value is false.</span></span>|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a><span data-ttu-id="b7d18-155">主领域发现策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="b7d18-155">Properties of a home realm discovery policy definition</span></span>
<span data-ttu-id="b7d18-156">下面的属性构成了表示令牌生存期策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b7d18-156">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="b7d18-157">此 JSON 对象必须**转换为转义了引号的字符串**，以将其插入到**定义**属性中。</span><span class="sxs-lookup"><span data-stu-id="b7d18-157">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="b7d18-158">下面以 JSON 格式显示了一个示例：</span><span class="sxs-lookup"><span data-stu-id="b7d18-158">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"HomeRealmDiscoveryPolicy\":
     {\"AccelerateToFederatedDomain\":true,
      \"PreferredDomain\":\"federated.example.edu\"}}"
  ]
```

| <span data-ttu-id="b7d18-159">属性</span><span class="sxs-lookup"><span data-stu-id="b7d18-159">Property</span></span>     | <span data-ttu-id="b7d18-160">类型</span><span class="sxs-lookup"><span data-stu-id="b7d18-160">Type</span></span>   |<span data-ttu-id="b7d18-161">说明</span><span class="sxs-lookup"><span data-stu-id="b7d18-161">Description</span></span>| 
|:---------------|:--------|:----------|
|<span data-ttu-id="b7d18-162">AccelerateToFederatedDomain</span><span class="sxs-lookup"><span data-stu-id="b7d18-162">AccelerateToFederatedDomain</span></span>|<span data-ttu-id="b7d18-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7d18-163">Boolean</span></span>| <span data-ttu-id="b7d18-164">设置为`true`以进行自动加速（绕过主页领域发现）。</span><span class="sxs-lookup"><span data-stu-id="b7d18-164">Set to `true` for auto-acceleration (bypass home realm discovery).</span></span> <span data-ttu-id="b7d18-165">如果`true`在租户中只有一个经过验证和联合的域，则用户将直接转到联合身份提供程序（如 ADFS）以进行登录。</span><span class="sxs-lookup"><span data-stu-id="b7d18-165">If `true` and there is only one verified and federated domain in the tenant, then users will be taken straight to the federated identity provider (such as ADFS) for sign in.</span></span> <span data-ttu-id="b7d18-166">如果`true`租户中有多个已验证的域，则必须指定**PreferredDomain** 。</span><span class="sxs-lookup"><span data-stu-id="b7d18-166">If `true` and there is more than one verified domain in the tenant, **PreferredDomain** must be specified.</span></span> <span data-ttu-id="b7d18-167">可选。</span><span class="sxs-lookup"><span data-stu-id="b7d18-167">Optional.</span></span>|
|<span data-ttu-id="b7d18-168">PreferredDomain</span><span class="sxs-lookup"><span data-stu-id="b7d18-168">PreferredDomain</span></span>|<span data-ttu-id="b7d18-169">String</span><span class="sxs-lookup"><span data-stu-id="b7d18-169">String</span></span>| <span data-ttu-id="b7d18-170">指定要加速登录到的域。</span><span class="sxs-lookup"><span data-stu-id="b7d18-170">Specifies a domain to accelerate sign-in to.</span></span> <span data-ttu-id="b7d18-171">如果租户只有一个联合域，则可以省略它。</span><span class="sxs-lookup"><span data-stu-id="b7d18-171">It can be omitted if the tenant has only one federated domain.</span></span> <span data-ttu-id="b7d18-172">如果省略它，并且有多个经过验证的联合域，则此策略将不起作用。</span><span class="sxs-lookup"><span data-stu-id="b7d18-172">If it is omitted, and there is more than one verified federated domain, this policy has no effect.</span></span> <span data-ttu-id="b7d18-173">如果**AccelerateToFederatedDomain**为， `true`则为必需。</span><span class="sxs-lookup"><span data-stu-id="b7d18-173">Required if **AccelerateToFederatedDomain** is `true`.</span></span>|
|<span data-ttu-id="b7d18-174">AllowCloudPasswordValidation</span><span class="sxs-lookup"><span data-stu-id="b7d18-174">AllowCloudPasswordValidation</span></span>|<span data-ttu-id="b7d18-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7d18-175">Boolean</span></span>| <span data-ttu-id="b7d18-176">设置为`true`以允许应用程序通过直接向 Azure Active Directory 令牌终结点提供用户名/密码凭据来对联合用户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="b7d18-176">Set to `true` to allow an application to authenticate a federated user by presenting username/password credentials directly to the Azure Active Directory token endpoint.</span></span> <span data-ttu-id="b7d18-177">仅在启用密码哈希同步时才有效。</span><span class="sxs-lookup"><span data-stu-id="b7d18-177">Only works if Password Hash Sync is enabled.</span></span> <span data-ttu-id="b7d18-178">可选。</span><span class="sxs-lookup"><span data-stu-id="b7d18-178">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7d18-179">关系</span><span class="sxs-lookup"><span data-stu-id="b7d18-179">Relationships</span></span>

| <span data-ttu-id="b7d18-180">关系</span><span class="sxs-lookup"><span data-stu-id="b7d18-180">Relationship</span></span> | <span data-ttu-id="b7d18-181">类型</span><span class="sxs-lookup"><span data-stu-id="b7d18-181">Type</span></span>        | <span data-ttu-id="b7d18-182">说明</span><span class="sxs-lookup"><span data-stu-id="b7d18-182">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b7d18-183">appliesTo</span><span class="sxs-lookup"><span data-stu-id="b7d18-183">appliesTo</span></span>|<span data-ttu-id="b7d18-184">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="b7d18-184">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="b7d18-185">已将此策略应用于的[directoryObject](directoryObject.md)集合。</span><span class="sxs-lookup"><span data-stu-id="b7d18-185">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="b7d18-186">只读。</span><span class="sxs-lookup"><span data-stu-id="b7d18-186">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7d18-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7d18-187">JSON representation</span></span>

<span data-ttu-id="b7d18-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7d18-188">The following is a JSON representation of the resource.</span></span>

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