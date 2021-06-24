---
title: onPremisesPublishing 资源类型
description: 表示应用程序代理 onPremisesPublishing 对象。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: d91eae080f46fd43e5ac9cc8d083681e12da8d12
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108808"
---
# <a name="onpremisespublishing-resource-type"></a>onPremisesPublishing 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过 [Azure AD](https://aka.ms/whyappproxy) 应用程序代理发布的本地应用程序由 [应用程序](application.md) 对象及其关联的 **onPremisesPublishing** 属性表示。 应用程序代理提供对本地应用程序的安全远程访问。

**onPremisesPublishing** 对象表示为本地应用程序配置应用程序代理 [的属性集](application.md)。 

实例[化自定义应用程序或](../api/applicationtemplate-instantiate.md)创建应用程序后，[](../api/application-post-applications.md)可以通过更新应用程序的 onPremisesPublishing 属性来[](../api/application-update.md)配置应用程序的应用程序代理设置。

有关配置应用程序代理的教程，请参阅使用 Microsoft Graph API 自动[配置应用程序代理](/graph/application-proxy-configure-api)。

## <a name="properties"></a>属性

| 属性|类型|说明|
|:---------------|:--------|:----------|
|alternateUrl|字符串| 如果要在多个应用程序代理应用程序前面配置流量管理器，则 alternateUrl 是将指向流量管理器的用户友好 URL。 |
|applicationServerTimeout|字符串| 连接器在关闭连接之前等待后端应用程序响应的持续时间。 可能的值是 `default` `long` 、。 设置为默认值时，后端应用程序超时的长度为 85 秒。 设置为长时，后端超时将增加到 180 秒。 如果服务器响应请求的时间超过 85 秒，或者无法访问应用程序并且错误状态为" `long` 后端超时"，请使用 。 默认值为 `default`。 |
|applicationType|String| 指示此应用程序是否配置了应用程序代理。 这是由系统预先设置的。 只读。 |
|externalAuthenticationType|externalAuthenticationType| 详细说明应用程序的预身份验证设置。 预身份验证强制用户在访问应用之前必须进行身份验证。 Passthru 不需要身份验证。 可取值为：`passthru`、`aadPreAuthentication`。 |
|externalUrl|字符串| 应用程序的已发布外部 URL。 例如，https://intranet-contoso.msappproxy.net/。  |
|internalUrl|字符串| 应用程序的内部 URL。 例如，https://intranet/。 |
|isBackendCertificateValidationEnabled|布尔值| 指示是否对应用程序启用后端 SSL 证书验证。 对于所有新的应用程序代理应用，默认情况下，该属性将设置为 `true` 。 对于所有现有应用，该属性将设置为 `false` 。 |
|isHttpOnlyCookieEnabled|布尔值| 指示 HTTPOnly Cookie 标记是否应在 HTTP 响应标头中设置。 将此值设置为让应用程序代理 Cookie 在 HTTP 响应标头中包括 `true` HTTPOnly 标志。 如果使用远程桌面服务，将此值设置为 False。 默认值为 `false`。 |
|isOnPremPublishingEnabled|布尔值| 指示应用程序当前是否正在通过应用程序代理发布。 这是由系统预先设置的。 只读。 |
|isPersistentCookieEnabled|布尔值| 指示是否应在 HTTP 响应标头中设置永久性 Cookie 标记。 将此值设置为 `false` 。 仅对进程之间无法共享 Cookie 的应用程序使用此设置。 有关 Cookie 设置详细信息，请参阅 Cookie 设置，用于访问 Azure Active Directory 中的[本地应用程序](/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)。 默认值为 `false`。 |
|isSecureCookieEnabled|布尔值| 指示是否应在 HTTP 响应标头中设置安全 Cookie 标记。 将此值设置为通过安全通道（如加密的 HTTPS 请求）传输 `true` Cookie。 默认值为 `true`。|
|isTranslateHostHeaderEnabled|布尔值| 指示应用程序是否应转换响应标头中的 URL。 将此值保留为 ，除非您的应用程序在身份验证请求中需要原始 `true` 主机头。 默认值为 `true`。|
|isTranslateLinksInBodyEnabled|布尔值| 指示应用程序是否应在应用程序正文中翻译 URL。 将此值保留为 ，除非您具有指向其他本地应用程序的硬编码 HTML 链接 `false` ，并且不使用自定义域。 有关详细信息，请参阅使用 [应用程序代理链接翻译](/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation)。 默认值为 `false`。|
|singleSignOnSettings|[onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md)| 表示本地应用程序的单一登录配置。 |
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
  "isBackendCertificationValidationEnabled": true,
  "isHttpOnlyCookieEnabled": true,
  "isOnPremPublishingEnabled": true,
  "isPersistentCookieEnabled": true,
  "isSecureCookieEnabled": true,
  "isTranslateHostHeaderEnabled": true,
  "isTranslateLinksInBodyEnabled": true,
  "singleSignOnSettings": {"@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn"},
  "verifiedCustomDomainCertificatesMetadata": {"@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata"},
  "verifiedCustomDomainKeyCredential": {"@odata.type": "microsoft.graph.keyCredential"},
  "verifiedCustomDomainPasswordCredential": {"@odata.type": "microsoft.graph.passwordCredential"},
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


