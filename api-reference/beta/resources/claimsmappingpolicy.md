---
title: claimsMappingPolicy 资源类型
description: 表示可控制 Azure Active Directory （Azure AD）颁发的访问令牌的生存期的策略。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a7f173cc8949dd0cf493620e08b5fdc5c61b8afb
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007008"
---
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="af418-103">claimsMappingPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="af418-103">claimsMappingPolicy resource type</span></span>

<span data-ttu-id="af418-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af418-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af418-105">表示对颁发给特定应用程序的令牌的 WS 馈送、SAML、OAuth 2.0 和 OpenID Connect 协议的声明映射策略。</span><span class="sxs-lookup"><span data-stu-id="af418-105">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="af418-106">您可以使用声明映射策略执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="af418-106">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="af418-107">选择令牌中包含的声明</span><span class="sxs-lookup"><span data-stu-id="af418-107">Select which claims are included in tokens</span></span>
- <span data-ttu-id="af418-108">创建尚不存在的声明类型</span><span class="sxs-lookup"><span data-stu-id="af418-108">Create claim types that do not already exist</span></span>
- <span data-ttu-id="af418-109">选择或更改特定声明中发出的数据源</span><span class="sxs-lookup"><span data-stu-id="af418-109">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="af418-110">有关更多方案和配置详细信息，请参阅[如何：自定义在租户中的特定应用程序令牌中发出的声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties)。</span><span class="sxs-lookup"><span data-stu-id="af418-110">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="af418-111">继承自[stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="af418-111">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="af418-112">方法</span><span class="sxs-lookup"><span data-stu-id="af418-112">Methods</span></span>

| <span data-ttu-id="af418-113">方法</span><span class="sxs-lookup"><span data-stu-id="af418-113">Method</span></span>       | <span data-ttu-id="af418-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="af418-114">Return Type</span></span> | <span data-ttu-id="af418-115">说明</span><span class="sxs-lookup"><span data-stu-id="af418-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="af418-116">创建 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="af418-116">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="af418-117">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="af418-117">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="af418-118">创建 claimsMappingPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="af418-118">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="af418-119">获取 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="af418-119">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="af418-120">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="af418-120">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="af418-121">读取 claimsMappingPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af418-121">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="af418-122">列出 claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="af418-122">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="af418-123">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="af418-123">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="af418-124">读取 claimsMappingPolicies 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af418-124">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="af418-125">更新 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="af418-125">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="af418-126">无</span><span class="sxs-lookup"><span data-stu-id="af418-126">None</span></span> | <span data-ttu-id="af418-127">更新 claimsMappingPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="af418-127">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="af418-128">删除 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="af418-128">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="af418-129">无</span><span class="sxs-lookup"><span data-stu-id="af418-129">None</span></span> | <span data-ttu-id="af418-130">删除 claimsMappingPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="af418-130">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="af418-131">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="af418-131">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="af418-132">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af418-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="af418-133">获取已应用此策略的 directoryObjects 的列表。</span><span class="sxs-lookup"><span data-stu-id="af418-133">Get the list of directoryObjects that this policy has been applied to.</span></span> |
| [<span data-ttu-id="af418-134">分配 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="af418-134">Assign claimsMappingPolicy</span></span>](../api/serviceprincipal-post-claimsmappingpolicies.md) | <span data-ttu-id="af418-135">无</span><span class="sxs-lookup"><span data-stu-id="af418-135">None</span></span> | <span data-ttu-id="af418-136">将 claimsMappingPolicy 分配给[servicePrincipal](serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="af418-136">Assign a claimsMappingPolicy to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="af418-137">列表已分配 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="af418-137">List assigned claimsMappingPolicy</span></span>](../api/serviceprincipal-list-claimsmappingpolicies.md) | <span data-ttu-id="af418-138">[claimsMappingPolicy](claimsmappingpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af418-138">[claimsMappingPolicy](claimsmappingpolicy.md) collection</span></span> | <span data-ttu-id="af418-139">列出分配给[servicePrincipal](serviceprincipal.md)对象的 claimsMappingPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="af418-139">List the claimsMappingPolicy objects that are assigned to a [servicePrincipal](serviceprincipal.md) object.</span></span> |
| [<span data-ttu-id="af418-140">删除 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="af418-140">Remove claimsMappingPolicy</span></span>](../api/serviceprincipal-delete-claimsmappingpolicies.md) | <span data-ttu-id="af418-141">无</span><span class="sxs-lookup"><span data-stu-id="af418-141">None</span></span> | <span data-ttu-id="af418-142">从[servicePrincipal](serviceprincipal.md)对象中删除 claimsMappingPolicy。</span><span class="sxs-lookup"><span data-stu-id="af418-142">Remove a claimsMappingPolicy from a [servicePrincipal](serviceprincipal.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="af418-143">属性</span><span class="sxs-lookup"><span data-stu-id="af418-143">Properties</span></span>

| <span data-ttu-id="af418-144">属性</span><span class="sxs-lookup"><span data-stu-id="af418-144">Property</span></span>     | <span data-ttu-id="af418-145">类型</span><span class="sxs-lookup"><span data-stu-id="af418-145">Type</span></span>        | <span data-ttu-id="af418-146">说明</span><span class="sxs-lookup"><span data-stu-id="af418-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="af418-147">id</span><span class="sxs-lookup"><span data-stu-id="af418-147">id</span></span>|<span data-ttu-id="af418-148">字符串</span><span class="sxs-lookup"><span data-stu-id="af418-148">String</span></span>| <span data-ttu-id="af418-149">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="af418-149">Unique identifier for this policy.</span></span> <span data-ttu-id="af418-150">只读。</span><span class="sxs-lookup"><span data-stu-id="af418-150">Read-only.</span></span>|
|<span data-ttu-id="af418-151">定义</span><span class="sxs-lookup"><span data-stu-id="af418-151">definition</span></span>|<span data-ttu-id="af418-152">String collection</span><span class="sxs-lookup"><span data-stu-id="af418-152">String collection</span></span>| <span data-ttu-id="af418-153">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="af418-153">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="af418-154">有关此属性的 JSON 架构的更多详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="af418-154">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="af418-155">必需。</span><span class="sxs-lookup"><span data-stu-id="af418-155">Required.</span></span>|
|<span data-ttu-id="af418-156">description</span><span class="sxs-lookup"><span data-stu-id="af418-156">description</span></span>|<span data-ttu-id="af418-157">String</span><span class="sxs-lookup"><span data-stu-id="af418-157">String</span></span>| <span data-ttu-id="af418-158">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="af418-158">Description for this policy.</span></span>|
|<span data-ttu-id="af418-159">displayName</span><span class="sxs-lookup"><span data-stu-id="af418-159">displayName</span></span>|<span data-ttu-id="af418-160">String</span><span class="sxs-lookup"><span data-stu-id="af418-160">String</span></span>| <span data-ttu-id="af418-161">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="af418-161">Display name for this policy.</span></span> <span data-ttu-id="af418-162">必需。</span><span class="sxs-lookup"><span data-stu-id="af418-162">Required.</span></span>|
|<span data-ttu-id="af418-163">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="af418-163">isOrganizationDefault</span></span>|<span data-ttu-id="af418-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="af418-164">Boolean</span></span>|<span data-ttu-id="af418-165">忽略此属性。</span><span class="sxs-lookup"><span data-stu-id="af418-165">Ignore this property.</span></span> <span data-ttu-id="af418-166">声明映射策略仅可应用于服务主体，不能为组织全局设置。</span><span class="sxs-lookup"><span data-stu-id="af418-166">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="af418-167">声明映射策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="af418-167">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="af418-168">下面的属性构成了表示声明映射策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="af418-168">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="af418-169">此 JSON 对象必须**转换为转义了引号的字符串**，以将其插入到**定义**属性中。</span><span class="sxs-lookup"><span data-stu-id="af418-169">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="af418-170">下面显示了几个定义示例：</span><span class="sxs-lookup"><span data-stu-id="af418-170">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="af418-171">示例：将 "雇员 Id" 和 "TenantCountry" 作为声明包含在标记中的**定义**</span><span class="sxs-lookup"><span data-stu-id="af418-171">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
<!-- {
  "blockType": "ignored"
}-->
``` json
{
  "definition": [
    "{\"ClaimsMappingPolicy\":{
      \"Version\":1,
      \"IncludeBasicClaimSet\":\"true\", 
      \"ClaimsSchema\": [
        {\"Source\":\"user\",\"ID\":\"employeeid\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\",\"JwtClaimType\":\"name\"},{\"Source\":\"company\",\"ID\":\"tenantcountry\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/country\",\"JwtClaimType\":\"country\"}
        ]
      }
    }"
  ]
}
```

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="af418-172">示例：使用声明转换的**定义**</span><span class="sxs-lookup"><span data-stu-id="af418-172">Example: **definition** that uses a claims transformation</span></span>
<!-- {
  "blockType": "ignored"
}-->
``` json
{
  "definition": [
    "{\"ClaimsMappingPolicy\":{
      \"Version\":1,
      \"IncludeBasicClaimSet\":\"true\", 
      \"ClaimsSchema\":[
        {\"Source\":\"user\",\"ID\":\"extensionattribute1\"},{\"Source\":\"transformation\",\"ID\":\"DataJoin\",\"TransformationId\":\"JoinTheData\",\"JwtClaimType\":\"JoinedData\"}
        ],
      \"ClaimsTransformation\":[
        {\"ID\":\"JoinTheData\",\"TransformationMethod\":\"Join\",\"InputClaims\":[{\"ClaimTypeReferenceId\":\"extensionattribute1\",\"TransformationClaimType\":\"string1\"}], \"InputParameters\": [{\"ID\":\"string2\",\"Value\":\"sandbox\"},{\"ID\":\"separator\",\"Value\":\".\"}],\"OutputClaims\":[{\"ClaimTypeReferenceId\":\"DataJoin\",\"TransformationClaimType\":\"outputClaim\"}]}
        ]
      }
    }"
  ]
}
```

| <span data-ttu-id="af418-173">属性</span><span class="sxs-lookup"><span data-stu-id="af418-173">Property</span></span>     | <span data-ttu-id="af418-174">类型</span><span class="sxs-lookup"><span data-stu-id="af418-174">Type</span></span>   |<span data-ttu-id="af418-175">说明</span><span class="sxs-lookup"><span data-stu-id="af418-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af418-176">版本</span><span class="sxs-lookup"><span data-stu-id="af418-176">Version</span></span>|<span data-ttu-id="af418-177">Integer</span><span class="sxs-lookup"><span data-stu-id="af418-177">Integer</span></span>|<span data-ttu-id="af418-178">将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="af418-178">Set value of 1.</span></span> <span data-ttu-id="af418-179">必需。</span><span class="sxs-lookup"><span data-stu-id="af418-179">Required.</span></span>|
|<span data-ttu-id="af418-180">IncludeBasicClaimSet</span><span class="sxs-lookup"><span data-stu-id="af418-180">IncludeBasicClaimSet</span></span>|<span data-ttu-id="af418-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="af418-181">Boolean</span></span>|<span data-ttu-id="af418-182">如果设置为 true，则在受策略影响的令牌中发出基本声明集中的所有声明。</span><span class="sxs-lookup"><span data-stu-id="af418-182">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="af418-183">如果设置为 false，则基本声明集中的声明不在令牌中，除非它们单独添加到同一策略的 ClaimsSchema 属性中。</span><span class="sxs-lookup"><span data-stu-id="af418-183">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="af418-184">ClaimsSchema</span><span class="sxs-lookup"><span data-stu-id="af418-184">ClaimsSchema</span></span>|<span data-ttu-id="af418-185">JSON 对象</span><span class="sxs-lookup"><span data-stu-id="af418-185">JSON object</span></span>|<span data-ttu-id="af418-186">定义受策略影响的令牌中存在的声明，以及基本声明集和核心声明集。</span><span class="sxs-lookup"><span data-stu-id="af418-186">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="af418-187">对于在此属性中定义的每个声明架构条目，需要特定信息。</span><span class="sxs-lookup"><span data-stu-id="af418-187">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="af418-188">指定数据的来源（"值" 或 "源/ID 对"），以及将数据作为（声明类型）发出的声明。</span><span class="sxs-lookup"><span data-stu-id="af418-188">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="af418-189">[ClaimsSchema 定义](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema)中提供了更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="af418-189">Further details are available in the [ClaimsSchema definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="af418-190">ClaimsTransformation</span><span class="sxs-lookup"><span data-stu-id="af418-190">ClaimsTransformation</span></span>|<span data-ttu-id="af418-191">JSON 对象</span><span class="sxs-lookup"><span data-stu-id="af418-191">JSON object</span></span>| <span data-ttu-id="af418-192">定义可应用于源数据的常见转换，以生成 ClaimsSchema 中指定的声明的输出数据。</span><span class="sxs-lookup"><span data-stu-id="af418-192">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="af418-193">[ClaimsTransformation 定义](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation)中提供了更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="af418-193">Further details are available in the [ClaimsTransformation definition](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="af418-194">关系</span><span class="sxs-lookup"><span data-stu-id="af418-194">Relationships</span></span>

| <span data-ttu-id="af418-195">关系</span><span class="sxs-lookup"><span data-stu-id="af418-195">Relationship</span></span> | <span data-ttu-id="af418-196">类型</span><span class="sxs-lookup"><span data-stu-id="af418-196">Type</span></span>        | <span data-ttu-id="af418-197">说明</span><span class="sxs-lookup"><span data-stu-id="af418-197">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="af418-198">appliesTo</span><span class="sxs-lookup"><span data-stu-id="af418-198">appliesTo</span></span>|<span data-ttu-id="af418-199">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af418-199">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="af418-200">已将此策略应用于的[directoryObject](directoryObject.md)集合。</span><span class="sxs-lookup"><span data-stu-id="af418-200">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="af418-201">只读。</span><span class="sxs-lookup"><span data-stu-id="af418-201">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af418-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af418-202">JSON representation</span></span>

<span data-ttu-id="af418-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af418-203">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
  "baseType": "microsoft.graph.stsPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": false,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "claimsMappingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->