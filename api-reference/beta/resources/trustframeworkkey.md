---
title: trustFrameworkKey 资源类型
description: 表示 JWK （JSON Web 密钥）。 TrustFrameworkKey 是一个 JSON 数据结构，它表示加密密钥。 此资源的结构遵循 RFC 7517 第4节中定义的格式。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a9b94075b7a81fdb596038afac21fbf6cbc68f42
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519650"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="ce0d4-105">trustFrameworkKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce0d4-105">trustFrameworkKey resource type</span></span>

<span data-ttu-id="ce0d4-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ce0d4-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce0d4-107">表示 JWK （JSON Web 密钥）。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-107">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="ce0d4-108">TrustFrameworkKey 是一个 JSON 数据结构，它表示加密密钥。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-108">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="ce0d4-109">此资源的结构遵循[RFC 7517 第4节](https://tools.ietf.org/html/rfc7517#section-4)中定义的格式。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-109">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="ce0d4-110">属性</span><span class="sxs-lookup"><span data-stu-id="ce0d4-110">Properties</span></span>

| <span data-ttu-id="ce0d4-111">属性</span><span class="sxs-lookup"><span data-stu-id="ce0d4-111">Property</span></span>     | <span data-ttu-id="ce0d4-112">类型</span><span class="sxs-lookup"><span data-stu-id="ce0d4-112">Type</span></span>        | <span data-ttu-id="ce0d4-113">说明</span><span class="sxs-lookup"><span data-stu-id="ce0d4-113">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ce0d4-114">式</span><span class="sxs-lookup"><span data-stu-id="ce0d4-114">kid</span></span> | <span data-ttu-id="ce0d4-115">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-115">string</span></span> | <span data-ttu-id="ce0d4-116">键的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-116">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="ce0d4-117">kty</span><span class="sxs-lookup"><span data-stu-id="ce0d4-117">kty</span></span> | <span data-ttu-id="ce0d4-118">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-118">string</span></span> | <span data-ttu-id="ce0d4-119">"Kty" （key type）参数标识密钥使用的加密算法系列，有效值为 "rsa，oct"。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-119">The "kty" (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are rsa, oct.</span></span> |
| <span data-ttu-id="ce0d4-120">改用</span><span class="sxs-lookup"><span data-stu-id="ce0d4-120">use</span></span> | <span data-ttu-id="ce0d4-121">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-121">string</span></span> | <span data-ttu-id="ce0d4-122">"使用" （公钥使用）参数标识公钥的用途。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-122">The "use" (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="ce0d4-123">使用 "use" 参数来指示是否使用公钥对数据进行加密或验证数据签名。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-123">The "use" parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="ce0d4-124">可能的值为1。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-124">Possible values are    1.</span></span> <span data-ttu-id="ce0d4-125">"sig" （签名）2。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-125">"sig" (signature)    2.</span></span>  <span data-ttu-id="ce0d4-126">"enc" （加密）</span><span class="sxs-lookup"><span data-stu-id="ce0d4-126">"enc" (encryption)</span></span>   |
| <span data-ttu-id="ce0d4-127">x5c</span><span class="sxs-lookup"><span data-stu-id="ce0d4-127">x5c</span></span> | <span data-ttu-id="ce0d4-128">string 集合</span><span class="sxs-lookup"><span data-stu-id="ce0d4-128">string collection</span></span> | <span data-ttu-id="ce0d4-129">"X5c" （X. x.509 证书链）参数包含一个或多个 PKIX 证书[RFC 5280](https://tools.ietf.org/html/rfc5280)的链。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-129">The "x5c" (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="ce0d4-130">x5t</span><span class="sxs-lookup"><span data-stu-id="ce0d4-130">x5t</span></span> | <span data-ttu-id="ce0d4-131">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-131">string</span></span> | <span data-ttu-id="ce0d4-132">"X5t" （x.509 证书 SHA-1 指纹）参数是 base64url 编码的 SHA-1 指纹（a.k.a。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-132">The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="ce0d4-133">摘要）的 x.509 证书[RFC 5280](https://tools.ietf.org/html/rfc5280)的 DER 编码。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-133">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="ce0d4-134">e</span><span class="sxs-lookup"><span data-stu-id="ce0d4-134">e</span></span> | <span data-ttu-id="ce0d4-135">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-135">string</span></span> | <span data-ttu-id="ce0d4-136">RSA Key-公共指数</span><span class="sxs-lookup"><span data-stu-id="ce0d4-136">RSA Key - public exponent</span></span> |
| <span data-ttu-id="ce0d4-137">d</span><span class="sxs-lookup"><span data-stu-id="ce0d4-137">d</span></span>| <span data-ttu-id="ce0d4-138">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-138">string</span></span> | <span data-ttu-id="ce0d4-139">RSA Key-专用指数。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-139">RSA Key - private exponent.</span></span> <span data-ttu-id="ce0d4-140">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-140">Field cannot be read back.</span></span> |
| <span data-ttu-id="ce0d4-141">n</span><span class="sxs-lookup"><span data-stu-id="ce0d4-141">n</span></span> | <span data-ttu-id="ce0d4-142">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-142">string</span></span> | <span data-ttu-id="ce0d4-143">RSA Key-模数</span><span class="sxs-lookup"><span data-stu-id="ce0d4-143">RSA Key - modulus</span></span> |
| <span data-ttu-id="ce0d4-144">p</span><span class="sxs-lookup"><span data-stu-id="ce0d4-144">p</span></span> | <span data-ttu-id="ce0d4-145">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-145">string</span></span> | <span data-ttu-id="ce0d4-146">RSA 键-第一个质数。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-146">RSA Key - first prime.</span></span> <span data-ttu-id="ce0d4-147">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-147">Field cannot be read back.</span></span> |
| <span data-ttu-id="ce0d4-148">q</span><span class="sxs-lookup"><span data-stu-id="ce0d4-148">q</span></span> | <span data-ttu-id="ce0d4-149">字符串</span><span class="sxs-lookup"><span data-stu-id="ce0d4-149">string</span></span> | <span data-ttu-id="ce0d4-150">RSA 键-第二个质数。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-150">RSA Key - second prime.</span></span> <span data-ttu-id="ce0d4-151">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-151">Field cannot be read back.</span></span> |
| <span data-ttu-id="ce0d4-152">分发</span><span class="sxs-lookup"><span data-stu-id="ce0d4-152">dp</span></span> | <span data-ttu-id="ce0d4-153">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-153">string</span></span> | <span data-ttu-id="ce0d4-154">RSA Key-第一个指数。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-154">RSA Key - first exponent.</span></span> <span data-ttu-id="ce0d4-155">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-155">Field cannot be read back.</span></span> |
| <span data-ttu-id="ce0d4-156">dq</span><span class="sxs-lookup"><span data-stu-id="ce0d4-156">dq</span></span> | <span data-ttu-id="ce0d4-157">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-157">string</span></span> | <span data-ttu-id="ce0d4-158">RSA 键-第二个指数。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-158">RSA Key - second exponent.</span></span> <span data-ttu-id="ce0d4-159">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-159">Field cannot be read back.</span></span> |
| <span data-ttu-id="ce0d4-160">qi</span><span class="sxs-lookup"><span data-stu-id="ce0d4-160">qi</span></span> | <span data-ttu-id="ce0d4-161">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-161">string</span></span> | <span data-ttu-id="ce0d4-162">RSA 键-系数。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-162">RSA Key - Coefficient.</span></span> <span data-ttu-id="ce0d4-163">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-163">Field cannot be read back.</span></span> |
| <span data-ttu-id="ce0d4-164">kb</span><span class="sxs-lookup"><span data-stu-id="ce0d4-164">k</span></span> | <span data-ttu-id="ce0d4-165">string</span><span class="sxs-lookup"><span data-stu-id="ce0d4-165">string</span></span> | <span data-ttu-id="ce0d4-166">Oct 密钥类型的对称密钥。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-166">Symmetric Key for oct key type.</span></span> <span data-ttu-id="ce0d4-167">字段无法读回。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-167">Field cannot be read back.</span></span>   |
| <span data-ttu-id="ce0d4-168">nbf</span><span class="sxs-lookup"><span data-stu-id="ce0d4-168">nbf</span></span> | <span data-ttu-id="ce0d4-169">int</span><span class="sxs-lookup"><span data-stu-id="ce0d4-169">int</span></span> | <span data-ttu-id="ce0d4-170">此值是在 RFC 7519 中定义的 NumericDate （一个 JSON 数值，表示从 1970-01-01T00：00： 00Z UTC 到指定 UTC 日期/时间之间的秒数，忽略闰秒。）</span><span class="sxs-lookup"><span data-stu-id="ce0d4-170">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="ce0d4-171">exp</span><span class="sxs-lookup"><span data-stu-id="ce0d4-171">exp</span></span> | <span data-ttu-id="ce0d4-172">int</span><span class="sxs-lookup"><span data-stu-id="ce0d4-172">int</span></span> | <span data-ttu-id="ce0d4-173">此值是在 RFC 7519 中定义的 NumericDate （一个 JSON 数值，表示从 1970-01-01T00：00： 00Z UTC 到指定 UTC 日期/时间之间的秒数，忽略闰秒。）</span><span class="sxs-lookup"><span data-stu-id="ce0d4-173">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="ce0d4-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce0d4-174">JSON representation</span></span>

<span data-ttu-id="ce0d4-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce0d4-175">The following is a JSON representation of the resource.</span></span>

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
