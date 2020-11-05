---
title: onPremisesPublishing 资源类型
description: 表示应用程序代理 onPremisesPublishing 对象。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bda657d3579fab5419852df4ce9a79961aafc89d
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921513"
---
# <a name="onpremisespublishing-resource-type"></a>onPremisesPublishing 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过 [AZURE AD 应用程序代理](https://aka.ms/whyappproxy) 发布的本地应用程序由 [application](application.md) 对象及其关联的 **onPremisesPublishing** 属性表示。 应用程序代理提供对本地应用程序的安全远程访问。

一个 **onPremisesPublishing** 对象，表示用于为本地 [应用程序](application.md)配置应用程序代理的一组属性。 

在 [实例化自定义应用程序](../api/applicationtemplate-instantiate.md) 或 [创建应用程序](../api/application-post-applications.md)后，可以通过 [更新应用程序的](../api/application-update.md) onPremisesPublishing 属性来配置该应用程序的应用程序代理设置。

有关配置应用程序代理的教程，请参阅 [使用 Microsoft GRAPH API 自动化应用程序代理的配置](/graph/application-proxy-configure-api)。

## <a name="properties"></a>属性

| 属性|类型|说明|
|:---------------|:--------|:----------|
|alternateUrl|String| 如果要在多个应用程序代理应用程序的前面配置流量管理器，则 alternateUrl 是将指向流量管理器的用户友好 URL。 |
|applicationServerTimeout|String| 在关闭连接之前，连接器将等待后端应用程序响应的持续时间。 可能的值 `default` 为 `long` 。 如果设置为 "默认"，后端应用程序超时的长度为85秒。 当设置为 "长" 时，后端超时将增加到180秒。 `long`如果服务器要响应请求的时间超过85秒，或者如果您无法访问应用程序，并且错误状态为 "后端超时"，则使用。 默认值为 `default`。 |
|applicationType|String| 指示此应用程序是否为应用程序代理配置的应用程序。 这是由系统预设置的。 只读。 |
|externalAuthenticationType|String| 详细介绍了应用程序的预身份验证设置。 预身份验证强制用户必须先进行身份验证，然后才能访问应用程序。 Passthru 不需要身份验证。 可取值为：`passthru`、`aadPreAuthentication`。 |
|externalUrl|String| 应用程序的已发布外部 url。 例如，https://intranet-contoso.msappproxy.net/。  |
|internalUrl|String| 应用程序的内部 url。 例如，https://intranet/。 |
|isHttpOnlyCookieEnabled|Boolean| 指示是否应在 HTTP 响应标头中设置 HTTPOnly cookie 标志。 将此值设置为 `true` ，让应用程序代理 cookie 在 HTTP 响应标头中包含 HTTPOnly 标志。 如果使用远程桌面服务，则将此值设置为 False。 默认值为 `false`。 |
|isOnPremPublishingEnabled|Boolean| 指示是否当前正在通过应用程序代理发布应用程序。 这是由系统预设置的。 只读。 |
|isPersistentCookieEnabled|Boolean| 指示是否应在 HTTP 响应头中设置永久 cookie 标志。 将此值设置为 `false` 。 仅对无法在进程之间共享 cookie 的应用程序使用此设置。 有关 cookie 设置的详细信息，请参阅 [用于访问 Azure Active Directory 中的本地应用程序的 cookie 设置](/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)。 默认值为 `false`。 |
|isSecureCookieEnabled|Boolean| 指示是否应在 HTTP 响应头中设置安全 cookie 标志。 将此值设置为 `true` 通过安全通道（如加密的 HTTPS 请求）传输 cookie。 默认值为 `true`。|
|isTranslateHostHeaderEnabled|Boolean| 指示应用程序是否应转换响应标头中的 url。 将此值保留为， `true` 除非您的应用程序需要身份验证请求中的原始主机标头。 默认值为 `true`。|
|isTranslateLinksInBodyEnabled|Boolean| 指示应用程序是否应转换应用程序正文中的 url。 将此值保留为， `false` 除非您有硬编码的 HTML 链接到其他本地应用程序，并且不使用自定义域。 有关详细信息，请参阅 [链接转换 With Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation)。 默认值为 `false`。|
|singleSignOnSettings|[onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md)| 表示内部部署应用程序的单一登录配置。 |
|verifiedCustomDomainCertificatesMetadata|[verifiedCustomDomainCertificatesMetadata](verifiedcustomdomaincertificatesmetadata.md)| 使用自定义域时与应用程序关联的证书的详细信息。 `null` 使用默认域时。 只读。|
|verifiedCustomDomainKeyCredential|[keyCredential](keycredential.md)| 使用的自定义域的关联密钥凭据。 |
|verifiedCustomDomainPasswordCredential|[passwordCredential](passwordcredential.md)| 使用的自定义域的关联密码凭据。 |



## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "alternateUrl": "String",
  "applicationServerTimeout": "String",
  "applicationType": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isHttpOnlyCookieEnabled": true,
  "isOnPremPublishingEnabled": true,
  "isPersistentCookieEnabled": true,
  "isSecureCookieEnabled": true,
  "isTranslateHostHeaderEnabled": true,
  "isTranslateLinksInBodyEnabled": true,
  "singleSignOnSettings": {"@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn"},
  "verifiedCustomDomainCertificatesMetadata": {"@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata"},
  "verifiedCustomDomainKeyCredential": {"@odata.type": "microsoft.graph.keyCredential"},
  "verifiedCustomDomainPasswordCredential": {"@odata.type": "microsoft.graph.passwordCredential"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2019-02-04 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


