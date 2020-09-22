---
title: tokenIssuancePolicy 资源类型
description: 表示指定由 Azure AD 颁发的 SAML 令牌的特征的策略。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f26ad245bfbbcc821753bddb9bdb346e399cd560
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057967"
---
# <a name="tokenissuancepolicy-resource-type"></a><span data-ttu-id="0dad7-103">tokenIssuancePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="0dad7-103">tokenIssuancePolicy resource type</span></span>

<span data-ttu-id="0dad7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dad7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dad7-105">表示指定由 Azure AD 颁发的 SAML 令牌的特征的策略。</span><span class="sxs-lookup"><span data-stu-id="0dad7-105">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span> <span data-ttu-id="0dad7-106">您可以使用令牌颁发策略执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="0dad7-106">You can use token-issuance policies to:</span></span>

- <span data-ttu-id="0dad7-107">设置签名选项</span><span class="sxs-lookup"><span data-stu-id="0dad7-107">Set signing options</span></span>
- <span data-ttu-id="0dad7-108">设置签名算法</span><span class="sxs-lookup"><span data-stu-id="0dad7-108">Set signing algorithm</span></span>
- <span data-ttu-id="0dad7-109">设置 SAML 令牌版本</span><span class="sxs-lookup"><span data-stu-id="0dad7-109">Set SAML token version</span></span>

<span data-ttu-id="0dad7-110">继承自 [stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="0dad7-110">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0dad7-111">方法</span><span class="sxs-lookup"><span data-stu-id="0dad7-111">Methods</span></span>

| <span data-ttu-id="0dad7-112">方法</span><span class="sxs-lookup"><span data-stu-id="0dad7-112">Method</span></span>       | <span data-ttu-id="0dad7-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="0dad7-113">Return Type</span></span> | <span data-ttu-id="0dad7-114">说明</span><span class="sxs-lookup"><span data-stu-id="0dad7-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0dad7-115">创建 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="0dad7-115">Create tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [<span data-ttu-id="0dad7-116">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="0dad7-116">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="0dad7-117">创建 tokenIssuancePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="0dad7-117">Create a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="0dad7-118">获取 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="0dad7-118">Get tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-get.md) | [<span data-ttu-id="0dad7-119">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="0dad7-119">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="0dad7-120">读取 tokenIssuancePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0dad7-120">Read properties and relationships of a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="0dad7-121">列出 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="0dad7-121">List tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-list.md) | [<span data-ttu-id="0dad7-122">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="0dad7-122">tokenIssuancePolicy</span></span>](tokenissuancepolicy.md) | <span data-ttu-id="0dad7-123">读取 tokenIssuancePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0dad7-123">Read properties and relationships of tokenIssuancePolicy objects.</span></span> |
| [<span data-ttu-id="0dad7-124">更新 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="0dad7-124">Update tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-update.md) | <span data-ttu-id="0dad7-125">无</span><span class="sxs-lookup"><span data-stu-id="0dad7-125">None</span></span> | <span data-ttu-id="0dad7-126">更新 tokenIssuancePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="0dad7-126">Update a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="0dad7-127">删除 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="0dad7-127">Delete tokenIssuancePolicy</span></span>](../api/tokenissuancepolicy-delete.md) | <span data-ttu-id="0dad7-128">无</span><span class="sxs-lookup"><span data-stu-id="0dad7-128">None</span></span> | <span data-ttu-id="0dad7-129">删除 tokenIssuancePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="0dad7-129">Delete a tokenIssuancePolicy object.</span></span> |
| [<span data-ttu-id="0dad7-130">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="0dad7-130">List appliesTo</span></span>](../api/tokenissuancepolicy-list-appliesto.md) | <span data-ttu-id="0dad7-131">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0dad7-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="0dad7-132">获取已应用此策略的 directoryObjects 的列表。</span><span class="sxs-lookup"><span data-stu-id="0dad7-132">Get the list of directoryObjects that this policy has been applied to.</span></span> |

## <a name="properties"></a><span data-ttu-id="0dad7-133">属性</span><span class="sxs-lookup"><span data-stu-id="0dad7-133">Properties</span></span>

| <span data-ttu-id="0dad7-134">属性</span><span class="sxs-lookup"><span data-stu-id="0dad7-134">Property</span></span>     | <span data-ttu-id="0dad7-135">类型</span><span class="sxs-lookup"><span data-stu-id="0dad7-135">Type</span></span>        | <span data-ttu-id="0dad7-136">说明</span><span class="sxs-lookup"><span data-stu-id="0dad7-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0dad7-137">id</span><span class="sxs-lookup"><span data-stu-id="0dad7-137">id</span></span>|<span data-ttu-id="0dad7-138">String</span><span class="sxs-lookup"><span data-stu-id="0dad7-138">String</span></span>| <span data-ttu-id="0dad7-139">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0dad7-139">Unique identifier for this policy.</span></span> <span data-ttu-id="0dad7-140">只读。</span><span class="sxs-lookup"><span data-stu-id="0dad7-140">Read-only.</span></span>|
|<span data-ttu-id="0dad7-141">定义</span><span class="sxs-lookup"><span data-stu-id="0dad7-141">definition</span></span>|<span data-ttu-id="0dad7-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="0dad7-142">String collection</span></span>| <span data-ttu-id="0dad7-143">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="0dad7-143">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="0dad7-144">有关此属性的 JSON 架构的更多详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="0dad7-144">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="0dad7-145">必需。</span><span class="sxs-lookup"><span data-stu-id="0dad7-145">Required.</span></span>|
|<span data-ttu-id="0dad7-146">description</span><span class="sxs-lookup"><span data-stu-id="0dad7-146">description</span></span>|<span data-ttu-id="0dad7-147">String</span><span class="sxs-lookup"><span data-stu-id="0dad7-147">String</span></span>| <span data-ttu-id="0dad7-148">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="0dad7-148">Description for this policy.</span></span>|
|<span data-ttu-id="0dad7-149">displayName</span><span class="sxs-lookup"><span data-stu-id="0dad7-149">displayName</span></span>|<span data-ttu-id="0dad7-150">String</span><span class="sxs-lookup"><span data-stu-id="0dad7-150">String</span></span>| <span data-ttu-id="0dad7-151">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0dad7-151">Display name for this policy.</span></span> <span data-ttu-id="0dad7-152">必需。</span><span class="sxs-lookup"><span data-stu-id="0dad7-152">Required.</span></span>|
|<span data-ttu-id="0dad7-153">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="0dad7-153">isOrganizationDefault</span></span>|<span data-ttu-id="0dad7-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="0dad7-154">Boolean</span></span>|<span data-ttu-id="0dad7-155">忽略此属性。</span><span class="sxs-lookup"><span data-stu-id="0dad7-155">Ignore this property.</span></span> <span data-ttu-id="0dad7-156">令牌颁发策略仅适用于服务主体，不能为组织全局设置。</span><span class="sxs-lookup"><span data-stu-id="0dad7-156">The token-issuance policy can only be applied to service principals and can't be set globally for the organization.</span></span>|


### <a name="properties-of-a-token-issuance-policy-definition"></a><span data-ttu-id="0dad7-157">令牌颁发策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="0dad7-157">Properties of a token issuance policy definition</span></span>
<span data-ttu-id="0dad7-158">属性构成表示令牌颁发策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0dad7-158">The properties form the JSON object that represents a token issuance policy.</span></span> <span data-ttu-id="0dad7-159">此 JSON 对象必须 **转换为转义了引号的字符串** ，以将其插入到 **定义** 属性中。</span><span class="sxs-lookup"><span data-stu-id="0dad7-159">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="0dad7-160">以下是 JSON 格式的示例：</span><span class="sxs-lookup"><span data-stu-id="0dad7-160">The following is an example in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| <span data-ttu-id="0dad7-161">属性</span><span class="sxs-lookup"><span data-stu-id="0dad7-161">Property</span></span>     | <span data-ttu-id="0dad7-162">类型</span><span class="sxs-lookup"><span data-stu-id="0dad7-162">Type</span></span>   |<span data-ttu-id="0dad7-163">说明</span><span class="sxs-lookup"><span data-stu-id="0dad7-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0dad7-164">TokenResponseSigningPolicy</span><span class="sxs-lookup"><span data-stu-id="0dad7-164">TokenResponseSigningPolicy</span></span>|<span data-ttu-id="0dad7-165">String</span><span class="sxs-lookup"><span data-stu-id="0dad7-165">String</span></span>|<span data-ttu-id="0dad7-166">表示 Azure AD 中可用的证书签名选项。</span><span class="sxs-lookup"><span data-stu-id="0dad7-166">Represents the certificate signing options available in Azure AD.</span></span> <span data-ttu-id="0dad7-167">支持的值为： `ResponseOnly` 、 `TokenOnly` 、 `ResponseAndToken` 。</span><span class="sxs-lookup"><span data-stu-id="0dad7-167">Supported values are: `ResponseOnly`, `TokenOnly`, `ResponseAndToken`.</span></span>  |
|<span data-ttu-id="0dad7-168">SamlTokenVersion</span><span class="sxs-lookup"><span data-stu-id="0dad7-168">SamlTokenVersion</span></span>|<span data-ttu-id="0dad7-169">String</span><span class="sxs-lookup"><span data-stu-id="0dad7-169">String</span></span>|<span data-ttu-id="0dad7-170">SAML 令牌的版本。</span><span class="sxs-lookup"><span data-stu-id="0dad7-170">Version of the SAML token.</span></span> <span data-ttu-id="0dad7-171">支持的值为： `1.1` 、 `2.0` 。</span><span class="sxs-lookup"><span data-stu-id="0dad7-171">Supported values are: `1.1`, `2.0`.</span></span> |
|<span data-ttu-id="0dad7-172">SigningAlgorithm</span><span class="sxs-lookup"><span data-stu-id="0dad7-172">SigningAlgorithm</span></span>|<span data-ttu-id="0dad7-173">String</span><span class="sxs-lookup"><span data-stu-id="0dad7-173">String</span></span>|<span data-ttu-id="0dad7-174">Azure AD 使用的签名算法对 SAML 令牌进行签名。</span><span class="sxs-lookup"><span data-stu-id="0dad7-174">Signing algorithm use by Azure AD to sign the SAML token.</span></span> <span data-ttu-id="0dad7-175">支持的值为： `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256` 、 `http://www.w3.org/2000/09/xmldsig#rsa-sha1` 。</span><span class="sxs-lookup"><span data-stu-id="0dad7-175">Supported values are: `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`, `http://www.w3.org/2000/09/xmldsig#rsa-sha1`.</span></span>|
|<span data-ttu-id="0dad7-176">版本</span><span class="sxs-lookup"><span data-stu-id="0dad7-176">Version</span></span>|<span data-ttu-id="0dad7-177">整数</span><span class="sxs-lookup"><span data-stu-id="0dad7-177">Integer</span></span>|<span data-ttu-id="0dad7-178">将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="0dad7-178">Set value of 1.</span></span> <span data-ttu-id="0dad7-179">必需。</span><span class="sxs-lookup"><span data-stu-id="0dad7-179">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="0dad7-180">关系</span><span class="sxs-lookup"><span data-stu-id="0dad7-180">Relationships</span></span>

| <span data-ttu-id="0dad7-181">关系</span><span class="sxs-lookup"><span data-stu-id="0dad7-181">Relationship</span></span> | <span data-ttu-id="0dad7-182">类型</span><span class="sxs-lookup"><span data-stu-id="0dad7-182">Type</span></span>        | <span data-ttu-id="0dad7-183">说明</span><span class="sxs-lookup"><span data-stu-id="0dad7-183">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0dad7-184">appliesTo</span><span class="sxs-lookup"><span data-stu-id="0dad7-184">appliesTo</span></span>|<span data-ttu-id="0dad7-185">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0dad7-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="0dad7-186">已将此策略应用于的 [directoryObject](directoryObject.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="0dad7-186">The [directoryObject](directoryObject.md) collection that this policy has been applied to.</span></span> <span data-ttu-id="0dad7-187">只读。</span><span class="sxs-lookup"><span data-stu-id="0dad7-187">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0dad7-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0dad7-188">JSON representation</span></span>

<span data-ttu-id="0dad7-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0dad7-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
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
  "description": "tokenIssuancePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


