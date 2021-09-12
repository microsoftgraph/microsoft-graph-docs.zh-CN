---
title: pkcs12Certificate 资源类型
description: 表示用于上载 pkcs12Certificate 的配置。
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2e86cd05fa2ee1b1646e7e402b738f90fd8ccaba
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59006947"
---
# <a name="pkcs12certificate-resource-type"></a>pkcs12Certificate 资源类型

命名空间：microsoft.graph

表示使用 HTTPS 客户端证书身份验证调用 API 连接器终结点时用于上载证书的配置。 客户端证书身份验证是基于相互证书的身份验证，其中客户端向 API 终结点提供客户端证书以证明其身份。 Azure AD 将 API 连接器的配置证书发送到给定的 API 终结点，然后验证该证书。

继承自 [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|pkcs12Value|String| 表示发送的 pfx 内容。 该值应为实际证书内容的 Base64 编码版本。 必需。|
|密码|String| pfx 文件的密码。 必填。 如果未使用密码，则仍必须提供 的值 `""` 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12Certificate"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.pkcs12Certificate",
  "pkcs12Value": "String",
  "password": "String"
}
```
