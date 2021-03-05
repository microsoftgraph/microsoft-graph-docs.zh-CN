---
title: tokenIssuancePolicy 资源类型
description: 表示用于指定 Azure AD 颁发的 SAML 令牌特征的策略。
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 761e1d7e45f2d6a2cb11513cd3484a88a080888e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444320"
---
# <a name="tokenissuancepolicy-resource-type"></a><span data-ttu-id="dfee8-103">tokenIssuancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfee8-103">tokenIssuancePolicy resource type</span></span>

<span data-ttu-id="dfee8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfee8-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="dfee8-105">表示用于指定 Azure AD 颁发的 SAML 令牌特征的策略。</span><span class="sxs-lookup"><span data-stu-id="dfee8-105">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span> <span data-ttu-id="dfee8-106">可以使用令牌颁发策略：</span><span class="sxs-lookup"><span data-stu-id="dfee8-106">You can use token-issuance policies to:</span></span>

- <span data-ttu-id="dfee8-107">设置签名选项</span><span class="sxs-lookup"><span data-stu-id="dfee8-107">Set signing options</span></span>
- <span data-ttu-id="dfee8-108">设置签名算法</span><span class="sxs-lookup"><span data-stu-id="dfee8-108">Set signing algorithm</span></span>
- <span data-ttu-id="dfee8-109">设置 SAML 令牌版本</span><span class="sxs-lookup"><span data-stu-id="dfee8-109">Set SAML token version</span></span>

<span data-ttu-id="dfee8-110">继承自 [stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="dfee8-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dfee8-111">Methods</span><span class="sxs-lookup"><span data-stu-id="dfee8-111">Methods</span></span>

| <span data-ttu-id="dfee8-112">方法</span><span class="sxs-lookup"><span data-stu-id="dfee8-112">Method</span></span>       | <span data-ttu-id="dfee8-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="dfee8-113">Return Type</span></span> | <span data-ttu-id="dfee8-114">说明</span><span class="sxs-lookup"><span data-stu-id="dfee8-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dfee8-115">列出 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="dfee8-115">List tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-list.md) | [<span data-ttu-id="dfee8-116">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="dfee8-116">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="dfee8-117">读取 tokenIssuancePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dfee8-117">Read properties and relationships of tokenIssuancePolicy objects.</span></span> |
| [<span data-ttu-id="dfee8-118">创建 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="dfee8-118">Create tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [<span data-ttu-id="dfee8-119">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="dfee8-119">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="dfee8-120">创建 tokenIssuancePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="dfee8-120">Create a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="dfee8-121">获取 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="dfee8-121">Get tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-get.md) | [<span data-ttu-id="dfee8-122">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="dfee8-122">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="dfee8-123">读取 tokenIssuancePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dfee8-123">Read properties and relationships of a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="dfee8-124">更新 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="dfee8-124">Update tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-update.md) | <span data-ttu-id="dfee8-125">无</span><span class="sxs-lookup"><span data-stu-id="dfee8-125">None</span></span> | <span data-ttu-id="dfee8-126">更新 tokenIssuancePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="dfee8-126">Update a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="dfee8-127">删除 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="dfee8-127">Delete tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-delete.md) | <span data-ttu-id="dfee8-128">无</span><span class="sxs-lookup"><span data-stu-id="dfee8-128">None</span></span> | <span data-ttu-id="dfee8-129">删除 tokenIssuancePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="dfee8-129">Delete a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="dfee8-130">List appliesTo</span><span class="sxs-lookup"><span data-stu-id="dfee8-130">List appliesTo</span></span>](../api/tokenissuancepolicy-list-appliesto.md) | <span data-ttu-id="dfee8-131">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="dfee8-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="dfee8-132">获取已应用此策略的 directoryObjects 列表。</span><span class="sxs-lookup"><span data-stu-id="dfee8-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="dfee8-133">属性</span><span class="sxs-lookup"><span data-stu-id="dfee8-133">Properties</span></span>

| <span data-ttu-id="dfee8-134">属性</span><span class="sxs-lookup"><span data-stu-id="dfee8-134">Property</span></span>     | <span data-ttu-id="dfee8-135">类型</span><span class="sxs-lookup"><span data-stu-id="dfee8-135">Type</span></span>        | <span data-ttu-id="dfee8-136">说明</span><span class="sxs-lookup"><span data-stu-id="dfee8-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dfee8-137">id</span><span class="sxs-lookup"><span data-stu-id="dfee8-137">id</span></span>|<span data-ttu-id="dfee8-138">String</span><span class="sxs-lookup"><span data-stu-id="dfee8-138">String</span></span>| <span data-ttu-id="dfee8-139">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dfee8-139">Unique identifier for this policy.</span></span> <span data-ttu-id="dfee8-140">只读。</span><span class="sxs-lookup"><span data-stu-id="dfee8-140">Read-only.</span></span>|
|<span data-ttu-id="dfee8-141">definition</span><span class="sxs-lookup"><span data-stu-id="dfee8-141">definition</span></span>|<span data-ttu-id="dfee8-142">String collection</span><span class="sxs-lookup"><span data-stu-id="dfee8-142">String collection</span></span>| <span data-ttu-id="dfee8-143">包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="dfee8-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="dfee8-144">有关此属性的 JSON 架构的详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="dfee8-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="dfee8-145">必需。</span><span class="sxs-lookup"><span data-stu-id="dfee8-145">Required.</span></span>|
|<span data-ttu-id="dfee8-146">description</span><span class="sxs-lookup"><span data-stu-id="dfee8-146">description</span></span>|<span data-ttu-id="dfee8-147">String</span><span class="sxs-lookup"><span data-stu-id="dfee8-147">String</span></span>| <span data-ttu-id="dfee8-148">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="dfee8-148">Description for this policy.</span></span>|
|<span data-ttu-id="dfee8-149">displayName</span><span class="sxs-lookup"><span data-stu-id="dfee8-149">displayName</span></span>|<span data-ttu-id="dfee8-150">String</span><span class="sxs-lookup"><span data-stu-id="dfee8-150">String</span></span>| <span data-ttu-id="dfee8-151">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dfee8-151">Display name for this policy.</span></span> <span data-ttu-id="dfee8-152">必填。</span><span class="sxs-lookup"><span data-stu-id="dfee8-152">Required.</span></span>|
|<span data-ttu-id="dfee8-153">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="dfee8-153">isOrganizationDefault</span></span>|<span data-ttu-id="dfee8-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfee8-154">Boolean</span></span>|<span data-ttu-id="dfee8-155">忽略此属性。</span><span class="sxs-lookup"><span data-stu-id="dfee8-155">Ignore this property.</span></span> <span data-ttu-id="dfee8-156">令牌颁发策略只能应用于服务主体，并且不能为组织全局设置。</span><span class="sxs-lookup"><span data-stu-id="dfee8-156">The token-issuance policy can only be applied to service principals and can't be set globally for the organization.</span></span>|


### <a name="properties-of-a-token-issuance-policy-definition"></a><span data-ttu-id="dfee8-157">令牌颁发策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="dfee8-157">Properties of a token issuance policy definition</span></span>
<span data-ttu-id="dfee8-158">这些属性形成表示令牌颁发策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="dfee8-158">The properties form the JSON object that represents a token issuance policy.</span></span> <span data-ttu-id="dfee8-159">此 JSON 对象 **必须转换为带** 转义引号的字符串，以插入到 **定义** 属性中。</span><span class="sxs-lookup"><span data-stu-id="dfee8-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="dfee8-160">下面是 JSON 格式的示例：</span><span class="sxs-lookup"><span data-stu-id="dfee8-160">The following is an example in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| <span data-ttu-id="dfee8-161">属性</span><span class="sxs-lookup"><span data-stu-id="dfee8-161">Property</span></span>     | <span data-ttu-id="dfee8-162">类型</span><span class="sxs-lookup"><span data-stu-id="dfee8-162">Type</span></span>   |<span data-ttu-id="dfee8-163">说明</span><span class="sxs-lookup"><span data-stu-id="dfee8-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfee8-164">TokenResponseSigningPolicy</span><span class="sxs-lookup"><span data-stu-id="dfee8-164">TokenResponseSigningPolicy</span></span>|<span data-ttu-id="dfee8-165">String</span><span class="sxs-lookup"><span data-stu-id="dfee8-165">String</span></span>|<span data-ttu-id="dfee8-166">表示 Azure AD 中可用的证书签名选项。</span><span class="sxs-lookup"><span data-stu-id="dfee8-166">Represents the certificate signing options available in Azure AD.</span></span> <span data-ttu-id="dfee8-167">支持的值是： `ResponseOnly` ， `TokenOnly` `ResponseAndToken` 。</span><span class="sxs-lookup"><span data-stu-id="dfee8-167">Supported values are: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.</span></span>  |
|<span data-ttu-id="dfee8-168">SamlTokenVersion</span><span class="sxs-lookup"><span data-stu-id="dfee8-168">SamlTokenVersion</span></span>|<span data-ttu-id="dfee8-169">String</span><span class="sxs-lookup"><span data-stu-id="dfee8-169">String</span></span>|<span data-ttu-id="dfee8-170">SAML 令牌的版本。</span><span class="sxs-lookup"><span data-stu-id="dfee8-170">Version of the SAML token.</span></span> <span data-ttu-id="dfee8-171">支持的值是： `1.1` `2.0` 。</span><span class="sxs-lookup"><span data-stu-id="dfee8-171">Supported values are: `1.1`, `2.0`.</span></span> |
|<span data-ttu-id="dfee8-172">SigningAlgorithm</span><span class="sxs-lookup"><span data-stu-id="dfee8-172">SigningAlgorithm</span></span>|<span data-ttu-id="dfee8-173">String</span><span class="sxs-lookup"><span data-stu-id="dfee8-173">String</span></span>|<span data-ttu-id="dfee8-174">Azure AD 使用签名算法对 SAML 令牌进行签名。</span><span class="sxs-lookup"><span data-stu-id="dfee8-174">Signing algorithm use by Azure AD to sign the SAML token.</span></span> <span data-ttu-id="dfee8-175">支持的值是： `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256` `http://www.w3.org/2000/09/xmldsig#rsa-sha1` 。</span><span class="sxs-lookup"><span data-stu-id="dfee8-175">Supported values are: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.</span></span>|
|<span data-ttu-id="dfee8-176">版本</span><span class="sxs-lookup"><span data-stu-id="dfee8-176">Version</span></span>|<span data-ttu-id="dfee8-177">整数</span><span class="sxs-lookup"><span data-stu-id="dfee8-177">Integer</span></span>|<span data-ttu-id="dfee8-178">设置值 1。</span><span class="sxs-lookup"><span data-stu-id="dfee8-178">Set value of 1.</span></span> <span data-ttu-id="dfee8-179">必填。</span><span class="sxs-lookup"><span data-stu-id="dfee8-179">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="dfee8-180">关系</span><span class="sxs-lookup"><span data-stu-id="dfee8-180">Relationships</span></span>

| <span data-ttu-id="dfee8-181">关系</span><span class="sxs-lookup"><span data-stu-id="dfee8-181">Relationship</span></span> | <span data-ttu-id="dfee8-182">类型</span><span class="sxs-lookup"><span data-stu-id="dfee8-182">Type</span></span>        | <span data-ttu-id="dfee8-183">说明</span><span class="sxs-lookup"><span data-stu-id="dfee8-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dfee8-184">appliesTo</span><span class="sxs-lookup"><span data-stu-id="dfee8-184">appliesTo</span></span>|<span data-ttu-id="dfee8-185">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="dfee8-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="dfee8-186">已应用此策略的 [directoryObject](directoryObject.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="dfee8-186">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="dfee8-187">只读。</span><span class="sxs-lookup"><span data-stu-id="dfee8-187">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfee8-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfee8-188">JSON representation</span></span>

<span data-ttu-id="dfee8-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfee8-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
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
  "description": "tokenIssuancePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

