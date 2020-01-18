---
title: tokenLifetimePolicy 资源类型
description: 表示一个可控制 Azure Active Directory 颁发的访问令牌的生存期的策略。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a19ec9e2b8747737895bed89b1a92ec4c5d134a
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234194"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="cb02c-103">tokenLifetimePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb02c-103">tokenLifetimePolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb02c-104">表示一个策略，该策略可以控制 JWT 访问令牌的有效期、由 Azure Active Directory （Azure AD）颁发的 ID 令牌或 SAML 1.1/2.0 令牌。</span><span class="sxs-lookup"><span data-stu-id="cb02c-104">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="cb02c-105">您可以为组织中的所有应用、多租户（多组织）应用程序或组织中的特定服务主体设置令牌生存期。</span><span class="sxs-lookup"><span data-stu-id="cb02c-105">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="cb02c-106">有关更多方案的详细信息，请参阅[Azure Active Directory 中的可配置令牌生存期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="cb02c-106">For more scenario details see [Configurable token lifetimes in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="cb02c-107">注意：不支持为刷新令牌和会话令牌配置此策略。</span><span class="sxs-lookup"><span data-stu-id="cb02c-107">Note: Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="cb02c-108">继承自[stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="cb02c-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cb02c-109">方法</span><span class="sxs-lookup"><span data-stu-id="cb02c-109">Methods</span></span>

| <span data-ttu-id="cb02c-110">方法</span><span class="sxs-lookup"><span data-stu-id="cb02c-110">Method</span></span>       | <span data-ttu-id="cb02c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="cb02c-111">Return Type</span></span> | <span data-ttu-id="cb02c-112">说明</span><span class="sxs-lookup"><span data-stu-id="cb02c-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cb02c-113">创建 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="cb02c-113">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="cb02c-114">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="cb02c-114">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="cb02c-115">创建 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="cb02c-115">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="cb02c-116">获取 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="cb02c-116">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="cb02c-117">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="cb02c-117">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="cb02c-118">读取 tokenLifetimePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb02c-118">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="cb02c-119">列出 tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="cb02c-119">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="cb02c-120">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="cb02c-120">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="cb02c-121">读取 tokenLifetimePolicies 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb02c-121">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="cb02c-122">更新 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="cb02c-122">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="cb02c-123">无</span><span class="sxs-lookup"><span data-stu-id="cb02c-123">None</span></span> | <span data-ttu-id="cb02c-124">更新 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="cb02c-124">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="cb02c-125">删除 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="cb02c-125">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="cb02c-126">无</span><span class="sxs-lookup"><span data-stu-id="cb02c-126">None</span></span> | <span data-ttu-id="cb02c-127">删除 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="cb02c-127">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="cb02c-128">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="cb02c-128">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="cb02c-129">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="cb02c-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="cb02c-130">获取已应用此策略的 directoryObjects 的列表。</span><span class="sxs-lookup"><span data-stu-id="cb02c-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="cb02c-131">属性</span><span class="sxs-lookup"><span data-stu-id="cb02c-131">Properties</span></span>

| <span data-ttu-id="cb02c-132">属性</span><span class="sxs-lookup"><span data-stu-id="cb02c-132">Property</span></span>     | <span data-ttu-id="cb02c-133">类型</span><span class="sxs-lookup"><span data-stu-id="cb02c-133">Type</span></span>        | <span data-ttu-id="cb02c-134">说明</span><span class="sxs-lookup"><span data-stu-id="cb02c-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb02c-135">id</span><span class="sxs-lookup"><span data-stu-id="cb02c-135">id</span></span>|<span data-ttu-id="cb02c-136">字符串</span><span class="sxs-lookup"><span data-stu-id="cb02c-136">String</span></span>| <span data-ttu-id="cb02c-137">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cb02c-137">Unique identifier for this policy.</span></span> <span data-ttu-id="cb02c-138">只读。</span><span class="sxs-lookup"><span data-stu-id="cb02c-138">Read-only.</span></span>|
|<span data-ttu-id="cb02c-139">定义</span><span class="sxs-lookup"><span data-stu-id="cb02c-139">definition</span></span>|<span data-ttu-id="cb02c-140">String collection</span><span class="sxs-lookup"><span data-stu-id="cb02c-140">String collection</span></span>| <span data-ttu-id="cb02c-141">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="cb02c-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="cb02c-142">有关此属性的 JSON 架构的更多详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="cb02c-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="cb02c-143">必需。</span><span class="sxs-lookup"><span data-stu-id="cb02c-143">Required.</span></span>|
|<span data-ttu-id="cb02c-144">description</span><span class="sxs-lookup"><span data-stu-id="cb02c-144">description</span></span>|<span data-ttu-id="cb02c-145">String</span><span class="sxs-lookup"><span data-stu-id="cb02c-145">String</span></span>| <span data-ttu-id="cb02c-146">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="cb02c-146">Description for this policy.</span></span>|
|<span data-ttu-id="cb02c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cb02c-147">displayName</span></span>|<span data-ttu-id="cb02c-148">String</span><span class="sxs-lookup"><span data-stu-id="cb02c-148">String</span></span>| <span data-ttu-id="cb02c-149">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cb02c-149">Display name for this policy.</span></span> <span data-ttu-id="cb02c-150">必需。</span><span class="sxs-lookup"><span data-stu-id="cb02c-150">Required.</span></span>|
|<span data-ttu-id="cb02c-151">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="cb02c-151">isOrganizationDefault</span></span>|<span data-ttu-id="cb02c-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb02c-152">Boolean</span></span>|<span data-ttu-id="cb02c-153">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="cb02c-153">If set to true, activates this policy.</span></span> <span data-ttu-id="cb02c-154">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="cb02c-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="cb02c-155">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="cb02c-155">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="cb02c-156">令牌生存期策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="cb02c-156">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="cb02c-157">下面的属性构成了表示令牌生存期策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cb02c-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="cb02c-158">此 JSON 对象必须**转换为转义了引号的字符串**，以将其插入到**定义**属性中。</span><span class="sxs-lookup"><span data-stu-id="cb02c-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="cb02c-159">下面以 JSON 格式显示了一个示例：</span><span class="sxs-lookup"><span data-stu-id="cb02c-159">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="cb02c-160">注意：这些属性中的所有持续时间均以 "dd. hh： mm： ss" 的格式指定。</span><span class="sxs-lookup"><span data-stu-id="cb02c-160">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="cb02c-161">注意： "天" 中表示的属性的最大值是表示的天数的1秒。</span><span class="sxs-lookup"><span data-stu-id="cb02c-161">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="cb02c-162">例如，"最大值为1天" 指定为 "23:59:59"。</span><span class="sxs-lookup"><span data-stu-id="cb02c-162">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="cb02c-163">属性</span><span class="sxs-lookup"><span data-stu-id="cb02c-163">Property</span></span>     | <span data-ttu-id="cb02c-164">类型</span><span class="sxs-lookup"><span data-stu-id="cb02c-164">Type</span></span>   |<span data-ttu-id="cb02c-165">说明</span><span class="sxs-lookup"><span data-stu-id="cb02c-165">Description</span></span>| <span data-ttu-id="cb02c-166">最小值</span><span class="sxs-lookup"><span data-stu-id="cb02c-166">Min Value</span></span> | <span data-ttu-id="cb02c-167">最大值</span><span class="sxs-lookup"><span data-stu-id="cb02c-167">Max Value</span></span> | <span data-ttu-id="cb02c-168">默认值</span><span class="sxs-lookup"><span data-stu-id="cb02c-168">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="cb02c-169">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="cb02c-169">AccessTokenLifetime</span></span>|<span data-ttu-id="cb02c-170">String</span><span class="sxs-lookup"><span data-stu-id="cb02c-170">String</span></span>|<span data-ttu-id="cb02c-171">控制访问和 ID 令牌被视为有效的时间。</span><span class="sxs-lookup"><span data-stu-id="cb02c-171">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="cb02c-172">10 分钟</span><span class="sxs-lookup"><span data-stu-id="cb02c-172">10 minutes</span></span>|<span data-ttu-id="cb02c-173">1 天</span><span class="sxs-lookup"><span data-stu-id="cb02c-173">1 day</span></span>|<span data-ttu-id="cb02c-174">1 hour</span><span class="sxs-lookup"><span data-stu-id="cb02c-174">1 hour</span></span>|
|<span data-ttu-id="cb02c-175">版本</span><span class="sxs-lookup"><span data-stu-id="cb02c-175">Version</span></span>|<span data-ttu-id="cb02c-176">整数</span><span class="sxs-lookup"><span data-stu-id="cb02c-176">Integer</span></span>|<span data-ttu-id="cb02c-177">将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="cb02c-177">Set value of 1.</span></span> <span data-ttu-id="cb02c-178">必需。</span><span class="sxs-lookup"><span data-stu-id="cb02c-178">Required.</span></span>|<span data-ttu-id="cb02c-179">无</span><span class="sxs-lookup"><span data-stu-id="cb02c-179">None</span></span>|<span data-ttu-id="cb02c-180">无</span><span class="sxs-lookup"><span data-stu-id="cb02c-180">None</span></span>|<span data-ttu-id="cb02c-181">无</span><span class="sxs-lookup"><span data-stu-id="cb02c-181">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb02c-182">关系</span><span class="sxs-lookup"><span data-stu-id="cb02c-182">Relationships</span></span>

| <span data-ttu-id="cb02c-183">关系</span><span class="sxs-lookup"><span data-stu-id="cb02c-183">Relationship</span></span> | <span data-ttu-id="cb02c-184">类型</span><span class="sxs-lookup"><span data-stu-id="cb02c-184">Type</span></span>        | <span data-ttu-id="cb02c-185">说明</span><span class="sxs-lookup"><span data-stu-id="cb02c-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb02c-186">appliesTo</span><span class="sxs-lookup"><span data-stu-id="cb02c-186">appliesTo</span></span>|<span data-ttu-id="cb02c-187">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="cb02c-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="cb02c-188">已将此策略应用于的[directoryObject](directoryObject.md)集合。</span><span class="sxs-lookup"><span data-stu-id="cb02c-188">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="cb02c-189">只读。</span><span class="sxs-lookup"><span data-stu-id="cb02c-189">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb02c-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb02c-190">JSON representation</span></span>

<span data-ttu-id="cb02c-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb02c-191">The following is a JSON representation of the resource.</span></span>

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