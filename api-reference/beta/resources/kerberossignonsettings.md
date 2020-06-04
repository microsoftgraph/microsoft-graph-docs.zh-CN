---
title: kerberosSignOnSettings 资源类型
description: 表示通过应用程序代理发布的本地应用程序的 kerberos 设置。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b702405e320ba3f687b8cb5a758a7bdb868603b3
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556395"
---
# <a name="kerberossignonsettings-resource-type"></a>kerberosSignOnSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在通过 Azure AD 应用程序代理发布本地应用程序时， [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md)资源的 Keberos 约束委派（KCD）设置。 应用程序代理使用 Kerberos 约束委派（KCD）来支持对集成的 Windows 身份验证应用程序的单点登录。 有关详细信息，请参阅[使用应用程序代理以单点登录到应用的 Kerberos 约束委派](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)。

>[!NOTE]
>请勿使用此属性来配置 SAML 或基于密码的单一登录。 如果要配置 SAML 单一登录，则必须在[servicePrincipal](serviceprincipal.md)上设置此设置。
如果要配置基于密码的单签名，则必须使用[createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)进行设置。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|kerberosServicePrincipalName|String| 应用程序服务器的内部应用程序 SPN。 此 SPN 必须位于连接器可以向其提供委派凭据的服务列表中。 |
|kerberosSignOnMappingAttributeType|String| 代表用户使用的连接器的委派登录标识。 有关详细信息，请参阅使用[不同的内部部署和云标识](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities)。 可取值为：`userPrincipalName`、`onPremisesUserPrincipalName`、`userPrincipalUsername`、`onPremisesUserPrincipalUsername`、`onPremisesSAMAccountName`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.kerberosSignOnSettings",
  "baseType": null
}-->

```json
{
  "KerberosServicePrincipalName": "String",
  "KerberosSignOnMappingAttributeType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "kerberosSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->