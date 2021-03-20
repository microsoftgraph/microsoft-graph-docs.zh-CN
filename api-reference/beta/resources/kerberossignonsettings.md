---
title: kerberosSignOnSettings 资源类型
description: 表示通过应用程序代理发布的本地应用程序的 kerberos 设置。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: af00e70e1ef4603c1b1370ec5ef9e9ba75fecb4c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943658"
---
# <a name="kerberossignonsettings-resource-type"></a>kerberosSignOnSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过 Azure AD 应用程序代理发布本地应用程序时，代表 [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) 资源的 Keberos 约束委派 (KCD) 设置。 应用程序代理使用 Kerberos 约束 (KCD) 支持对集成 Windows 身份验证应用程序进行单一登录。 有关详细信息，请参阅 [Kerberos 约束委派，以使用应用程序代理单一登录应用](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)。

>[!NOTE]
>请勿使用此属性配置 SAML 或基于密码的单一登录。 如果要配置 SAML 单一登录，则必须在[servicePrincipal 上设置。](serviceprincipal.md)
如果要配置基于密码的单一签名，必须使用 [createPasswordSingleSignOnCredentials 进行设置](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|kerberosServicePrincipalName|String| 应用程序服务器的内部应用程序 SPN。 此 SPN 需在连接器可以呈现委派凭据的服务列表中。 |
|kerberosSignOnMappingAttributeType|kerberosSignOnMappingAttributeType| 代表用户使用的连接器的委派登录标识。 有关详细信息，请参阅使用不同的本地 [和云标识 ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities)。 可取值为：`userPrincipalName`、`onPremisesUserPrincipalName`、`userPrincipalUsername`、`onPremisesUserPrincipalUsername`、`onPremisesSAMAccountName`。|

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
  "kerberosServicePrincipalName": "String",
  "kerberosSignOnMappingAttributeType": "String"
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
