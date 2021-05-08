---
title: tokenLifetimePolicy 资源类型
description: 表示一个策略，该策略可以控制由用户颁发的访问Azure Active Directory。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d143faa87af81fbaae73973510bafe3fd3ee4fcb
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241042"
---
# <a name="tokenlifetimepolicy-resource-type"></a><span data-ttu-id="fd4f5-103">tokenLifetimePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd4f5-103">tokenLifetimePolicy resource type</span></span>

<span data-ttu-id="fd4f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd4f5-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="fd4f5-105">表示可以控制 JWT 访问令牌、ID 令牌或由 Azure AD Azure Active Directory (颁发的 SAML 1.1/2.0) 。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-105">Represents a policy that can control the lifetime of a JWT access token, an ID token or a SAML 1.1/2.0 token issued by Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="fd4f5-106">可以为组织中的所有应用程序、多租户（多组织）应用程序或组织中的特定服务主体设置令牌生存期。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-106">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> 

><span data-ttu-id="fd4f5-107">**注意：** 不支持为刷新令牌和会话令牌配置此策略。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-107">**Note:** Configuring this policy for Refresh Tokens and Session Tokens is not supported.</span></span>

<span data-ttu-id="fd4f5-108">继承自 [stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fd4f5-109">方法</span><span class="sxs-lookup"><span data-stu-id="fd4f5-109">Methods</span></span>

| <span data-ttu-id="fd4f5-110">方法</span><span class="sxs-lookup"><span data-stu-id="fd4f5-110">Method</span></span>       | <span data-ttu-id="fd4f5-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="fd4f5-111">Return Type</span></span> | <span data-ttu-id="fd4f5-112">说明</span><span class="sxs-lookup"><span data-stu-id="fd4f5-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fd4f5-113">列出 tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="fd4f5-113">List tokenLifetimePolicies</span></span>](../api/tokenlifetimepolicy-list.md) | [<span data-ttu-id="fd4f5-114">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="fd4f5-114">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="fd4f5-115">读取 tokenLifetimePolicies 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-115">Read properties and relationships of tokenLifetimePolicies objects.</span></span> |
| [<span data-ttu-id="fd4f5-116">创建 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="fd4f5-116">Create tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [<span data-ttu-id="fd4f5-117">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="fd4f5-117">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="fd4f5-118">创建 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-118">Create a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="fd4f5-119">获取 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="fd4f5-119">Get tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-get.md) | [<span data-ttu-id="fd4f5-120">tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="fd4f5-120">tokenLifetimePolicy</span></span>](tokenlifetimepolicy.md) | <span data-ttu-id="fd4f5-121">读取 tokenLifetimePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-121">Read properties and relationships of a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="fd4f5-122">更新 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="fd4f5-122">Update tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-update.md) | <span data-ttu-id="fd4f5-123">无</span><span class="sxs-lookup"><span data-stu-id="fd4f5-123">None</span></span> | <span data-ttu-id="fd4f5-124">更新 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-124">Update a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="fd4f5-125">删除 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="fd4f5-125">Delete tokenLifetimePolicy</span></span>](../api/tokenlifetimepolicy-delete.md) | <span data-ttu-id="fd4f5-126">无</span><span class="sxs-lookup"><span data-stu-id="fd4f5-126">None</span></span> | <span data-ttu-id="fd4f5-127">删除 tokenLifetimePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-127">Delete a tokenLifetimePolicy object.</span></span> |
| [<span data-ttu-id="fd4f5-128">List appliesTo</span><span class="sxs-lookup"><span data-stu-id="fd4f5-128">List appliesTo</span></span>](../api/tokenlifetimepolicy-list-appliesto.md) | <span data-ttu-id="fd4f5-129">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="fd4f5-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="fd4f5-130">获取已应用此策略的 directoryObjects 列表。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-130">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="fd4f5-131">属性</span><span class="sxs-lookup"><span data-stu-id="fd4f5-131">Properties</span></span>

| <span data-ttu-id="fd4f5-132">属性</span><span class="sxs-lookup"><span data-stu-id="fd4f5-132">Property</span></span>     | <span data-ttu-id="fd4f5-133">类型</span><span class="sxs-lookup"><span data-stu-id="fd4f5-133">Type</span></span>        | <span data-ttu-id="fd4f5-134">说明</span><span class="sxs-lookup"><span data-stu-id="fd4f5-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fd4f5-135">id</span><span class="sxs-lookup"><span data-stu-id="fd4f5-135">id</span></span>|<span data-ttu-id="fd4f5-136">String</span><span class="sxs-lookup"><span data-stu-id="fd4f5-136">String</span></span>| <span data-ttu-id="fd4f5-137">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-137">Unique identifier for this policy.</span></span> <span data-ttu-id="fd4f5-138">只读。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-138">Read-only.</span></span>|
|<span data-ttu-id="fd4f5-139">definition</span><span class="sxs-lookup"><span data-stu-id="fd4f5-139">definition</span></span>|<span data-ttu-id="fd4f5-140">String collection</span><span class="sxs-lookup"><span data-stu-id="fd4f5-140">String collection</span></span>| <span data-ttu-id="fd4f5-141">包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-141">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="fd4f5-142">有关此属性的 JSON 架构的更多详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-142">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="fd4f5-143">必需。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-143">Required.</span></span>|
|<span data-ttu-id="fd4f5-144">description</span><span class="sxs-lookup"><span data-stu-id="fd4f5-144">description</span></span>|<span data-ttu-id="fd4f5-145">String</span><span class="sxs-lookup"><span data-stu-id="fd4f5-145">String</span></span>| <span data-ttu-id="fd4f5-146">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-146">Description for this policy.</span></span>|
|<span data-ttu-id="fd4f5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="fd4f5-147">displayName</span></span>|<span data-ttu-id="fd4f5-148">String</span><span class="sxs-lookup"><span data-stu-id="fd4f5-148">String</span></span>| <span data-ttu-id="fd4f5-149">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-149">Display name for this policy.</span></span> <span data-ttu-id="fd4f5-150">必需。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-150">Required.</span></span>|
|<span data-ttu-id="fd4f5-151">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="fd4f5-151">isOrganizationDefault</span></span>|<span data-ttu-id="fd4f5-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd4f5-152">Boolean</span></span>|<span data-ttu-id="fd4f5-153">如果设置为 `true` ，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-153">If set to `true`, activates this policy.</span></span> <span data-ttu-id="fd4f5-154">同一策略类型可以有很多策略，但只有一个策略可以激活为组织默认策略。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-154">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="fd4f5-155">可选，默认值为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-155">Optional, default value is `false`.</span></span>|


### <a name="properties-of-a-token-lifetime-policy-definition"></a><span data-ttu-id="fd4f5-156">令牌生存期策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="fd4f5-156">Properties of a token lifetime policy definition</span></span>
<span data-ttu-id="fd4f5-157">下面的属性构成表示令牌生存期策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-157">The properties below form the JSON object that represents a token lifetime policy.</span></span> <span data-ttu-id="fd4f5-158">此 JSON 对象必须 **转换为** 转义为要插入到定义属性中的引号 **的** 字符串。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-158">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="fd4f5-159">下面以 JSON 格式显示了一个示例：</span><span class="sxs-lookup"><span data-stu-id="fd4f5-159">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

><span data-ttu-id="fd4f5-160">**注意：** 这些属性的所有持续时间均以"dd.hh：mm：ss"格式指定。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-160">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="fd4f5-161">**注意：** 用"天"表示的属性的最大值比指定天数短 1 秒。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-161">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="fd4f5-162">例如，最大值 1 天指定为"23：59：59"。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-162">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="fd4f5-163">属性</span><span class="sxs-lookup"><span data-stu-id="fd4f5-163">Property</span></span>     | <span data-ttu-id="fd4f5-164">类型</span><span class="sxs-lookup"><span data-stu-id="fd4f5-164">Type</span></span>   |<span data-ttu-id="fd4f5-165">说明</span><span class="sxs-lookup"><span data-stu-id="fd4f5-165">Description</span></span>| <span data-ttu-id="fd4f5-166">最小值</span><span class="sxs-lookup"><span data-stu-id="fd4f5-166">Min Value</span></span> | <span data-ttu-id="fd4f5-167">最大值</span><span class="sxs-lookup"><span data-stu-id="fd4f5-167">Max Value</span></span> | <span data-ttu-id="fd4f5-168">默认值</span><span class="sxs-lookup"><span data-stu-id="fd4f5-168">Default Value</span></span>|
|:---------------|:--------|:----------|:--------|:--------|:----|
|<span data-ttu-id="fd4f5-169">AccessTokenLifetime</span><span class="sxs-lookup"><span data-stu-id="fd4f5-169">AccessTokenLifetime</span></span>|<span data-ttu-id="fd4f5-170">String</span><span class="sxs-lookup"><span data-stu-id="fd4f5-170">String</span></span>|<span data-ttu-id="fd4f5-171">控制访问令牌和 ID 令牌都被视为有效的时间。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-171">Controls how long both access and ID tokens are considered valid.</span></span>|<span data-ttu-id="fd4f5-172">10 分钟</span><span class="sxs-lookup"><span data-stu-id="fd4f5-172">10 minutes</span></span>|<span data-ttu-id="fd4f5-173">1 天</span><span class="sxs-lookup"><span data-stu-id="fd4f5-173">1 day</span></span>|<span data-ttu-id="fd4f5-174">1 小时</span><span class="sxs-lookup"><span data-stu-id="fd4f5-174">1 hour</span></span>|
|<span data-ttu-id="fd4f5-175">版本</span><span class="sxs-lookup"><span data-stu-id="fd4f5-175">Version</span></span>|<span data-ttu-id="fd4f5-176">整数</span><span class="sxs-lookup"><span data-stu-id="fd4f5-176">Integer</span></span>|<span data-ttu-id="fd4f5-177">将值设置为 1。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-177">Set value of 1.</span></span> <span data-ttu-id="fd4f5-178">必需。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-178">Required.</span></span>|<span data-ttu-id="fd4f5-179">无</span><span class="sxs-lookup"><span data-stu-id="fd4f5-179">None</span></span>|<span data-ttu-id="fd4f5-180">无</span><span class="sxs-lookup"><span data-stu-id="fd4f5-180">None</span></span>|<span data-ttu-id="fd4f5-181">无</span><span class="sxs-lookup"><span data-stu-id="fd4f5-181">None</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd4f5-182">关系</span><span class="sxs-lookup"><span data-stu-id="fd4f5-182">Relationships</span></span>

| <span data-ttu-id="fd4f5-183">关系</span><span class="sxs-lookup"><span data-stu-id="fd4f5-183">Relationship</span></span> | <span data-ttu-id="fd4f5-184">类型</span><span class="sxs-lookup"><span data-stu-id="fd4f5-184">Type</span></span>        | <span data-ttu-id="fd4f5-185">说明</span><span class="sxs-lookup"><span data-stu-id="fd4f5-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fd4f5-186">appliesTo</span><span class="sxs-lookup"><span data-stu-id="fd4f5-186">appliesTo</span></span>|<span data-ttu-id="fd4f5-187">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="fd4f5-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="fd4f5-188">已应用此策略的 [directoryObject](directoryObject.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-188">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="fd4f5-189">只读。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-189">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd4f5-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd4f5-190">JSON representation</span></span>

<span data-ttu-id="fd4f5-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd4f5-191">The following is a JSON representation of the resource.</span></span>

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
