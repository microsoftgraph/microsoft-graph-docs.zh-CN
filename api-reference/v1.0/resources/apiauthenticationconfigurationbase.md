---
title: apiAuthenticationConfigurationBase 资源类型
description: 表示用于调用 API 的身份验证配置的基本类型。
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3e3086ac90eabc15527a84f9c215659def06b7ea
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094476"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a>apiAuthenticationConfigurationBase 资源类型

命名空间：microsoft.graph

用于保存用于调用 API 的身份验证信息的基类型。

派生类型包括：
- 用于 HTTP 基本身份验证的[basicAuthentication](basicauthentication.md)
- [用于客户端证书身份验证的 pkcs12certificate](pkcs12certificate.md) (API 连接器创建或上载) 
- [clientCertificateAuthentication，](pkcs12certificate.md) 用于 (API 连接器客户端证书的客户端证书的客户端) 

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.apiAuthenticationConfigurationBase"
}
```
