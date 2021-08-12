---
title: apiAuthenticationConfigurationBase 资源类型
description: 表示用于调用 API 的身份验证配置的基本类型。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c897bc970fc4527a03593a72e1ea760ab78fc696a75180e0e718a81ab90455ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54150043"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a>apiAuthenticationConfigurationBase 资源类型

命名空间：microsoft.graph

用于保存用于调用 API 的身份验证信息的基类型。

派生类型包括：
- 用于 HTTP 基本身份验证的[basicAuthentication](basicauthentication.md)
- [用于客户端证书身份验证的 pkcs12certificate](pkcs12certificate.md) (API 连接器创建或上载) 
- [clientCertificateAuthentication](pkcs12certificate.md) 用于 (API 连接器客户端证书的客户端证书身份验证) 

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
