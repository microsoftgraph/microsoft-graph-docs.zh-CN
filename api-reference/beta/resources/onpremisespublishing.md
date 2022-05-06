---
title: onPremisesPublishing 资源类型
description: 表示 应用程序代理 onPremisesPublishing 对象。
ms.localizationpriority: medium
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 453bf7f0ab0f0d13e5c333375d74518251b3f115
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246788"
---
# <a name="onpremisespublishing-resource-type"></a>onPremisesPublishing 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过 [Azure AD 应用程序代理](/azure/active-directory/app-proxy/what-is-application-proxy)发布的本地应用程序 [由应用程序对象](application.md)及其关联 **的 onPremisesPublishing** 属性表示。 应用程序代理提供对本地应用程序的安全远程访问。

**onPremisesPublishing** 对象表示用于 [为本地应用程序](application.md)配置应用程序代理的属性集。 

[实例化自定义应用程序](../api/applicationtemplate-instantiate.md)或[创建应用程序](../api/application-post-applications.md)后，可以通过[更新应用程序的](../api/application-update.md) onPremisesPublishing 属性来配置应用程序的应用程序代理设置。

有关配置应用程序代理的教程，请参阅[使用 Microsoft 图形 API 自动配置应用程序代理](/graph/application-proxy-configure-api)。

## <a name="properties"></a>属性

| 属性|类型|说明|
|:---------------|:--------|:----------|
|alternateUrl|String| 如果在多个应用代理应用程序前配置流量管理器，则 alternateUrl 是指向流量管理器的用户友好 URL。 |
|applicationServerTimeout|String| 连接器在关闭连接之前，将等待来自后端应用程序的响应的持续时间。 可能的值为 `default`. `long` 设置为默认值时，后端应用程序超时长度为 85 秒。 设置为 long 时，后端超时将增加到 180 秒。 如果服务器响应请求需要超过 85 秒，或者无法访问应用程序，错误状态为“后端超时”，请使用 `long` 。 默认值为 `default`。 |
|applicationType|String| 指示此应用程序是否为应用程序代理配置的应用程序。 这是系统预先设置的。 只读。 |
|externalAuthenticationType|externalAuthenticationType| 详细介绍应用程序的预身份验证设置。 预身份验证强制用户在访问应用之前必须进行身份验证。 Passthru 不需要身份验证。 可取值为：`passthru`、`aadPreAuthentication`。 |
|externalUrl|String| 应用程序的已发布外部 URL。 例如，https://intranet-contoso.msappproxy.net/。  |
|internalUrl|String| 应用程序的内部 URL。 例如，https://intranet/。 |
|isBackendCertificateValidationEnabled|Boolean| 指示是否为应用程序启用后端 SSL 证书验证。 对于所有新应用程序代理应用，默认情况下，该属性将设置为`true`。 对于所有现有应用，该属性将设置为 `false`。 |
|isHttpOnlyCookieEnabled|Boolean| 指示是否应在 HTTP 响应标头中设置 HTTPOnly Cookie 标志。 将此值设置为`true`应用程序代理 Cookie 在 HTTP 响应标头中包含 HTTPOnly 标志。 如果使用远程桌面服务，请将此值设置为 False。 默认值为 `false`。 |
|isOnPremPublishingEnabled|Boolean| 指示应用程序当前是否通过应用程序代理发布。 这是系统预先设置的。 只读。 |
|isPersistentCookieEnabled|Boolean| 指示是否应在 HTTP 响应标头中设置持久性 Cookie 标志。 将此值设置为 `false`. 仅对无法在进程之间共享 Cookie 的应用程序使用此设置。 有关 Cookie 设置的详细信息，请参阅 [Cookie 设置，以便在 Azure Active Directory 中访问本地应用程序](/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)。 默认值为 `false`。 |
|isSecureCookieEnabled|Boolean| 指示是否应在 HTTP 响应标头中设置安全 Cookie 标志。 将此值设置为 `true` 通过安全通道（例如加密的 HTTPS 请求）传输 Cookie。 默认值为 `true`。|
|isStateSessionEnabled|Boolean| 指示是否启用了在客户端使用 OAuth 2.0 授权代码授予流时验证状态参数。 此设置允许管理员指定是否要为其应用启用 CSRF 保护。 |
|isTranslateHostHeaderEnabled|Boolean| 指示应用程序是否应转换响应标头中的 URL。 将此值保留为 `true` 除非应用程序需要身份验证请求中的原始主机标头。 默认值为 `true`。|
|isTranslateLinksInBodyEnabled|Boolean| 指示应用程序是否应在应用程序正文中翻译 URL。 将此值保留为 `false` 除非有指向其他本地应用程序的硬编码 HTML 链接，并且不使用自定义域。 有关详细信息，请参阅[包含应用程序代理的链接翻译](/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation)。 默认值为 `false`。|
|singleSignOnSettings|[onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md)| 表示本地应用程序的单一登录配置。 |
|verifiedCustomDomainCertificatesMetadata|[verifiedCustomDomainCertificatesMetadata](verifiedcustomdomaincertificatesmetadata.md)| 使用自定义域时与应用程序关联的证书的详细信息。 `null` 使用默认域时。 只读。|
|verifiedCustomDomainKeyCredential|[keyCredential](keycredential.md)| 所用自定义域的关联密钥凭据。 |
|verifiedCustomDomainPasswordCredential|[passwordCredential](passwordcredential.md)| 所使用的自定义域的关联密码凭据。 |

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
  "isStateSessionEnabled": true,
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
