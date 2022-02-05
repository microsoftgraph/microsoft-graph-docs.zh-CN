---
title: x509CertificateAuthenticationModeConfiguration 资源类型
description: 定义 X.509 证书的强身份验证配置。 此配置包括默认身份验证模式和强身份验证绑定的不同规则。
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="x509certificateauthenticationmodeconfiguration-resource-type"></a>x509CertificateAuthenticationModeConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义 X.509 证书的强身份验证配置。 此配置包括默认身份验证模式和强身份验证绑定的不同规则。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|规则|[x509CertificateRule](../resources/x509certificaterule.md) 集合| 除了身份验证模式之外，还配置了规则，以将特定的 **x509CertificateRuleType** 绑定到 **x509CertificateAuthenticationMode**。 例如，将 with `policyOID` 标识符绑定到`1.32.132.343``x509CertificateMultiFactor`身份验证模式。|
|x509CertificateAuthenticationDefaultMode|x509CertificateAuthenticationMode| 强身份验证模式的类型。 可能的值包括 `x509CertificateSingleFactor`、`x509CertificateMultiFactor`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.x509CertificateAuthenticationModeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateAuthenticationModeConfiguration",
  "x509CertificateAuthenticationDefaultMode": "String",
  "rules": [
    {
      "@odata.type": "microsoft.graph.x509CertificateRule"
    }
  ]
}
```

