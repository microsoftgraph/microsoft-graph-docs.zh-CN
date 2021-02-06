---
title: trustFrameworkKey 资源类型
description: 表示 JWK (JSON Web 密钥) 。 TrustFrameworkKey 是表示加密密钥的 JSON 数据结构。 此资源的结构遵循 RFC 7517 第 4 节中定义的格式。
localization_priority: Normal
author: valnav
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3de9ce67298f31b3c40682040da69f5c2f6ba007
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135854"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="06110-105">trustFrameworkKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="06110-105">trustFrameworkKey resource type</span></span>

<span data-ttu-id="06110-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06110-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06110-107">表示 JWK (JSON Web 密钥) 。</span><span class="sxs-lookup"><span data-stu-id="06110-107">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="06110-108">TrustFrameworkKey 是表示加密密钥的 JSON 数据结构。</span><span class="sxs-lookup"><span data-stu-id="06110-108">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="06110-109">此资源的结构遵循 [RFC 7517 第 4 节中定义的格式](https://tools.ietf.org/html/rfc7517#section-4)。</span><span class="sxs-lookup"><span data-stu-id="06110-109">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="06110-110">属性</span><span class="sxs-lookup"><span data-stu-id="06110-110">Properties</span></span>

| <span data-ttu-id="06110-111">属性</span><span class="sxs-lookup"><span data-stu-id="06110-111">Property</span></span>     | <span data-ttu-id="06110-112">类型</span><span class="sxs-lookup"><span data-stu-id="06110-112">Type</span></span>        | <span data-ttu-id="06110-113">说明</span><span class="sxs-lookup"><span data-stu-id="06110-113">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="06110-114">一些</span><span class="sxs-lookup"><span data-stu-id="06110-114">kid</span></span> | <span data-ttu-id="06110-115">string</span><span class="sxs-lookup"><span data-stu-id="06110-115">string</span></span> | <span data-ttu-id="06110-116">密钥的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="06110-116">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="06110-117">kty</span><span class="sxs-lookup"><span data-stu-id="06110-117">kty</span></span> | <span data-ttu-id="06110-118">string</span><span class="sxs-lookup"><span data-stu-id="06110-118">string</span></span> | <span data-ttu-id="06110-119">"kty" (类型) 参数标识用于密钥的加密算法系列，有效值为 rsa、oct。</span><span class="sxs-lookup"><span data-stu-id="06110-119">The "kty" (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are rsa, oct.</span></span> |
| <span data-ttu-id="06110-120">use</span><span class="sxs-lookup"><span data-stu-id="06110-120">use</span></span> | <span data-ttu-id="06110-121">string</span><span class="sxs-lookup"><span data-stu-id="06110-121">string</span></span> | <span data-ttu-id="06110-122">"use" (使用) 参数标识公钥的预定用途。</span><span class="sxs-lookup"><span data-stu-id="06110-122">The "use" (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="06110-123">"use"参数用于指示公钥是否用于加密数据或验证数据上的签名。</span><span class="sxs-lookup"><span data-stu-id="06110-123">The "use" parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="06110-124">可能的值是 1。</span><span class="sxs-lookup"><span data-stu-id="06110-124">Possible values are    1.</span></span> <span data-ttu-id="06110-125">"sig" (2) 签名。</span><span class="sxs-lookup"><span data-stu-id="06110-125">"sig" (signature)    2.</span></span>  <span data-ttu-id="06110-126">"enc" (加密) </span><span class="sxs-lookup"><span data-stu-id="06110-126">"enc" (encryption)</span></span>   |
| <span data-ttu-id="06110-127">x5c</span><span class="sxs-lookup"><span data-stu-id="06110-127">x5c</span></span> | <span data-ttu-id="06110-128">string 集合</span><span class="sxs-lookup"><span data-stu-id="06110-128">string collection</span></span> | <span data-ttu-id="06110-129">"x5c" (X.509 证书链) 参数包含一个或多个 PKIX 证书 [RFC 5280 的链](https://tools.ietf.org/html/rfc5280)。</span><span class="sxs-lookup"><span data-stu-id="06110-129">The "x5c" (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="06110-130">x5t</span><span class="sxs-lookup"><span data-stu-id="06110-130">x5t</span></span> | <span data-ttu-id="06110-131">string</span><span class="sxs-lookup"><span data-stu-id="06110-131">string</span></span> | <span data-ttu-id="06110-132">"x5t" (X.509 证书 SHA-1 指纹) 参数是 base64url 编码的 SHA-1 指纹 (a.k.a。</span><span class="sxs-lookup"><span data-stu-id="06110-132">The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="06110-133">摘要) X.509 证书 [RFC 5280](https://tools.ietf.org/html/rfc5280)的 DER 编码。</span><span class="sxs-lookup"><span data-stu-id="06110-133">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="06110-134">e</span><span class="sxs-lookup"><span data-stu-id="06110-134">e</span></span> | <span data-ttu-id="06110-135">string</span><span class="sxs-lookup"><span data-stu-id="06110-135">string</span></span> | <span data-ttu-id="06110-136">RSA 密钥 - 公共指数</span><span class="sxs-lookup"><span data-stu-id="06110-136">RSA Key - public exponent</span></span> |
| <span data-ttu-id="06110-137">d</span><span class="sxs-lookup"><span data-stu-id="06110-137">d</span></span>| <span data-ttu-id="06110-138">string</span><span class="sxs-lookup"><span data-stu-id="06110-138">string</span></span> | <span data-ttu-id="06110-139">RSA 密钥 - 私有指数。</span><span class="sxs-lookup"><span data-stu-id="06110-139">RSA Key - private exponent.</span></span> <span data-ttu-id="06110-140">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="06110-140">Field cannot be read back.</span></span> |
| <span data-ttu-id="06110-141">n</span><span class="sxs-lookup"><span data-stu-id="06110-141">n</span></span> | <span data-ttu-id="06110-142">string</span><span class="sxs-lookup"><span data-stu-id="06110-142">string</span></span> | <span data-ttu-id="06110-143">RSA 密钥 - 模数</span><span class="sxs-lookup"><span data-stu-id="06110-143">RSA Key - modulus</span></span> |
| <span data-ttu-id="06110-144">p</span><span class="sxs-lookup"><span data-stu-id="06110-144">p</span></span> | <span data-ttu-id="06110-145">string</span><span class="sxs-lookup"><span data-stu-id="06110-145">string</span></span> | <span data-ttu-id="06110-146">RSA 密钥 - 第一个主密钥。</span><span class="sxs-lookup"><span data-stu-id="06110-146">RSA Key - first prime.</span></span> <span data-ttu-id="06110-147">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="06110-147">Field cannot be read back.</span></span> |
| <span data-ttu-id="06110-148">q</span><span class="sxs-lookup"><span data-stu-id="06110-148">q</span></span> | <span data-ttu-id="06110-149">字符串</span><span class="sxs-lookup"><span data-stu-id="06110-149">string</span></span> | <span data-ttu-id="06110-150">RSA 密钥 - 第二级。</span><span class="sxs-lookup"><span data-stu-id="06110-150">RSA Key - second prime.</span></span> <span data-ttu-id="06110-151">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="06110-151">Field cannot be read back.</span></span> |
| <span data-ttu-id="06110-152">dp</span><span class="sxs-lookup"><span data-stu-id="06110-152">dp</span></span> | <span data-ttu-id="06110-153">string</span><span class="sxs-lookup"><span data-stu-id="06110-153">string</span></span> | <span data-ttu-id="06110-154">RSA 密钥 - 第一个指数。</span><span class="sxs-lookup"><span data-stu-id="06110-154">RSA Key - first exponent.</span></span> <span data-ttu-id="06110-155">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="06110-155">Field cannot be read back.</span></span> |
| <span data-ttu-id="06110-156">dq</span><span class="sxs-lookup"><span data-stu-id="06110-156">dq</span></span> | <span data-ttu-id="06110-157">string</span><span class="sxs-lookup"><span data-stu-id="06110-157">string</span></span> | <span data-ttu-id="06110-158">RSA 密钥 - 第二个指数。</span><span class="sxs-lookup"><span data-stu-id="06110-158">RSA Key - second exponent.</span></span> <span data-ttu-id="06110-159">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="06110-159">Field cannot be read back.</span></span> |
| <span data-ttu-id="06110-160">一些</span><span class="sxs-lookup"><span data-stu-id="06110-160">qi</span></span> | <span data-ttu-id="06110-161">string</span><span class="sxs-lookup"><span data-stu-id="06110-161">string</span></span> | <span data-ttu-id="06110-162">RSA 键 - 系数。</span><span class="sxs-lookup"><span data-stu-id="06110-162">RSA Key - Coefficient.</span></span> <span data-ttu-id="06110-163">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="06110-163">Field cannot be read back.</span></span> |
| <span data-ttu-id="06110-164">k</span><span class="sxs-lookup"><span data-stu-id="06110-164">k</span></span> | <span data-ttu-id="06110-165">string</span><span class="sxs-lookup"><span data-stu-id="06110-165">string</span></span> | <span data-ttu-id="06110-166">八进制密钥类型的对称密钥。</span><span class="sxs-lookup"><span data-stu-id="06110-166">Symmetric Key for oct key type.</span></span> <span data-ttu-id="06110-167">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="06110-167">Field cannot be read back.</span></span>   |
| <span data-ttu-id="06110-168">nbf</span><span class="sxs-lookup"><span data-stu-id="06110-168">nbf</span></span> | <span data-ttu-id="06110-169">int</span><span class="sxs-lookup"><span data-stu-id="06110-169">int</span></span> | <span data-ttu-id="06110-170">此值是 RFC 7519 (中定义的 NumericDate。JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跨越秒数）的秒数。) </span><span class="sxs-lookup"><span data-stu-id="06110-170">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="06110-171">exp</span><span class="sxs-lookup"><span data-stu-id="06110-171">exp</span></span> | <span data-ttu-id="06110-172">int</span><span class="sxs-lookup"><span data-stu-id="06110-172">int</span></span> | <span data-ttu-id="06110-173">此值是 RFC 7519 (中定义的 NumericDate。JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跨越秒数）的秒数。) </span><span class="sxs-lookup"><span data-stu-id="06110-173">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="06110-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06110-174">JSON representation</span></span>

<span data-ttu-id="06110-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06110-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKey",
  "baseType": null
}-->

```json
{
  "d": "String",
  "dp": "String",
  "dq": "String",
  "e": "String",
  "exp": 1024,
  "k": "String",
  "kid": "String",
  "kty": "String",
  "n": "String",
  "nbf": 1024,
  "p": "String",
  "q": "String",
  "qi": "String",
  "use": "String",
  "x5c": ["String"],
  "x5t": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKey resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


