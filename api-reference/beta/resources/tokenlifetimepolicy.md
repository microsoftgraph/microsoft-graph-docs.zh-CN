---
title: tokenLifetimePolicy 资源类型
description: 表示一个可控制 Azure Active Directory 颁发的访问令牌的生存期的策略。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 721444335ee4787a34e6fefd26d7d8cde270851e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979306"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="b1edf-103">tokenLifetimePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1edf-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="b1edf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1edf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1edf-105">表示一个策略，该策略可以控制 JWT 访问令牌的有效期、Azure Active Directory (Azure AD) 颁发的 ID 令牌或 SAML 1.1/2.0 令牌。</span><span class="sxs-lookup"><span data-stu-id="b1edf-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="b1edf-106">您可以为组织中的所有应用程序、多租户 (多组织) 应用程序或组织中的特定服务主体设置令牌生存期。</span><span class="sxs-lookup"><span data-stu-id="b1edf-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="b1edf-107">有关更多方案的详细信息，请参阅 [Azure Active Directory 中的可配置令牌生存期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="b1edf-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="b1edf-108">注意：不支持为刷新令牌和会话令牌配置此策略。</span><span class="sxs-lookup"><span data-stu-id="b1edf-108">Note: Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="b1edf-109">继承自 [stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="b1edf-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b1edf-110">方法</span><span class="sxs-lookup"><span data-stu-id="b1edf-110">Methods</span></span>

| <span data-ttu-id="b1edf-111">方法</span><span class="sxs-lookup"><span data-stu-id="b1edf-111">Method</span></span>       | <span data-ttu-id="b1edf-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1edf-112">Return Type</span></span> | <span data-ttu-id="b1edf-113">说明</span><span class="sxs-lookup"><span data-stu-id="b1edf-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b1edf-114">创建 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b1edf-114">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="b1edf-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b1edf-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="b1edf-116">创建 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="b1edf-116">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="b1edf-117">获取 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b1edf-117">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="b1edf-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b1edf-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="b1edf-119">读取 tokenLifetimePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b1edf-119">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="b1edf-120">列出 tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="b1edf-120">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="b1edf-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b1edf-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="b1edf-122">读取 tokenLifetimePolicies 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b1edf-122">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="b1edf-123">更新 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b1edf-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="b1edf-124">无</span><span class="sxs-lookup"><span data-stu-id="b1edf-124">None</span></span> | <span data-ttu-id="b1edf-125">更新 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="b1edf-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="b1edf-126">删除 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b1edf-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="b1edf-127">无</span><span class="sxs-lookup"><span data-stu-id="b1edf-127">None</span></span> | <span data-ttu-id="b1edf-128">删除 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="b1edf-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="b1edf-129">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="b1edf-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="b1edf-130">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="b1edf-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="b1edf-131">获取已应用此策略的 directoryObjects 的列表。</span><span class="sxs-lookup"><span data-stu-id="b1edf-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="b1edf-132">分配 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b1edf-132">Assign tokenLifetimePolicy</span></span>](../api/application-post-tokenlifetimepolicies.md) | <span data-ttu-id="b1edf-133">无</span><span class="sxs-lookup"><span data-stu-id="b1edf-133">None</span></span> | <span data-ttu-id="b1edf-134">将 tokenLifetimePolicy 对象分配给 [application](application.md) 或 [servicePrincipal](serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1edf-134">Assign a tokenLifetimePolicy object to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="b1edf-135">列表已分配 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b1edf-135">List assigned tokenLifetimePolicy</span></span>](../api/application-list-tokenlifetimepolicies.md) | <span data-ttu-id="b1edf-136">[tokenLifetimePolicy](tokenlifetimepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b1edf-136">[tokenLifetimePolicy](tokenlifetimepolicy.md) collection</span></span> | <span data-ttu-id="b1edf-137">列出分配给 [application](application.md) 或 [ServicePrincipal](serviceprincipal.md) 对象的 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="b1edf-137">List the tokenLifetimePolicy objects that are assigned to an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="b1edf-138">删除 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b1edf-138">Remove tokenLifetimePolicy</span></span>](../api/application-delete-tokenlifetimepolicies.md) | <span data-ttu-id="b1edf-139">无</span><span class="sxs-lookup"><span data-stu-id="b1edf-139">None</span></span> | <span data-ttu-id="b1edf-140">从 [应用程序](application.md) 或 [servicePrincipal](serviceprincipal.md) 对象中删除 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="b1edf-140">Remove a tokenLifetimePolicy object from an [application](application.md) or [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b1edf-141">属性</span><span class="sxs-lookup"><span data-stu-id="b1edf-141">Properties</span></span>

| <span data-ttu-id="b1edf-142">属性</span><span class="sxs-lookup"><span data-stu-id="b1edf-142">Property</span></span>     | <span data-ttu-id="b1edf-143">类型</span><span class="sxs-lookup"><span data-stu-id="b1edf-143">Type</span></span>        | <span data-ttu-id="b1edf-144">说明</span><span class="sxs-lookup"><span data-stu-id="b1edf-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1edf-145">id</span><span class="sxs-lookup"><span data-stu-id="b1edf-145">id</span></span>|<span data-ttu-id="b1edf-146">String</span><span class="sxs-lookup"><span data-stu-id="b1edf-146">String</span></span>| <span data-ttu-id="b1edf-147">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b1edf-147">Unique identifier for this policy.</span></span> <span data-ttu-id="b1edf-148">只读。</span><span class="sxs-lookup"><span data-stu-id="b1edf-148">Read-only.</span></span>|
|<span data-ttu-id="b1edf-149">定义</span><span class="sxs-lookup"><span data-stu-id="b1edf-149">definition</span></span>|<span data-ttu-id="b1edf-150">String collection</span><span class="sxs-lookup"><span data-stu-id="b1edf-150">String collection</span></span>| <span data-ttu-id="b1edf-151">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="b1edf-151">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="b1edf-152">有关此属性的 JSON 架构的更多详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="b1edf-152">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="b1edf-153">必需。</span><span class="sxs-lookup"><span data-stu-id="b1edf-153">Required.</span></span>|
|<span data-ttu-id="b1edf-154">description</span><span class="sxs-lookup"><span data-stu-id="b1edf-154">description</span></span>|<span data-ttu-id="b1edf-155">String</span><span class="sxs-lookup"><span data-stu-id="b1edf-155">String</span></span>| <span data-ttu-id="b1edf-156">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="b1edf-156">Description for this policy.</span></span>|
|<span data-ttu-id="b1edf-157">displayName</span><span class="sxs-lookup"><span data-stu-id="b1edf-157">displayName</span></span>|<span data-ttu-id="b1edf-158">String</span><span class="sxs-lookup"><span data-stu-id="b1edf-158">String</span></span>| <span data-ttu-id="b1edf-159">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b1edf-159">Display name for this policy.</span></span> <span data-ttu-id="b1edf-160">必需。</span><span class="sxs-lookup"><span data-stu-id="b1edf-160">Required.</span></span>|
|<span data-ttu-id="b1edf-161">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="b1edf-161">isOrganizationDefault</span></span>|<span data-ttu-id="b1edf-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1edf-162">Boolean</span></span>|<span data-ttu-id="b1edf-163">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="b1edf-163">If set to true, activates this policy.</span></span> <span data-ttu-id="b1edf-164">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="b1edf-164">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="b1edf-165">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="b1edf-165">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="b1edf-166">令牌生存期策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="b1edf-166">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="b1edf-167">下面的属性构成了表示令牌生存期策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b1edf-167">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="b1edf-168">此 JSON 对象必须 **转换为转义了引号的字符串** ，以将其插入到 **定义** 属性中。</span><span class="sxs-lookup"><span data-stu-id="b1edf-168">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="b1edf-169">下面以 JSON 格式显示了一个示例：</span><span class="sxs-lookup"><span data-stu-id="b1edf-169">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="b1edf-170">注意：这些属性中的所有持续时间均以 "dd. hh： mm： ss" 的格式指定。</span><span class="sxs-lookup"><span data-stu-id="b1edf-170">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="b1edf-171">注意： "天" 中表示的属性的最大值是表示的天数的1秒。</span><span class="sxs-lookup"><span data-stu-id="b1edf-171">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="b1edf-172">例如，"最大值为1天" 指定为 "23:59:59"。</span><span class="sxs-lookup"><span data-stu-id="b1edf-172">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="b1edf-173">属性</span><span class="sxs-lookup"><span data-stu-id="b1edf-173">Property</span></span>     | <span data-ttu-id="b1edf-174">类型</span><span class="sxs-lookup"><span data-stu-id="b1edf-174">Type</span></span>   |<span data-ttu-id="b1edf-175">说明</span><span class="sxs-lookup"><span data-stu-id="b1edf-175">Description</span></span>| <span data-ttu-id="b1edf-176">最小值</span><span class="sxs-lookup"><span data-stu-id="b1edf-176">Min Value</span></span> | <span data-ttu-id="b1edf-177">最大值</span><span class="sxs-lookup"><span data-stu-id="b1edf-177">Max Value</span></span> | <span data-ttu-id="b1edf-178">默认值</span><span class="sxs-lookup"><span data-stu-id="b1edf-178">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="b1edf-179">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="b1edf-179">AccessTokenLifetime</span></span>|<span data-ttu-id="b1edf-180">String</span><span class="sxs-lookup"><span data-stu-id="b1edf-180">String</span></span>|<span data-ttu-id="b1edf-181">控制访问和 ID 令牌被视为有效的时间。</span><span class="sxs-lookup"><span data-stu-id="b1edf-181">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="b1edf-182">10 分钟</span><span class="sxs-lookup"><span data-stu-id="b1edf-182">10 minutes</span></span>|<span data-ttu-id="b1edf-183">1 天</span><span class="sxs-lookup"><span data-stu-id="b1edf-183">1 day</span></span>|<span data-ttu-id="b1edf-184">1 小时</span><span class="sxs-lookup"><span data-stu-id="b1edf-184">1 hour</span></span>|
|<span data-ttu-id="b1edf-185">版本</span><span class="sxs-lookup"><span data-stu-id="b1edf-185">Version</span></span>|<span data-ttu-id="b1edf-186">整数</span><span class="sxs-lookup"><span data-stu-id="b1edf-186">Integer</span></span>|<span data-ttu-id="b1edf-187">将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="b1edf-187">Set value of 1.</span></span> <span data-ttu-id="b1edf-188">必需。</span><span class="sxs-lookup"><span data-stu-id="b1edf-188">Required.</span></span>|<span data-ttu-id="b1edf-189">无</span><span class="sxs-lookup"><span data-stu-id="b1edf-189">None</span></span>|<span data-ttu-id="b1edf-190">无</span><span class="sxs-lookup"><span data-stu-id="b1edf-190">None</span></span>|<span data-ttu-id="b1edf-191">无</span><span class="sxs-lookup"><span data-stu-id="b1edf-191">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1edf-192">关系</span><span class="sxs-lookup"><span data-stu-id="b1edf-192">Relationships</span></span>

| <span data-ttu-id="b1edf-193">关系</span><span class="sxs-lookup"><span data-stu-id="b1edf-193">Relationship</span></span> | <span data-ttu-id="b1edf-194">类型</span><span class="sxs-lookup"><span data-stu-id="b1edf-194">Type</span></span>        | <span data-ttu-id="b1edf-195">说明</span><span class="sxs-lookup"><span data-stu-id="b1edf-195">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1edf-196">appliesTo</span><span class="sxs-lookup"><span data-stu-id="b1edf-196">appliesTo</span></span>|<span data-ttu-id="b1edf-197">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="b1edf-197">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="b1edf-198">已将此策略应用于的 [directoryObject](directoryObject.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="b1edf-198">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="b1edf-199">只读。</span><span class="sxs-lookup"><span data-stu-id="b1edf-199">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1edf-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1edf-200">JSON representation</span></span>

<span data-ttu-id="b1edf-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1edf-201">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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
  "description": "tokenLifetimePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

