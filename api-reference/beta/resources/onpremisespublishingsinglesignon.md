---
title: kerberosSignOnSettings 资源类型
description: 表示通过应用程序代理发布的本地应用程序的单一登录设置。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f07fc81fee6fdc8e8ff3b55c246facdc4f155d11
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556392"
---
# <a name="onpremisespublishingsinglesignon-resource-type"></a>onPremisesPublishingSingleSignOn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在使用 Azure AD 应用程序代理发布本地应用程序时， [onPremisesPublishing](onpremisespublishing.md)资源的单一登录设置。 此资源用于将集成的 Windows 身份验证和基于标头的身份验证设置为单一登录模式。 有关详细信息，请参阅[使用应用程序代理以单点登录到应用的 Kerberos 约束委派](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)。

>[!NOTE]
>请勿使用此属性来配置 SAML 或基于密码的单一登录。 如果要配置 SAML 单一登录，则必须在[servicePrincipal](serviceprincipal.md)上设置此设置。
如果要配置基于密码的单签名，则必须使用[createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)进行设置。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|kerberosSignOnSettings| [kerberosSignOnSettings](kerberossignonsettings.md)| 应用程序的 Kerberos 约束委派设置。 |
|singleSignOnMode|String| 应用程序的首选单一登录模式。 可取值为：`none`、`onPremisesKerberos`、`headerBased`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn",
  "baseType": null
}-->

```json
{
  "KerberosSignOnSettings": {"@odata.type": "microsoft.graph.kerberosSignOnSettings"},
  "SingleSignOnMode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingSingleSignOn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->