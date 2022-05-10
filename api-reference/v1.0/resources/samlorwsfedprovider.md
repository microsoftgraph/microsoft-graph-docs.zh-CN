---
title: samlOrWsFedProvider 资源类型
description: 设置基于 SAML 或基于WS-Fed标识提供者的配置详细信息。
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0dec6cac2cdbe1bbe7f42d0d3580e82148e99ff3
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296605"
---
# <a name="samlorwsfedprovider-resource-type"></a>samlOrWsFedProvider 资源类型

命名空间：microsoft.graph

一种抽象类型，提供设置 SAML 或WS-Fed外部基于域的标识提供者 (IdP) 的配置详细信息。

继承自 [identityProviderBase](../resources/identityproviderbase.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|基于 SAML/WS-Fed 的标识提供者的显示名称。 继承自 [identityProviderBase](../resources/identityproviderbase.md)。|
|id|String|标识提供程序的标识符。 继承自 [entity](../resources/entity.md)。|
|issuerUri|String|联合服务器的颁发者 URI。|
|metadataExchangeUri|String|用于从丰富的客户端应用程序进行身份验证的元数据交换终结点的 URI。|
|metadataExchangeUri|字符串|用于从丰富的客户端应用程序进行身份验证的元数据交换终结点的 URI。|
|passiveSignInUri|字符串|登录到Azure Active Directory (Azure AD) 服务时，基于 Web 的客户端将定向到的 URI。|
|preferredAuthenticationProtocol|authenticationProtocol|首选身份验证协议。 可能的值包括 `wsFed`、`saml`、`unknownFutureValue`。|
|signingCertificate|String|用于对传递给Microsoft 标识平台的令牌进行签名的当前证书。 该证书的格式设置为联合 IdP 令牌签名证书公共部分的 Base64 编码字符串，并且必须与 X509Certificate2 类兼容。  <br/><br/> 此属性在以下方案中使用： <ul><li> 如果自动滚动更新外部需要滚动更新 <li>正在设置新的联合身份验证服务 <li> 如果更新联合身份验证服务证书后，联合身份验证属性中不存在新的令牌签名证书。 </ul> <br/><br/> Azure AD通过自动滚动更新过程更新证书，在此过程中，它会尝试在当前证书过期前 30 天从联合身份验证服务元数据中检索新证书。 如果新证书不可用，Azure AD每天监视元数据，并在有新证书可用时更新域的联合身份验证设置。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.samlOrWsFedProvider",
  "baseType": "microsoft.graph.identityProviderBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.samlOrWsFedProvider",
  "id": "String (identifier)",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String"
}
```
