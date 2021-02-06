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
# <a name="trustframeworkkey-resource-type"></a>trustFrameworkKey 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 JWK (JSON Web 密钥) 。 TrustFrameworkKey 是表示加密密钥的 JSON 数据结构。 此资源的结构遵循 [RFC 7517 第 4 节中定义的格式](https://tools.ietf.org/html/rfc7517#section-4)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| 一些 | string | 密钥的唯一标识符。   |
| kty | string | "kty" (类型) 参数标识用于密钥的加密算法系列，有效值为 rsa、oct。 |
| use | string | "use" (使用) 参数标识公钥的预定用途。  "use"参数用于指示公钥是否用于加密数据或验证数据上的签名。 可能的值是 1。 "sig" (2) 签名。  "enc" (加密)    |
| x5c | string 集合 | "x5c" (X.509 证书链) 参数包含一个或多个 PKIX 证书 [RFC 5280 的链](https://tools.ietf.org/html/rfc5280)。 |
| x5t | string | "x5t" (X.509 证书 SHA-1 指纹) 参数是 base64url 编码的 SHA-1 指纹 (a.k.a。 摘要) X.509 证书 [RFC 5280](https://tools.ietf.org/html/rfc5280)的 DER 编码。 |
| e | string | RSA 密钥 - 公共指数 |
| d| string | RSA 密钥 - 私有指数。 无法重新读取字段。 |
| n | string | RSA 密钥 - 模数 |
| p | string | RSA 密钥 - 第一个主密钥。 无法重新读取字段。 |
| q | 字符串 | RSA 密钥 - 第二级。 无法重新读取字段。 |
| dp | string | RSA 密钥 - 第一个指数。 无法重新读取字段。 |
| dq | string | RSA 密钥 - 第二个指数。 无法重新读取字段。 |
| 一些 | string | RSA 键 - 系数。 无法重新读取字段。 |
| k | string | 八进制密钥类型的对称密钥。 无法重新读取字段。   |
| nbf | int | 此值是 RFC 7519 (中定义的 NumericDate。JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跨越秒数）的秒数。)  |
| exp | int | 此值是 RFC 7519 (中定义的 NumericDate。JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跨越秒数）的秒数。)  |



## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

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


