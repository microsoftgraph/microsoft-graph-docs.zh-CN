---
title: claimsMappingPolicy 资源类型
description: 表示对颁发给特定应用程序的令牌的 WS 馈送、SAML、OAuth 2.0 和 OpenID Connect 协议的声明映射策略。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e170008bf42cbf5d1d218d2b82570fc0dfff8444
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581272"
---
# <a name="claimsmappingpolicy-resource-type"></a><span data-ttu-id="62d2b-103">claimsMappingPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="62d2b-103">claimsMappingPolicy resource type</span></span>

<span data-ttu-id="62d2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62d2b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62d2b-105">表示对颁发给特定应用程序的令牌的 WS 馈送、SAML、OAuth 2.0 和 OpenID Connect 协议的声明映射策略。</span><span class="sxs-lookup"><span data-stu-id="62d2b-105">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> <span data-ttu-id="62d2b-106">您可以使用声明映射策略执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="62d2b-106">You can use claims-mapping policies to:</span></span>

- <span data-ttu-id="62d2b-107">选择令牌中包含的声明</span><span class="sxs-lookup"><span data-stu-id="62d2b-107">Select which claims are included in tokens</span></span>
- <span data-ttu-id="62d2b-108">创建尚不存在的声明类型</span><span class="sxs-lookup"><span data-stu-id="62d2b-108">Create claim types that do not already exist</span></span>
- <span data-ttu-id="62d2b-109">选择或更改特定声明中发出的数据源</span><span class="sxs-lookup"><span data-stu-id="62d2b-109">Choose or change the source of data emitted in specific claims</span></span>  

<span data-ttu-id="62d2b-110">有关更多方案和配置详细信息，请参阅 [如何：自定义在租户中的特定应用程序令牌中发出的声明](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties)。</span><span class="sxs-lookup"><span data-stu-id="62d2b-110">For more scenario and configuration details see [How to: Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties).</span></span>

<span data-ttu-id="62d2b-111">继承自 [stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="62d2b-111">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="62d2b-112">方法</span><span class="sxs-lookup"><span data-stu-id="62d2b-112">Methods</span></span>

| <span data-ttu-id="62d2b-113">方法</span><span class="sxs-lookup"><span data-stu-id="62d2b-113">Method</span></span>       | <span data-ttu-id="62d2b-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="62d2b-114">Return Type</span></span> | <span data-ttu-id="62d2b-115">说明</span><span class="sxs-lookup"><span data-stu-id="62d2b-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="62d2b-116">创建 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="62d2b-116">Create claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [<span data-ttu-id="62d2b-117">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="62d2b-117">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="62d2b-118">创建 claimsMappingPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="62d2b-118">Create a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="62d2b-119">获取 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="62d2b-119">Get claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-get.md) | [<span data-ttu-id="62d2b-120">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="62d2b-120">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="62d2b-121">读取 claimsMappingPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62d2b-121">Read properties and relationships of a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="62d2b-122">列出 claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="62d2b-122">List claimsMappingPolicies</span></span>](../api/claimsmappingpolicy-list.md) | [<span data-ttu-id="62d2b-123">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="62d2b-123">claimsMappingPolicy</span></span>](claimsmappingpolicy.md) | <span data-ttu-id="62d2b-124">读取 claimsMappingPolicies 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62d2b-124">Read properties and relationships of claimsMappingPolicies objects.</span></span> |
| [<span data-ttu-id="62d2b-125">更新 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="62d2b-125">Update claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-update.md) | <span data-ttu-id="62d2b-126">无</span><span class="sxs-lookup"><span data-stu-id="62d2b-126">None</span></span> | <span data-ttu-id="62d2b-127">更新 claimsMappingPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="62d2b-127">Update a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="62d2b-128">删除 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="62d2b-128">Delete claimsMappingPolicy</span></span>](../api/claimsmappingpolicy-delete.md) | <span data-ttu-id="62d2b-129">无</span><span class="sxs-lookup"><span data-stu-id="62d2b-129">None</span></span> | <span data-ttu-id="62d2b-130">删除 claimsMappingPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="62d2b-130">Delete a claimsMappingPolicy object.</span></span> |
| [<span data-ttu-id="62d2b-131">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="62d2b-131">List appliesTo</span></span>](../api/claimsmappingpolicy-list-appliesto.md) | <span data-ttu-id="62d2b-132">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="62d2b-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="62d2b-133">获取已应用此策略的 directoryObjects 的列表。</span><span class="sxs-lookup"><span data-stu-id="62d2b-133">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="62d2b-134">属性</span><span class="sxs-lookup"><span data-stu-id="62d2b-134">Properties</span></span>

| <span data-ttu-id="62d2b-135">属性</span><span class="sxs-lookup"><span data-stu-id="62d2b-135">Property</span></span>     | <span data-ttu-id="62d2b-136">类型</span><span class="sxs-lookup"><span data-stu-id="62d2b-136">Type</span></span>        | <span data-ttu-id="62d2b-137">说明</span><span class="sxs-lookup"><span data-stu-id="62d2b-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62d2b-138">id</span><span class="sxs-lookup"><span data-stu-id="62d2b-138">id</span></span>|<span data-ttu-id="62d2b-139">字符串</span><span class="sxs-lookup"><span data-stu-id="62d2b-139">String</span></span>| <span data-ttu-id="62d2b-140">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="62d2b-140">Unique identifier for this policy.</span></span> <span data-ttu-id="62d2b-141">只读。</span><span class="sxs-lookup"><span data-stu-id="62d2b-141">Read-only.</span></span>|
|<span data-ttu-id="62d2b-142">定义</span><span class="sxs-lookup"><span data-stu-id="62d2b-142">definition</span></span>|<span data-ttu-id="62d2b-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="62d2b-143">String collection</span></span>| <span data-ttu-id="62d2b-144">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="62d2b-144">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="62d2b-145">有关此属性的 JSON 架构的更多详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="62d2b-145">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="62d2b-146">必需。</span><span class="sxs-lookup"><span data-stu-id="62d2b-146">Required.</span></span>|
|<span data-ttu-id="62d2b-147">description</span><span class="sxs-lookup"><span data-stu-id="62d2b-147">description</span></span>|<span data-ttu-id="62d2b-148">字符串</span><span class="sxs-lookup"><span data-stu-id="62d2b-148">String</span></span>| <span data-ttu-id="62d2b-149">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="62d2b-149">Description for this policy.</span></span>|
|<span data-ttu-id="62d2b-150">displayName</span><span class="sxs-lookup"><span data-stu-id="62d2b-150">displayName</span></span>|<span data-ttu-id="62d2b-151">字符串</span><span class="sxs-lookup"><span data-stu-id="62d2b-151">String</span></span>| <span data-ttu-id="62d2b-152">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="62d2b-152">Display name for this policy.</span></span> <span data-ttu-id="62d2b-153">必填。</span><span class="sxs-lookup"><span data-stu-id="62d2b-153">Required.</span></span>|
|<span data-ttu-id="62d2b-154">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="62d2b-154">isOrganizationDefault</span></span>|<span data-ttu-id="62d2b-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="62d2b-155">Boolean</span></span>|<span data-ttu-id="62d2b-156">忽略此属性。</span><span class="sxs-lookup"><span data-stu-id="62d2b-156">Ignore this property.</span></span> <span data-ttu-id="62d2b-157">声明映射策略仅可应用于服务主体，不能为组织全局设置。</span><span class="sxs-lookup"><span data-stu-id="62d2b-157">The claims-mapping policy can only be applied to service principals and can't be set globally for the organization.</span></span>|

### <a name="properties-of-a-claims-mapping-policy-definition"></a><span data-ttu-id="62d2b-158">声明映射策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="62d2b-158">Properties of a claims-mapping policy definition</span></span>

<span data-ttu-id="62d2b-159">下面的属性构成了表示声明映射策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="62d2b-159">The properties below form the JSON object that represents a claims-mapping policy.</span></span> <span data-ttu-id="62d2b-160">此 JSON 对象必须 **转换为转义了引号的字符串** ，以将其插入到 **定义** 属性中。</span><span class="sxs-lookup"><span data-stu-id="62d2b-160">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="62d2b-161">下面显示了几个定义示例：</span><span class="sxs-lookup"><span data-stu-id="62d2b-161">A few definition examples are shown below:</span></span>

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a><span data-ttu-id="62d2b-162">示例：将 "雇员 Id" 和 "TenantCountry" 作为声明包含在标记中的**定义**</span><span class="sxs-lookup"><span data-stu-id="62d2b-162">Example: **definition** to include the EmployeeID and TenantCountry as claims in tokens</span></span>
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

#### <a name="example-definition-that-uses-a-claims-transformation"></a><span data-ttu-id="62d2b-163">示例：使用声明转换的**定义**</span><span class="sxs-lookup"><span data-stu-id="62d2b-163">Example: **definition** that uses a claims transformation</span></span>
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

| <span data-ttu-id="62d2b-164">属性</span><span class="sxs-lookup"><span data-stu-id="62d2b-164">Property</span></span>     | <span data-ttu-id="62d2b-165">类型</span><span class="sxs-lookup"><span data-stu-id="62d2b-165">Type</span></span>   |<span data-ttu-id="62d2b-166">说明</span><span class="sxs-lookup"><span data-stu-id="62d2b-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62d2b-167">版本</span><span class="sxs-lookup"><span data-stu-id="62d2b-167">Version</span></span>|<span data-ttu-id="62d2b-168">整数</span><span class="sxs-lookup"><span data-stu-id="62d2b-168">Integer</span></span>|<span data-ttu-id="62d2b-169">将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="62d2b-169">Set value of 1.</span></span> <span data-ttu-id="62d2b-170">必填。</span><span class="sxs-lookup"><span data-stu-id="62d2b-170">Required.</span></span>|
|<span data-ttu-id="62d2b-171">IncludeBasicClaimSet</span><span class="sxs-lookup"><span data-stu-id="62d2b-171">IncludeBasicClaimSet</span></span>|<span data-ttu-id="62d2b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="62d2b-172">Boolean</span></span>|<span data-ttu-id="62d2b-173">如果设置为 true，则在受策略影响的令牌中发出基本声明集中的所有声明。</span><span class="sxs-lookup"><span data-stu-id="62d2b-173">If set to true, all claims in the basic claim set are emitted in tokens affected by the policy.</span></span> <span data-ttu-id="62d2b-174">如果设置为 false，则基本声明集中的声明不在令牌中，除非它们单独添加到同一策略的 ClaimsSchema 属性中。</span><span class="sxs-lookup"><span data-stu-id="62d2b-174">If set to false, claims in the basic claim set are not in the tokens, unless they are individually added in the ClaimsSchema property of the same policy.</span></span>|
|<span data-ttu-id="62d2b-175">ClaimsSchema</span><span class="sxs-lookup"><span data-stu-id="62d2b-175">ClaimsSchema</span></span>|<span data-ttu-id="62d2b-176">JSON 对象</span><span class="sxs-lookup"><span data-stu-id="62d2b-176">JSON object</span></span>|<span data-ttu-id="62d2b-177">定义受策略影响的令牌中存在的声明，以及基本声明集和核心声明集。</span><span class="sxs-lookup"><span data-stu-id="62d2b-177">Defines which claims are present in the tokens affected by the policy, in addition to the basic claim set and the core claim set.</span></span> <span data-ttu-id="62d2b-178">对于在此属性中定义的每个声明架构条目，需要特定信息。</span><span class="sxs-lookup"><span data-stu-id="62d2b-178">For each claim schema entry defined in this property, certain information is required.</span></span> <span data-ttu-id="62d2b-179">指定数据来自 (值或源/ID 对) ，并声明数据作为 (声明类型) 发出。</span><span class="sxs-lookup"><span data-stu-id="62d2b-179">Specify where the data is coming from (Value or Source/ID pair), and which claim the data is emitted as (Claim Type).</span></span> <span data-ttu-id="62d2b-180">有关详细信息，请参阅 [ClaimsSchema definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema)。</span><span class="sxs-lookup"><span data-stu-id="62d2b-180">For more information, see [ClaimsSchema definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema).</span></span>|
|<span data-ttu-id="62d2b-181">ClaimsTransformation</span><span class="sxs-lookup"><span data-stu-id="62d2b-181">ClaimsTransformation</span></span>|<span data-ttu-id="62d2b-182">JSON 对象</span><span class="sxs-lookup"><span data-stu-id="62d2b-182">JSON object</span></span>| <span data-ttu-id="62d2b-183">定义可应用于源数据的常见转换，以生成 ClaimsSchema 中指定的声明的输出数据。</span><span class="sxs-lookup"><span data-stu-id="62d2b-183">Defines common transformations that can be applied to source data, to generate the output data for claims specified in the ClaimsSchema.</span></span> <span data-ttu-id="62d2b-184">有关详细信息，请参阅 [ClaimsTransformation definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation)。</span><span class="sxs-lookup"><span data-stu-id="62d2b-184">For more information, see [ClaimsTransformation definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation).</span></span>|


## <a name="relationships"></a><span data-ttu-id="62d2b-185">关系</span><span class="sxs-lookup"><span data-stu-id="62d2b-185">Relationships</span></span>

| <span data-ttu-id="62d2b-186">关系</span><span class="sxs-lookup"><span data-stu-id="62d2b-186">Relationship</span></span> | <span data-ttu-id="62d2b-187">类型</span><span class="sxs-lookup"><span data-stu-id="62d2b-187">Type</span></span>        | <span data-ttu-id="62d2b-188">说明</span><span class="sxs-lookup"><span data-stu-id="62d2b-188">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62d2b-189">appliesTo</span><span class="sxs-lookup"><span data-stu-id="62d2b-189">appliesTo</span></span>|<span data-ttu-id="62d2b-190">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="62d2b-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="62d2b-191">已将此策略应用于的 [directoryObject](directoryObject.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="62d2b-191">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="62d2b-192">只读。</span><span class="sxs-lookup"><span data-stu-id="62d2b-192">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62d2b-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62d2b-193">JSON representation</span></span>

<span data-ttu-id="62d2b-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62d2b-194">The following is a JSON representation of the resource.</span></span>

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