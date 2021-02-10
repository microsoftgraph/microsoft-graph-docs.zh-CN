---
title: tokenLifetimePolicy 资源类型
description: 表示可以控制 Azure Active Directory 颁发的访问令牌的生存期的策略。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b9b9f75e55c027ecee0189b4ace2fd52e3d10e78
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158077"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="5cb8a-103">tokenLifetimePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cb8a-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="5cb8a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cb8a-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="5cb8a-105">表示可控制 JWT 访问令牌、ID 令牌或 Azure Active Directory (Azure AD) 颁发的 SAML 1.1/2.0 令牌的生命周期的策略。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="5cb8a-106">可以为组织中的所有应用程序、多租户（多组织）应用程序或组织中的特定服务主体设置令牌生存期。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span>  <span data-ttu-id="5cb8a-107">有关更多方案的详细信息，请参阅 [Azure Active Directory 中的可配置令牌生存期](/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-107">For more scenario details see [Configurable token lifetimes in Azure Active Directory](/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

><span data-ttu-id="5cb8a-108">**注意：** 不支持为刷新令牌和会话令牌配置此策略。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-108">**Note:** Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="5cb8a-109">继承自 [stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-109">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5cb8a-110">方法</span><span class="sxs-lookup"><span data-stu-id="5cb8a-110">Methods</span></span>

| <span data-ttu-id="5cb8a-111">方法</span><span class="sxs-lookup"><span data-stu-id="5cb8a-111">Method</span></span>       | <span data-ttu-id="5cb8a-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="5cb8a-112">Return Type</span></span> | <span data-ttu-id="5cb8a-113">说明</span><span class="sxs-lookup"><span data-stu-id="5cb8a-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5cb8a-114">列出 tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="5cb8a-114">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="5cb8a-115">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="5cb8a-115">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="5cb8a-116">读取 tokenLifetimePolicies 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-116">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="5cb8a-117">创建 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="5cb8a-117">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="5cb8a-118">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="5cb8a-118">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="5cb8a-119">创建 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-119">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="5cb8a-120">获取 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="5cb8a-120">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="5cb8a-121">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="5cb8a-121">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="5cb8a-122">读取 tokenLifetimePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-122">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="5cb8a-123">更新 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="5cb8a-123">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="5cb8a-124">无</span><span class="sxs-lookup"><span data-stu-id="5cb8a-124">None</span></span> | <span data-ttu-id="5cb8a-125">更新 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-125">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="5cb8a-126">删除 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="5cb8a-126">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="5cb8a-127">无</span><span class="sxs-lookup"><span data-stu-id="5cb8a-127">None</span></span> | <span data-ttu-id="5cb8a-128">删除 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-128">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="5cb8a-129">List appliesTo</span><span class="sxs-lookup"><span data-stu-id="5cb8a-129">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="5cb8a-130">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5cb8a-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="5cb8a-131">获取已应用此策略的 directoryObjects 列表。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-131">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="5cb8a-132">属性</span><span class="sxs-lookup"><span data-stu-id="5cb8a-132">Properties</span></span>

| <span data-ttu-id="5cb8a-133">属性</span><span class="sxs-lookup"><span data-stu-id="5cb8a-133">Property</span></span>     | <span data-ttu-id="5cb8a-134">类型</span><span class="sxs-lookup"><span data-stu-id="5cb8a-134">Type</span></span>        | <span data-ttu-id="5cb8a-135">说明</span><span class="sxs-lookup"><span data-stu-id="5cb8a-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5cb8a-136">id</span><span class="sxs-lookup"><span data-stu-id="5cb8a-136">id</span></span>|<span data-ttu-id="5cb8a-137">String</span><span class="sxs-lookup"><span data-stu-id="5cb8a-137">String</span></span>| <span data-ttu-id="5cb8a-138">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-138">Unique identifier for this policy.</span></span> <span data-ttu-id="5cb8a-139">只读。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-139">Read-only.</span></span>|
|<span data-ttu-id="5cb8a-140">definition</span><span class="sxs-lookup"><span data-stu-id="5cb8a-140">definition</span></span>|<span data-ttu-id="5cb8a-141">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5cb8a-141">String collection</span></span>| <span data-ttu-id="5cb8a-142">包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-142">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="5cb8a-143">有关此属性的 JSON 架构的更多详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-143">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="5cb8a-144">必需。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-144">Required.</span></span>|
|<span data-ttu-id="5cb8a-145">description</span><span class="sxs-lookup"><span data-stu-id="5cb8a-145">description</span></span>|<span data-ttu-id="5cb8a-146">String</span><span class="sxs-lookup"><span data-stu-id="5cb8a-146">String</span></span>| <span data-ttu-id="5cb8a-147">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-147">Description for this policy.</span></span>|
|<span data-ttu-id="5cb8a-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5cb8a-148">displayName</span></span>|<span data-ttu-id="5cb8a-149">String</span><span class="sxs-lookup"><span data-stu-id="5cb8a-149">String</span></span>| <span data-ttu-id="5cb8a-150">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-150">Display name for this policy.</span></span> <span data-ttu-id="5cb8a-151">必需。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-151">Required.</span></span>|
|<span data-ttu-id="5cb8a-152">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="5cb8a-152">isOrganizationDefault</span></span>|<span data-ttu-id="5cb8a-153">布尔值</span><span class="sxs-lookup"><span data-stu-id="5cb8a-153">Boolean</span></span>|<span data-ttu-id="5cb8a-154">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-154">If set to true, activates this policy.</span></span> <span data-ttu-id="5cb8a-155">同一策略类型可以有很多策略，但只有一个策略可以激活为组织默认策略。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-155">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="5cb8a-156">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-156">Optional, default value is false.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="5cb8a-157">令牌生存期策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="5cb8a-157">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="5cb8a-158">以下属性构成表示令牌生存期策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-158">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="5cb8a-159">此 JSON 对象 **必须转换为** 带转义引号的字符串，以插入到 **定义** 属性中。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="5cb8a-160">下面显示了 JSON 格式的示例：</span><span class="sxs-lookup"><span data-stu-id="5cb8a-160">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="5cb8a-161">**注意：** 这些属性的所有持续时间都以"dd.hh：mm：ss"格式指定。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-161">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="5cb8a-162">**注意：** 用"days"表示的属性的最大值比表示的天数短 1 秒。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-162">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="5cb8a-163">例如，最大值 1 天指定为"23：59：59"。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-163">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="5cb8a-164">属性</span><span class="sxs-lookup"><span data-stu-id="5cb8a-164">Property</span></span>     | <span data-ttu-id="5cb8a-165">类型</span><span class="sxs-lookup"><span data-stu-id="5cb8a-165">Type</span></span>   |<span data-ttu-id="5cb8a-166">说明</span><span class="sxs-lookup"><span data-stu-id="5cb8a-166">Description</span></span>| <span data-ttu-id="5cb8a-167">最小值</span><span class="sxs-lookup"><span data-stu-id="5cb8a-167">Min Value</span></span> | <span data-ttu-id="5cb8a-168">最大值</span><span class="sxs-lookup"><span data-stu-id="5cb8a-168">Max Value</span></span> | <span data-ttu-id="5cb8a-169">默认值</span><span class="sxs-lookup"><span data-stu-id="5cb8a-169">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="5cb8a-170">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="5cb8a-170">AccessTokenLifetime</span></span>|<span data-ttu-id="5cb8a-171">String</span><span class="sxs-lookup"><span data-stu-id="5cb8a-171">String</span></span>|<span data-ttu-id="5cb8a-172">控制访问令牌和 ID 令牌都被视为有效的时间。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-172">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="5cb8a-173">10 分钟</span><span class="sxs-lookup"><span data-stu-id="5cb8a-173">10 minutes</span></span>|<span data-ttu-id="5cb8a-174">1 天</span><span class="sxs-lookup"><span data-stu-id="5cb8a-174">1 day</span></span>|<span data-ttu-id="5cb8a-175">1 小时</span><span class="sxs-lookup"><span data-stu-id="5cb8a-175">1 hour</span></span>|
|<span data-ttu-id="5cb8a-176">版本</span><span class="sxs-lookup"><span data-stu-id="5cb8a-176">Version</span></span>|<span data-ttu-id="5cb8a-177">整数</span><span class="sxs-lookup"><span data-stu-id="5cb8a-177">Integer</span></span>|<span data-ttu-id="5cb8a-178">将值设置为 1。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-178">Set value of 1.</span></span> <span data-ttu-id="5cb8a-179">必需。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-179">Required.</span></span>|<span data-ttu-id="5cb8a-180">无</span><span class="sxs-lookup"><span data-stu-id="5cb8a-180">None</span></span>|<span data-ttu-id="5cb8a-181">无</span><span class="sxs-lookup"><span data-stu-id="5cb8a-181">None</span></span>|<span data-ttu-id="5cb8a-182">无</span><span class="sxs-lookup"><span data-stu-id="5cb8a-182">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cb8a-183">关系</span><span class="sxs-lookup"><span data-stu-id="5cb8a-183">Relationships</span></span>

| <span data-ttu-id="5cb8a-184">关系</span><span class="sxs-lookup"><span data-stu-id="5cb8a-184">Relationship</span></span> | <span data-ttu-id="5cb8a-185">类型</span><span class="sxs-lookup"><span data-stu-id="5cb8a-185">Type</span></span>        | <span data-ttu-id="5cb8a-186">说明</span><span class="sxs-lookup"><span data-stu-id="5cb8a-186">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5cb8a-187">appliesTo</span><span class="sxs-lookup"><span data-stu-id="5cb8a-187">appliesTo</span></span>|<span data-ttu-id="5cb8a-188">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5cb8a-188">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="5cb8a-189">已 [应用此策略的 directoryObject](directoryObject.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-189">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="5cb8a-190">只读。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-190">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5cb8a-191">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cb8a-191">JSON representation</span></span>

<span data-ttu-id="5cb8a-192">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cb8a-192">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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