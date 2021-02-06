---
title: kerberosSignOnSettings 资源类型
description: 表示通过应用程序代理发布的本地应用程序的单一登录设置。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 85b2b4963c077b8dcb6ded4818ecc57bce635b39
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134867"
---
# <a name="onpremisespublishingsinglesignon-resource-type"></a>onPremisesPublishingSingleSignOn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示使用 Azure AD 应用程序代理发布本地应用程序时 [onPremisesPublishing](onpremisespublishing.md) 资源的单一登录设置。 此资源用于将集成 Windows 身份验证和基于标头的身份验证设置为单一登录模式。 有关详细信息，请参阅 [Kerberos 约束委派](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)，以使用应用程序代理单一登录应用。

>[!NOTE]
>请勿使用此属性配置 SAML 或基于密码的单一登录。 如果要配置 SAML 单一登录，则必须在[servicePrincipal 上设置。](serviceprincipal.md)
如果要配置基于密码的单一签名，则必须使用 [createPasswordSingleSignOnCredentials 进行设置](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|kerberosSignOnSettings| [kerberosSignOnSettings](kerberossignonsettings.md)| 使用集成窗口身份验证的应用程序的 Kerberos 约束委派设置。 |
|singleSignOnMode|字符串| 应用程序的首选单一登录模式。 可取值为：`none`、`onPremisesKerberos`、`headerBased`。|

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
  "kerberosSignOnSettings": {"@odata.type": "microsoft.graph.kerberosSignOnSettings"},
  "singleSignOnMode": "String"
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
