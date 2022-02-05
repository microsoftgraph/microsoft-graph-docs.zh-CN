---
title: x509CertificateRule 资源类型
description: 定义 X.509 证书的强身份验证配置规则。 除了身份验证模式之外，还配置了规则。
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="x509certificaterule-resource-type"></a>x509CertificateRule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义 X.509 证书的强身份验证配置规则。 除了身份验证模式之外，还配置了规则。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|标识符|String| X.509 证书的标识符。 必需。|
|x509CertificateAuthenticationMode|x509CertificateAuthenticationMode| 强身份验证模式的类型。 可能的值包括 `x509CertificateSingleFactor`、`x509CertificateMultiFactor`、`unknownFutureValue`。 必需。|
|x509CertificateRuleType|x509CertificateRuleType| X.509 证书模式配置规则的类型。 可能的值包括 `issuerSubject`、`policyOID`、`unknownFutureValue`。 必填。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.x509CertificateRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateRule",
  "x509CertificateRuleType": "String",
  "identifier": "String",
  "x509CertificateAuthenticationMode": "String"
}
```

