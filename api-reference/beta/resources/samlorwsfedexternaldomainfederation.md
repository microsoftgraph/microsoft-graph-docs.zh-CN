---
title: samlOrWsFedExternalDomainFederation 资源类型
description: 表示使用 Azure AD 租户的 azure AD Azure Active Directory (设置的 SAML/WS-fed) 联合
author: namkedia
localization_priority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aee7550d2a8a098fa841056637cfc73aed5aca03
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697043"
---
# <a name="samlorwsfedexternaldomainfederation-resource-type"></a>samlOrWsFedExternalDomainFederation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

允许 Azure AD) 租户Azure Active Directory (其标识提供程序 (IdP) 支持 SAML 或 WS-Fed 协议的另一个组织建立联盟的资源。 这使 Azure AD 租户允许来宾用户访问其资源。 有关 SAML/WS-Fed IdP 联盟的信息，请参阅 [联合身份验证与来宾用户的 SAML/WS-Fed 标识提供程序](/azure/active-directory/external-identities/direct-federation)。

继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 samlOrWsFedExternalDomainFederations](../api/samlorwsfedexternaldomainfederation-list.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 集合|获取 [samlOrWsFedExternalDomainFederation 对象](../resources/samlorwsfedexternaldomainfederation.md) 及其属性的列表。|
|[创建 samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-post.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|创建新的 [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 对象。|
|[获取 samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-get.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|读取 [samlOrWsFedExternalDomainFederation 对象的属性和](../resources/samlorwsfedexternaldomainfederation.md) 关系。|
|[更新 samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-update.md)|[samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md)|更新 [samlOrWsFedExternalDomainFederation 对象](../resources/samlorwsfedexternaldomainfederation.md) 的属性。|
|[删除 samlOrWsFedExternalDomainFederation](../api/samlorwsfedexternaldomainfederation-delete.md)|None|删除 [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 对象。|
|[列出域](../api/samlorwsfedexternaldomainfederation-list-domains.md)|[externalDomainName](../resources/externaldomainname.md) 集合|从域导航属性获取 externalDomainName 资源。|
|[创建 externalDomainName](../api/samlorwsfedexternaldomainfederation-post-domains.md)|[externalDomainName](../resources/externaldomainname.md)|创建新的 externalDomainName 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|基于显示名称 IdP 的 SAML WS-Fed IdP。 继承自 [identityProviderBase](../resources/identityproviderbase.md)。|
|id|String|标识提供程序的标识符。 继承自 [实体](../resources/entity.md)。|
|issuerUri|String|联合服务器的颁发者 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|metadataExchangeUri|String|用于从富客户端应用程序进行身份验证的元数据交换终结点的 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|passiveSignInUri|String|登录 Azure AD 服务时基于 Web 的客户端定向到的 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|preferredAuthenticationProtocol|String|首选身份验证协议。 支持的值包括 `saml` 或 `wsfed` 。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|signingCertificate|String|用于对传递到令牌的令牌进行签名的当前Microsoft 标识平台。 证书的格式设置为联合 IdP 令牌签名证书的公共部分的 Base64 编码字符串，并且必须与 X509Certificate2 类兼容。  <br/><br/> 此属性用于以下方案： <ul><li> 如果在自动注册更新之外需要滚动 <li>正在设置新的联合身份验证服务 <li> 如果更新联合身份验证服务证书后，联合身份验证属性中不存在新的令牌签名证书。 </ul> <br/><br/> Azure AD 通过自动注册过程更新证书，其中它尝试从联合身份验证服务元数据检索新证书，即当前证书到期前 30 天。 如果新证书不可用，Azure AD 将每天监视元数据，并且将在新证书可用时更新域的联盟设置。 <br/><br/> 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|domains|[externalDomainName](../resources/externaldomainname.md) 集合|与租户联盟的外部组织的域名集合。 支持 `$filter`（`eq`）。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.samlOrWsFedExternalDomainFederation",
  "baseType": "microsoft.graph.samlOrWsFedProvider",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.samlOrWsFedExternalDomainFederation",
  "id": "String (identifier)",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String"
}
```
