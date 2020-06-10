---
title: onPremisesPublishing 资源类型
description: 表示应用程序代理 onPremisesPublishing 对象。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4d19a726e2f09c1df994bc8aee7d91eb53ef2628
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682003"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="07694-103">onPremisesPublishing 资源类型</span><span class="sxs-lookup"><span data-stu-id="07694-103">onPremisesPublishing resource type</span></span>

<span data-ttu-id="07694-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07694-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07694-105">通过[AZURE AD 应用程序代理](https://aka.ms/whyappproxy)发布的本地应用程序由[application](application.md)对象及其关联的**onPremisesPublishing**属性表示。</span><span class="sxs-lookup"><span data-stu-id="07694-105">An on-premises application published via [Azure AD Application Proxy](https://aka.ms/whyappproxy) is represented by an [application](application.md) object and its associated **onPremisesPublishing** property.</span></span> <span data-ttu-id="07694-106">应用程序代理提供对本地应用程序的安全远程访问。</span><span class="sxs-lookup"><span data-stu-id="07694-106">Application Proxy provides secure remote access to on-premises applications.</span></span>

<span data-ttu-id="07694-107">一个**onPremisesPublishing**对象，表示用于为本地[应用程序](application.md)配置应用程序代理的一组属性。</span><span class="sxs-lookup"><span data-stu-id="07694-107">An **onPremisesPublishing** object represents the set of properties for configuring Application Proxy for an on-premises [application](application.md).</span></span> 

<span data-ttu-id="07694-108">在[实例化自定义应用程序](../api/applicationtemplate-instantiate.md)或[创建应用程序](../api/application-post-applications.md)后，可以通过[更新应用程序的](../api/application-update.md)onPremisesPublishing 属性来配置该应用程序的应用程序代理设置。</span><span class="sxs-lookup"><span data-stu-id="07694-108">After [instantiating a custom application](../api/applicationtemplate-instantiate.md) or [creating an application](../api/application-post-applications.md), the Application Proxy settings for the application can be configured by [updating the application's](../api/application-update.md) onPremisesPublishing properties.</span></span>

## <a name="properties"></a><span data-ttu-id="07694-109">属性</span><span class="sxs-lookup"><span data-stu-id="07694-109">Properties</span></span>

| <span data-ttu-id="07694-110">属性</span><span class="sxs-lookup"><span data-stu-id="07694-110">Property</span></span>|<span data-ttu-id="07694-111">类型</span><span class="sxs-lookup"><span data-stu-id="07694-111">Type</span></span>|<span data-ttu-id="07694-112">Description</span><span class="sxs-lookup"><span data-stu-id="07694-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07694-113">alternateUrl</span><span class="sxs-lookup"><span data-stu-id="07694-113">alternateUrl</span></span>|<span data-ttu-id="07694-114">String</span><span class="sxs-lookup"><span data-stu-id="07694-114">String</span></span>| <span data-ttu-id="07694-115">如果要在多个应用程序代理应用程序的前面配置流量管理器，则 alternateUrl 是将指向流量管理器的用户友好 URL。</span><span class="sxs-lookup"><span data-stu-id="07694-115">If you are configuring a traffic manager in front of multiple App Proxy applications, the alternateUrl is the user-friendly URL that will point to the traffic manager.</span></span> |
|<span data-ttu-id="07694-116">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="07694-116">applicationServerTimeout</span></span>|<span data-ttu-id="07694-117">String</span><span class="sxs-lookup"><span data-stu-id="07694-117">String</span></span>| <span data-ttu-id="07694-118">在关闭连接之前，连接器将等待后端应用程序响应的持续时间。</span><span class="sxs-lookup"><span data-stu-id="07694-118">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="07694-119">可能的值 `default` 为 `long` 。</span><span class="sxs-lookup"><span data-stu-id="07694-119">Possible values are `default`, `long`.</span></span> <span data-ttu-id="07694-120">如果设置为 "默认"，后端应用程序超时的长度为85秒。</span><span class="sxs-lookup"><span data-stu-id="07694-120">When set to default, the backend application timeout has a length of 85 seconds.</span></span> <span data-ttu-id="07694-121">当设置为 "长" 时，后端超时将增加到180秒。</span><span class="sxs-lookup"><span data-stu-id="07694-121">When set to long, the backend timeout is increased to 180 seconds.</span></span> <span data-ttu-id="07694-122">`long`如果服务器要响应请求的时间超过85秒，或者如果您无法访问应用程序，并且错误状态为 "后端超时"，则使用。</span><span class="sxs-lookup"><span data-stu-id="07694-122">Use `long` if your server takes more than 85 seconds to respond to requests or if you are unable to access the application and the error status is "Backend Timeout".</span></span> <span data-ttu-id="07694-123">默认值为 `default`。</span><span class="sxs-lookup"><span data-stu-id="07694-123">Default value is `default`.</span></span> |
|<span data-ttu-id="07694-124">applicationType</span><span class="sxs-lookup"><span data-stu-id="07694-124">applicationType</span></span>|<span data-ttu-id="07694-125">String</span><span class="sxs-lookup"><span data-stu-id="07694-125">String</span></span>| <span data-ttu-id="07694-126">指示此应用程序是否为应用程序代理配置的应用程序。</span><span class="sxs-lookup"><span data-stu-id="07694-126">Indicates if this application is an Application Proxy configured application.</span></span> <span data-ttu-id="07694-127">这是由系统预设置的。</span><span class="sxs-lookup"><span data-stu-id="07694-127">This is pre-set by the system.</span></span> <span data-ttu-id="07694-128">只读。</span><span class="sxs-lookup"><span data-stu-id="07694-128">Read-only.</span></span> |
|<span data-ttu-id="07694-129">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="07694-129">externalAuthenticationType</span></span>|<span data-ttu-id="07694-130">String</span><span class="sxs-lookup"><span data-stu-id="07694-130">String</span></span>| <span data-ttu-id="07694-131">详细介绍了应用程序的预身份验证设置。</span><span class="sxs-lookup"><span data-stu-id="07694-131">Details the pre-authentication setting for the application.</span></span> <span data-ttu-id="07694-132">预身份验证强制用户必须先进行身份验证，然后才能访问应用程序。</span><span class="sxs-lookup"><span data-stu-id="07694-132">Pre-authentication enforces that users must authenticate before accessing the app.</span></span> <span data-ttu-id="07694-133">Passthru 不需要身份验证。</span><span class="sxs-lookup"><span data-stu-id="07694-133">Passthru does not require authentication.</span></span> <span data-ttu-id="07694-134">可取值为：`passthru`、`aadPreAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="07694-134">Possible values are: `passthru`, `aadPreAuthentication`.</span></span> |
|<span data-ttu-id="07694-135">externalUrl</span><span class="sxs-lookup"><span data-stu-id="07694-135">externalUrl</span></span>|<span data-ttu-id="07694-136">String</span><span class="sxs-lookup"><span data-stu-id="07694-136">String</span></span>| <span data-ttu-id="07694-137">应用程序的已发布外部 url。</span><span class="sxs-lookup"><span data-stu-id="07694-137">The published external url for the application.</span></span> <span data-ttu-id="07694-138">例如，https://intranet-contoso.msappproxy.net/。</span><span class="sxs-lookup"><span data-stu-id="07694-138">For example, https://intranet-contoso.msappproxy.net/.</span></span>  |
|<span data-ttu-id="07694-139">internalUrl</span><span class="sxs-lookup"><span data-stu-id="07694-139">internalUrl</span></span>|<span data-ttu-id="07694-140">String</span><span class="sxs-lookup"><span data-stu-id="07694-140">String</span></span>| <span data-ttu-id="07694-141">应用程序的内部 url。</span><span class="sxs-lookup"><span data-stu-id="07694-141">The internal url of the application.</span></span> <span data-ttu-id="07694-142">例如，https://intranet/。</span><span class="sxs-lookup"><span data-stu-id="07694-142">For example, https://intranet/.</span></span> |
|<span data-ttu-id="07694-143">isHttpOnlyCookieEnabled</span><span class="sxs-lookup"><span data-stu-id="07694-143">isHttpOnlyCookieEnabled</span></span>|<span data-ttu-id="07694-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="07694-144">Boolean</span></span>| <span data-ttu-id="07694-145">指示是否应在 HTTP 响应标头中设置 HTTPOnly cookie 标志。</span><span class="sxs-lookup"><span data-stu-id="07694-145">Indicates if the HTTPOnly cookie flag should be set in the HTTP response headers.</span></span> <span data-ttu-id="07694-146">将此值设置为 `true` ，让应用程序代理 cookie 在 HTTP 响应标头中包含 HTTPOnly 标志。</span><span class="sxs-lookup"><span data-stu-id="07694-146">Set this value to `true` to have Application Proxy cookies include the HTTPOnly flag in the HTTP response headers.</span></span> <span data-ttu-id="07694-147">如果使用远程桌面服务，则将此值设置为 False。</span><span class="sxs-lookup"><span data-stu-id="07694-147">If using Remote Desktop Services, set this value to False.</span></span> <span data-ttu-id="07694-148">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="07694-148">Default value is `false`.</span></span> |
|<span data-ttu-id="07694-149">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="07694-149">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="07694-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="07694-150">Boolean</span></span>| <span data-ttu-id="07694-151">指示是否当前正在通过应用程序代理发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="07694-151">Indicates if the application is currently being published via Application Proxy or not.</span></span> <span data-ttu-id="07694-152">这是由系统预设置的。</span><span class="sxs-lookup"><span data-stu-id="07694-152">This is pre-set by the system.</span></span> <span data-ttu-id="07694-153">只读。</span><span class="sxs-lookup"><span data-stu-id="07694-153">Read-only.</span></span> |
|<span data-ttu-id="07694-154">isPersistentCookieEnabled</span><span class="sxs-lookup"><span data-stu-id="07694-154">isPersistentCookieEnabled</span></span>|<span data-ttu-id="07694-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="07694-155">Boolean</span></span>| <span data-ttu-id="07694-156">指示是否应在 HTTP 响应头中设置永久 cookie 标志。</span><span class="sxs-lookup"><span data-stu-id="07694-156">Indicates if the Persistent cookie flag should be set in the HTTP response headers.</span></span> <span data-ttu-id="07694-157">将此值设置为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="07694-157">Keep this value set to `false`.</span></span> <span data-ttu-id="07694-158">仅对无法在进程之间共享 cookie 的应用程序使用此设置。</span><span class="sxs-lookup"><span data-stu-id="07694-158">Only use this setting for applications that can't share cookies between processes.</span></span> <span data-ttu-id="07694-159">有关 cookie 设置的详细信息，请参阅[用于访问 Azure Active Directory 中的本地应用程序的 cookie 设置](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)。</span><span class="sxs-lookup"><span data-stu-id="07694-159">For more information about cookie settings, see [Cookie settings for accessing on-premises applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings).</span></span> <span data-ttu-id="07694-160">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="07694-160">Default value is `false`.</span></span> |
|<span data-ttu-id="07694-161">isSecureCookieEnabled</span><span class="sxs-lookup"><span data-stu-id="07694-161">isSecureCookieEnabled</span></span>|<span data-ttu-id="07694-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="07694-162">Boolean</span></span>| <span data-ttu-id="07694-163">指示是否应在 HTTP 响应头中设置安全 cookie 标志。</span><span class="sxs-lookup"><span data-stu-id="07694-163">Indicates if the Secure cookie flag should be set in the HTTP response headers.</span></span> <span data-ttu-id="07694-164">将此值设置为 `true` 通过安全通道（如加密的 HTTPS 请求）传输 cookie。</span><span class="sxs-lookup"><span data-stu-id="07694-164">Set this value to `true` to transmit cookies over a secure channel such as an encrypted HTTPS request.</span></span> <span data-ttu-id="07694-165">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="07694-165">Default value is `true`.</span></span>|
|<span data-ttu-id="07694-166">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="07694-166">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="07694-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="07694-167">Boolean</span></span>| <span data-ttu-id="07694-168">指示应用程序是否应转换响应标头中的 url。</span><span class="sxs-lookup"><span data-stu-id="07694-168">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="07694-169">将此值保留为， `true` 除非您的应用程序需要身份验证请求中的原始主机标头。</span><span class="sxs-lookup"><span data-stu-id="07694-169">Keep this value as `true` unless your application required the original host header in the authentication request.</span></span> <span data-ttu-id="07694-170">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="07694-170">Default value is `true`.</span></span>|
|<span data-ttu-id="07694-171">isTranslateLinksInBodyEnabled</span><span class="sxs-lookup"><span data-stu-id="07694-171">isTranslateLinksInBodyEnabled</span></span>|<span data-ttu-id="07694-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="07694-172">Boolean</span></span>| <span data-ttu-id="07694-173">指示应用程序是否应转换应用程序正文中的 url。</span><span class="sxs-lookup"><span data-stu-id="07694-173">Indicates if the application should translate urls in the application body.</span></span> <span data-ttu-id="07694-174">将此值保留为， `false` 除非您有硬编码的 HTML 链接到其他本地应用程序，并且不使用自定义域。</span><span class="sxs-lookup"><span data-stu-id="07694-174">Keep this value as `false` unless you have hardcoded HTML links to other on-premises applications and don't use custom domains.</span></span> <span data-ttu-id="07694-175">有关详细信息，请参阅[链接转换 With Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation)。</span><span class="sxs-lookup"><span data-stu-id="07694-175">For more information, see [Link translation with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation).</span></span> <span data-ttu-id="07694-176">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="07694-176">Default value is `false`.</span></span>|
|<span data-ttu-id="07694-177">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="07694-177">singleSignOnSettings</span></span>|[<span data-ttu-id="07694-178">onPremisesPublishingSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="07694-178">onPremisesPublishingSingleSignOn</span></span>](onpremisespublishingsinglesignon.md)| <span data-ttu-id="07694-179">表示内部部署应用程序的单一登录配置。</span><span class="sxs-lookup"><span data-stu-id="07694-179">Represents the single sign-on configuration for the on-premises application.</span></span> |
|<span data-ttu-id="07694-180">verifiedCustomDomainCertificatesMetadata</span><span class="sxs-lookup"><span data-stu-id="07694-180">verifiedCustomDomainCertificatesMetadata</span></span>|[<span data-ttu-id="07694-181">verifiedCustomDomainCertificatesMetadata</span><span class="sxs-lookup"><span data-stu-id="07694-181">verifiedCustomDomainCertificatesMetadata</span></span>](verifiedcustomdomaincertificatesmetadata.md)| <span data-ttu-id="07694-182">使用自定义域时与应用程序关联的证书的详细信息。</span><span class="sxs-lookup"><span data-stu-id="07694-182">Details of the certificate associated with the application when a custom domain is in use.</span></span> <span data-ttu-id="07694-183">`null`使用默认域时。</span><span class="sxs-lookup"><span data-stu-id="07694-183">`null` when using the default domain.</span></span> <span data-ttu-id="07694-184">只读。</span><span class="sxs-lookup"><span data-stu-id="07694-184">Read-only.</span></span>|
|<span data-ttu-id="07694-185">verifiedCustomDomainKeyCredential</span><span class="sxs-lookup"><span data-stu-id="07694-185">verifiedCustomDomainKeyCredential</span></span>|[<span data-ttu-id="07694-186">keyCredential</span><span class="sxs-lookup"><span data-stu-id="07694-186">keyCredential</span></span>](keycredential.md)| <span data-ttu-id="07694-187">使用的自定义域的关联密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="07694-187">The associated key credential for the custom domain used.</span></span> |
|<span data-ttu-id="07694-188">verifiedCustomDomainPasswordCredential</span><span class="sxs-lookup"><span data-stu-id="07694-188">verifiedCustomDomainPasswordCredential</span></span>|[<span data-ttu-id="07694-189">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="07694-189">passwordCredential</span></span>](passwordcredential.md)| <span data-ttu-id="07694-190">使用的自定义域的关联密码凭据。</span><span class="sxs-lookup"><span data-stu-id="07694-190">The associated password credential for the custom domain used.</span></span> |



## <a name="json-representation"></a><span data-ttu-id="07694-191">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07694-191">JSON representation</span></span>

<span data-ttu-id="07694-192">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07694-192">Here is a JSON representation of the resource.</span></span>

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
