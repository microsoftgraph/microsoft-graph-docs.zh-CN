---
title: trustFrameworkKey 资源类型
description: 表示 JWK (JSON Web 密钥) 。 TrustFrameworkKey 是表示加密密钥的 JSON 数据结构。 此资源的结构遵循 RFC 7517 第 4 节中定义的格式。
localization_priority: Normal
author: valnav
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b50e82748db6c0c26252ce6b79290781fa88819b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945632"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="9625a-105">trustFrameworkKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="9625a-105">trustFrameworkKey resource type</span></span>

<span data-ttu-id="9625a-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9625a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9625a-107">表示 JWK (JSON Web 密钥) 。</span><span class="sxs-lookup"><span data-stu-id="9625a-107">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="9625a-108">TrustFrameworkKey 是表示加密密钥的 JSON 数据结构。</span><span class="sxs-lookup"><span data-stu-id="9625a-108">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="9625a-109">此资源的结构遵循 [RFC 7517 第 4 节中定义的格式](https://tools.ietf.org/html/rfc7517#section-4)。</span><span class="sxs-lookup"><span data-stu-id="9625a-109">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="9625a-110">属性</span><span class="sxs-lookup"><span data-stu-id="9625a-110">Properties</span></span>

| <span data-ttu-id="9625a-111">属性</span><span class="sxs-lookup"><span data-stu-id="9625a-111">Property</span></span>     | <span data-ttu-id="9625a-112">类型</span><span class="sxs-lookup"><span data-stu-id="9625a-112">Type</span></span>        | <span data-ttu-id="9625a-113">说明</span><span class="sxs-lookup"><span data-stu-id="9625a-113">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9625a-114">一些</span><span class="sxs-lookup"><span data-stu-id="9625a-114">kid</span></span> | <span data-ttu-id="9625a-115">string</span><span class="sxs-lookup"><span data-stu-id="9625a-115">string</span></span> | <span data-ttu-id="9625a-116">密钥的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9625a-116">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="9625a-117">kty</span><span class="sxs-lookup"><span data-stu-id="9625a-117">kty</span></span> | <span data-ttu-id="9625a-118">String</span><span class="sxs-lookup"><span data-stu-id="9625a-118">String</span></span> | <span data-ttu-id="9625a-119">**keyty** (类型) 参数标识与密钥一同使用的加密算法系列，有效值为 、 `rsa` `oct` 。</span><span class="sxs-lookup"><span data-stu-id="9625a-119">The **kty** (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are `rsa`, `oct`.</span></span> |
| <span data-ttu-id="9625a-120">use</span><span class="sxs-lookup"><span data-stu-id="9625a-120">use</span></span> | <span data-ttu-id="9625a-121">String</span><span class="sxs-lookup"><span data-stu-id="9625a-121">String</span></span> | <span data-ttu-id="9625a-122">**公钥** (参数) 标识公钥的预定用途。</span><span class="sxs-lookup"><span data-stu-id="9625a-122">The **use** (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="9625a-123">**use** 参数用于指示公钥是否用于加密数据或验证数据签名。</span><span class="sxs-lookup"><span data-stu-id="9625a-123">The **use** parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="9625a-124">可能的值包括 `sig` ： (签名)  (`enc` 加密) </span><span class="sxs-lookup"><span data-stu-id="9625a-124">Possible values are: `sig` (signature), `enc` (encryption)</span></span>  |
| <span data-ttu-id="9625a-125">x5c</span><span class="sxs-lookup"><span data-stu-id="9625a-125">x5c</span></span> | <span data-ttu-id="9625a-126">string 集合</span><span class="sxs-lookup"><span data-stu-id="9625a-126">string collection</span></span> | <span data-ttu-id="9625a-127">**x5c (** X.509 证书链) 参数包含一个或多个 PKIX 证书 [的链 RFC 5280。](https://tools.ietf.org/html/rfc5280)</span><span class="sxs-lookup"><span data-stu-id="9625a-127">The **x5c** (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="9625a-128">x5t</span><span class="sxs-lookup"><span data-stu-id="9625a-128">x5t</span></span> | <span data-ttu-id="9625a-129">string</span><span class="sxs-lookup"><span data-stu-id="9625a-129">string</span></span> | <span data-ttu-id="9625a-130">**x5t** (X.509 证书 SHA-1 指纹) 参数是 base64url 编码的 SHA-1 指纹 (。k.a。</span><span class="sxs-lookup"><span data-stu-id="9625a-130">The **x5t** (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="9625a-131">摘要) X.509 证书 [RFC 5280](https://tools.ietf.org/html/rfc5280)的 DER 编码。</span><span class="sxs-lookup"><span data-stu-id="9625a-131">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="9625a-132">e</span><span class="sxs-lookup"><span data-stu-id="9625a-132">e</span></span> | <span data-ttu-id="9625a-133">string</span><span class="sxs-lookup"><span data-stu-id="9625a-133">string</span></span> | <span data-ttu-id="9625a-134">RSA 密钥 - 公共指数</span><span class="sxs-lookup"><span data-stu-id="9625a-134">RSA Key - public exponent</span></span> |
| <span data-ttu-id="9625a-135">d</span><span class="sxs-lookup"><span data-stu-id="9625a-135">d</span></span>| <span data-ttu-id="9625a-136">string</span><span class="sxs-lookup"><span data-stu-id="9625a-136">string</span></span> | <span data-ttu-id="9625a-137">RSA 密钥 - 专用指数。</span><span class="sxs-lookup"><span data-stu-id="9625a-137">RSA Key - private exponent.</span></span> <span data-ttu-id="9625a-138">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="9625a-138">Field cannot be read back.</span></span> |
| <span data-ttu-id="9625a-139">n</span><span class="sxs-lookup"><span data-stu-id="9625a-139">n</span></span> | <span data-ttu-id="9625a-140">string</span><span class="sxs-lookup"><span data-stu-id="9625a-140">string</span></span> | <span data-ttu-id="9625a-141">RSA 密钥 - 模数</span><span class="sxs-lookup"><span data-stu-id="9625a-141">RSA Key - modulus</span></span> |
| <span data-ttu-id="9625a-142">p</span><span class="sxs-lookup"><span data-stu-id="9625a-142">p</span></span> | <span data-ttu-id="9625a-143">string</span><span class="sxs-lookup"><span data-stu-id="9625a-143">string</span></span> | <span data-ttu-id="9625a-144">RSA 密钥 - 第一个主密钥。</span><span class="sxs-lookup"><span data-stu-id="9625a-144">RSA Key - first prime.</span></span> <span data-ttu-id="9625a-145">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="9625a-145">Field cannot be read back.</span></span> |
| <span data-ttu-id="9625a-146">q</span><span class="sxs-lookup"><span data-stu-id="9625a-146">q</span></span> | <span data-ttu-id="9625a-147">字符串</span><span class="sxs-lookup"><span data-stu-id="9625a-147">string</span></span> | <span data-ttu-id="9625a-148">RSA 密钥 - 第二级。</span><span class="sxs-lookup"><span data-stu-id="9625a-148">RSA Key - second prime.</span></span> <span data-ttu-id="9625a-149">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="9625a-149">Field cannot be read back.</span></span> |
| <span data-ttu-id="9625a-150">dp</span><span class="sxs-lookup"><span data-stu-id="9625a-150">dp</span></span> | <span data-ttu-id="9625a-151">string</span><span class="sxs-lookup"><span data-stu-id="9625a-151">string</span></span> | <span data-ttu-id="9625a-152">RSA 密钥 - 第一个指数。</span><span class="sxs-lookup"><span data-stu-id="9625a-152">RSA Key - first exponent.</span></span> <span data-ttu-id="9625a-153">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="9625a-153">Field cannot be read back.</span></span> |
| <span data-ttu-id="9625a-154">dq</span><span class="sxs-lookup"><span data-stu-id="9625a-154">dq</span></span> | <span data-ttu-id="9625a-155">string</span><span class="sxs-lookup"><span data-stu-id="9625a-155">string</span></span> | <span data-ttu-id="9625a-156">RSA 密钥 - 第二个指数。</span><span class="sxs-lookup"><span data-stu-id="9625a-156">RSA Key - second exponent.</span></span> <span data-ttu-id="9625a-157">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="9625a-157">Field cannot be read back.</span></span> |
| <span data-ttu-id="9625a-158">一些</span><span class="sxs-lookup"><span data-stu-id="9625a-158">qi</span></span> | <span data-ttu-id="9625a-159">string</span><span class="sxs-lookup"><span data-stu-id="9625a-159">string</span></span> | <span data-ttu-id="9625a-160">RSA 密钥 - 系数。</span><span class="sxs-lookup"><span data-stu-id="9625a-160">RSA Key - Coefficient.</span></span> <span data-ttu-id="9625a-161">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="9625a-161">Field cannot be read back.</span></span> |
| <span data-ttu-id="9625a-162">k</span><span class="sxs-lookup"><span data-stu-id="9625a-162">k</span></span> | <span data-ttu-id="9625a-163">string</span><span class="sxs-lookup"><span data-stu-id="9625a-163">string</span></span> | <span data-ttu-id="9625a-164">八进制密钥类型的对称密钥。</span><span class="sxs-lookup"><span data-stu-id="9625a-164">Symmetric Key for oct key type.</span></span> <span data-ttu-id="9625a-165">无法重新读取字段。</span><span class="sxs-lookup"><span data-stu-id="9625a-165">Field cannot be read back.</span></span>   |
| <span data-ttu-id="9625a-166">nbf</span><span class="sxs-lookup"><span data-stu-id="9625a-166">nbf</span></span> | <span data-ttu-id="9625a-167">int</span><span class="sxs-lookup"><span data-stu-id="9625a-167">int</span></span> | <span data-ttu-id="9625a-168">此值是 RFC 7519 (中定义的 NumericDate 一个 JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跃点秒）的秒数。) </span><span class="sxs-lookup"><span data-stu-id="9625a-168">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="9625a-169">exp</span><span class="sxs-lookup"><span data-stu-id="9625a-169">exp</span></span> | <span data-ttu-id="9625a-170">int</span><span class="sxs-lookup"><span data-stu-id="9625a-170">int</span></span> | <span data-ttu-id="9625a-171">此值是 RFC 7519 (中定义的 NumericDate 一个 JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跃点秒）的秒数。) </span><span class="sxs-lookup"><span data-stu-id="9625a-171">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="9625a-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9625a-172">JSON representation</span></span>

<span data-ttu-id="9625a-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9625a-173">The following is a JSON representation of the resource.</span></span>

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


