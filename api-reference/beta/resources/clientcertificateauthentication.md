---
title: clientCertificateAuthentication 资源类型
description: 表示用于获取 API 调用中的 clientCertificateAuthentication 的配置。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e88a1de011fb975afae49d53b8707b95e16157c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509391"
---
# <a name="clientcertificateauthentication-resource-type"></a>clientCertificateAuthentication 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

派生自 apiAuthenticationConfigurationBase 的类型，用于表示基于 Pkcs12 的客户端证书身份验证。 这用于检索上载的证书的公共属性。

继承自 [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|certificateList| [pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md) 集合| 为此 API 连接器上载的证书列表。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.clientCertificateAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
  "certificateList": "Collection(microsoft.graph.pkcs12CertificateInformation)",
}
```
