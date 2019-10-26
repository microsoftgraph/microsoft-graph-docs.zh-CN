---
title: trustFrameworkKey 资源类型
description: 表示 JWK （JSON Web 密钥）。 TrustFrameworkKey 是一个 JSON 数据结构，它表示加密密钥。 此资源的结构遵循 RFC 7517 第4节中定义的格式。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7d61548707d9530d30f81b61ad88dd29ae2576c8
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734563"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="dd7ae-105">trustFrameworkKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd7ae-105">trustFrameworkKey resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd7ae-106">表示 JWK （JSON Web 密钥）。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-106">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="dd7ae-107">TrustFrameworkKey 是一个 JSON 数据结构，它表示加密密钥。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-107">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="dd7ae-108">此资源的结构遵循[RFC 7517 第4节](https://tools.ietf.org/html/rfc7517#section-4)中定义的格式。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-108">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="dd7ae-109">属性</span><span class="sxs-lookup"><span data-stu-id="dd7ae-109">Properties</span></span>

| <span data-ttu-id="dd7ae-110">属性</span><span class="sxs-lookup"><span data-stu-id="dd7ae-110">Property</span></span>     | <span data-ttu-id="dd7ae-111">类型</span><span class="sxs-lookup"><span data-stu-id="dd7ae-111">Type</span></span>        | <span data-ttu-id="dd7ae-112">说明</span><span class="sxs-lookup"><span data-stu-id="dd7ae-112">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="dd7ae-113">式</span><span class="sxs-lookup"><span data-stu-id="dd7ae-113">kid</span></span> | <span data-ttu-id="dd7ae-114">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-114">string</span></span> | <span data-ttu-id="dd7ae-115">键的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-115">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="dd7ae-116">kty</span><span class="sxs-lookup"><span data-stu-id="dd7ae-116">kty</span></span> | <span data-ttu-id="dd7ae-117">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-117">string</span></span> | <span data-ttu-id="dd7ae-118">"Kty" （key type）参数标识密钥使用的加密算法系列，有效值为 "rsa，oct"。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-118">The "kty" (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are rsa, oct.</span></span> |
| <span data-ttu-id="dd7ae-119">改用</span><span class="sxs-lookup"><span data-stu-id="dd7ae-119">use</span></span> | <span data-ttu-id="dd7ae-120">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-120">string</span></span> | <span data-ttu-id="dd7ae-121">"使用" （公钥使用）参数标识公钥的用途。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-121">The "use" (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="dd7ae-122">使用 "use" 参数来指示是否使用公钥对数据进行加密或验证数据签名。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-122">The "use" parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="dd7ae-123">可能的值为1。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-123">Possible values are    1.</span></span> <span data-ttu-id="dd7ae-124">"sig" （签名）2。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-124">"sig" (signature)    2.</span></span>  <span data-ttu-id="dd7ae-125">"enc" （加密）</span><span class="sxs-lookup"><span data-stu-id="dd7ae-125">"enc" (encryption)</span></span>   |
| <span data-ttu-id="dd7ae-126">x5c</span><span class="sxs-lookup"><span data-stu-id="dd7ae-126">x5c</span></span> | <span data-ttu-id="dd7ae-127">string 集合</span><span class="sxs-lookup"><span data-stu-id="dd7ae-127">string collection</span></span> | <span data-ttu-id="dd7ae-128">"X5c" （X. x.509 证书链）参数包含一个或多个 PKIX 证书[RFC 5280](https://tools.ietf.org/html/rfc5280)的链。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-128">The "x5c" (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="dd7ae-129">x5t</span><span class="sxs-lookup"><span data-stu-id="dd7ae-129">x5t</span></span> | <span data-ttu-id="dd7ae-130">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-130">string</span></span> | <span data-ttu-id="dd7ae-131">"X5t" （x.509 证书 SHA-1 指纹）参数是 base64url 编码的 SHA-1 指纹（a.k.a。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-131">The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="dd7ae-132">摘要）的 x.509 证书[RFC 5280](https://tools.ietf.org/html/rfc5280)的 DER 编码。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-132">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="dd7ae-133">e</span><span class="sxs-lookup"><span data-stu-id="dd7ae-133">e</span></span> | <span data-ttu-id="dd7ae-134">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-134">string</span></span> | <span data-ttu-id="dd7ae-135">RSA Key-公共指数</span><span class="sxs-lookup"><span data-stu-id="dd7ae-135">RSA Key - public exponent</span></span> |
| <span data-ttu-id="dd7ae-136">d</span><span class="sxs-lookup"><span data-stu-id="dd7ae-136">d</span></span>| <span data-ttu-id="dd7ae-137">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-137">string</span></span> | <span data-ttu-id="dd7ae-138">RSA Key-专用指数。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-138">RSA Key - private exponent.</span></span> <span data-ttu-id="dd7ae-139">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-139">Field cannot be read back.</span></span> |
| <span data-ttu-id="dd7ae-140">n</span><span class="sxs-lookup"><span data-stu-id="dd7ae-140">n</span></span> | <span data-ttu-id="dd7ae-141">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-141">string</span></span> | <span data-ttu-id="dd7ae-142">RSA Key-模数</span><span class="sxs-lookup"><span data-stu-id="dd7ae-142">RSA Key - modulus</span></span> |
| <span data-ttu-id="dd7ae-143">p</span><span class="sxs-lookup"><span data-stu-id="dd7ae-143">p</span></span> | <span data-ttu-id="dd7ae-144">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-144">string</span></span> | <span data-ttu-id="dd7ae-145">RSA 键-第一个质数。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-145">RSA Key - first prime.</span></span> <span data-ttu-id="dd7ae-146">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-146">Field cannot be read back.</span></span> |
| <span data-ttu-id="dd7ae-147">q</span><span class="sxs-lookup"><span data-stu-id="dd7ae-147">q</span></span> | <span data-ttu-id="dd7ae-148">字符串</span><span class="sxs-lookup"><span data-stu-id="dd7ae-148">string</span></span> | <span data-ttu-id="dd7ae-149">RSA 键-第二个质数。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-149">RSA Key - second prime.</span></span> <span data-ttu-id="dd7ae-150">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-150">Field cannot be read back.</span></span> |
| <span data-ttu-id="dd7ae-151">分发</span><span class="sxs-lookup"><span data-stu-id="dd7ae-151">dp</span></span> | <span data-ttu-id="dd7ae-152">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-152">string</span></span> | <span data-ttu-id="dd7ae-153">RSA Key-第一个指数。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-153">RSA Key - first exponent.</span></span> <span data-ttu-id="dd7ae-154">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-154">Field cannot be read back.</span></span> |
| <span data-ttu-id="dd7ae-155">dq</span><span class="sxs-lookup"><span data-stu-id="dd7ae-155">dq</span></span> | <span data-ttu-id="dd7ae-156">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-156">string</span></span> | <span data-ttu-id="dd7ae-157">RSA 键-第二个指数。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-157">RSA Key - second exponent.</span></span> <span data-ttu-id="dd7ae-158">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-158">Field cannot be read back.</span></span> |
| <span data-ttu-id="dd7ae-159">qi</span><span class="sxs-lookup"><span data-stu-id="dd7ae-159">qi</span></span> | <span data-ttu-id="dd7ae-160">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-160">string</span></span> | <span data-ttu-id="dd7ae-161">RSA 键-系数。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-161">RSA Key - Coefficient.</span></span> <span data-ttu-id="dd7ae-162">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-162">Field cannot be read back.</span></span> |
| <span data-ttu-id="dd7ae-163">kb</span><span class="sxs-lookup"><span data-stu-id="dd7ae-163">k</span></span> | <span data-ttu-id="dd7ae-164">string</span><span class="sxs-lookup"><span data-stu-id="dd7ae-164">string</span></span> | <span data-ttu-id="dd7ae-165">Oct 密钥类型的对称密钥。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-165">Symmetric Key for oct key type.</span></span> <span data-ttu-id="dd7ae-166">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-166">Field cannot be read back.</span></span>   |
| <span data-ttu-id="dd7ae-167">nbf</span><span class="sxs-lookup"><span data-stu-id="dd7ae-167">nbf</span></span> | <span data-ttu-id="dd7ae-168">int</span><span class="sxs-lookup"><span data-stu-id="dd7ae-168">int</span></span> | <span data-ttu-id="dd7ae-169">此值是在 RFC 7519 中定义的 NumericDate （一个 JSON 数值，表示从 1970-01-01T00：00： 00Z UTC 到指定 UTC 日期/时间之间的秒数，忽略闰秒。）</span><span class="sxs-lookup"><span data-stu-id="dd7ae-169">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="dd7ae-170">exp</span><span class="sxs-lookup"><span data-stu-id="dd7ae-170">exp</span></span> | <span data-ttu-id="dd7ae-171">int</span><span class="sxs-lookup"><span data-stu-id="dd7ae-171">int</span></span> | <span data-ttu-id="dd7ae-172">此值是在 RFC 7519 中定义的 NumericDate （一个 JSON 数值，表示从 1970-01-01T00：00： 00Z UTC 到指定 UTC 日期/时间之间的秒数，忽略闰秒。）</span><span class="sxs-lookup"><span data-stu-id="dd7ae-172">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="dd7ae-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd7ae-173">JSON representation</span></span>

<span data-ttu-id="dd7ae-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd7ae-174">The following is a JSON representation of the resource.</span></span>

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
