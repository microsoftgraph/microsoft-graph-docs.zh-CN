---
title: clientCertificateAuthentication 资源类型
description: 表示用于检索 clientCertificateAuthentication 的配置。
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 70a3885d313f368c71ab1dc2f10c158a726ffde9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109267"
---
# <a name="clientcertificateauthentication-resource-type"></a>clientCertificateAuthentication 资源类型

命名空间：microsoft.graph

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
