---
title: samlOrWsFedProvider 资源类型
description: 用于设置基于 SAML 或基于WS-Fed提供程序的配置详细信息。
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9dbe48d7d2c229132dfea4b84282cadcdbcc8d7c
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697047"
---
# <a name="samlorwsfedprovider-resource-type"></a>samlOrWsFedProvider 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供配置详细信息的抽象类型，用于通过 IdP WS-Fed基于外部域的标识提供程序 (SAML) 。

继承自 [identityProviderBase](../resources/identityproviderbase.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|基于显示名称 SAML/WS-Fed 的标识提供程序的名称。 继承自 [identityProviderBase](../resources/identityproviderbase.md)。|
|id|String|标识提供程序的标识符。 继承自 [实体](../resources/entity.md)。|
|issuerUri|String|联合服务器的颁发者 URI。|
|metadataExchangeUri|String|用于从富客户端应用程序进行身份验证的元数据交换终结点的 URI。|
|passiveSignInUri|String|登录 Azure AD 服务时基于 Web 的客户端Azure Active Directory (定向) URI。|
|metadataExchangeUri|String|用于从富客户端应用程序进行身份验证的元数据交换终结点的 URI。|
|passiveSignInUri|String|登录 Azure AD 服务时基于 Web 的客户端定向到的 URI。|
|preferredAuthenticationProtocol|String|首选身份验证协议。 支持的值包括 `saml` 或 `wsfed` 。|
|signingCertificate|String|用于对传递到令牌的令牌进行签名的当前Microsoft 标识平台。 证书的格式设置为联合 IdP 令牌签名证书的公共部分的 Base64 编码字符串，并且必须与 X509Certificate2 类兼容。  <br/><br/> 此属性用于以下方案： <ul><li> 如果在自动注册更新之外需要滚动 <li>正在设置新的联合身份验证服务 <li> 如果更新联合身份验证服务证书后联合身份验证属性中不存在新的令牌签名证书。 </ul> <br/><br/> Azure AD 通过自动注册过程更新证书，其中它尝试从联合身份验证服务元数据检索新证书，即当前证书到期前 30 天。 如果新证书不可用，Azure AD 将每天监视元数据，并且将在新证书可用时更新域的联盟设置。|

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
