---
title: 更新 serviceprincipal
description: 更新 serviceprincipal 对象的属性。
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ade4dd91e9469f56d6c4d498005888c0f59f5da1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969274"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="5208e-103">更新 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="5208e-103">Update servicePrincipal</span></span>

<span data-ttu-id="5208e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5208e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5208e-105">更新 [servicePrincipal](../resources/serviceprincipal.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5208e-105">Update the properties of [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5208e-p101">Using PATCH to set [**passwordCredential**](../resources/passwordcredential.md) is not supported. Use the [addPassword](./serviceprincipal-addpassword.md) and [removePassword](./serviceprincipal-removepassword.md) methods to update the password for a servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="5208e-p101">Using PATCH to set [**passwordCredential**](../resources/passwordcredential.md) is not supported. Use the [addPassword](./serviceprincipal-addpassword.md) and [removePassword](./serviceprincipal-removepassword.md) methods to update the password for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="5208e-108">权限</span><span class="sxs-lookup"><span data-stu-id="5208e-108">Permissions</span></span>
<span data-ttu-id="5208e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5208e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5208e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5208e-111">Permission type</span></span>      | <span data-ttu-id="5208e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5208e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5208e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5208e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5208e-114">Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5208e-114">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5208e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5208e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5208e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5208e-116">Not supported.</span></span>    |
|<span data-ttu-id="5208e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5208e-117">Application</span></span> | <span data-ttu-id="5208e-118">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5208e-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5208e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5208e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5208e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5208e-120">Request headers</span></span>
| <span data-ttu-id="5208e-121">名称</span><span class="sxs-lookup"><span data-stu-id="5208e-121">Name</span></span>       | <span data-ttu-id="5208e-122">说明</span><span class="sxs-lookup"><span data-stu-id="5208e-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5208e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5208e-123">Authorization</span></span> | <span data-ttu-id="5208e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5208e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5208e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5208e-126">Content-Type</span></span> | <span data-ttu-id="5208e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5208e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5208e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5208e-129">Request body</span></span>
<span data-ttu-id="5208e-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5208e-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5208e-133">属性</span><span class="sxs-lookup"><span data-stu-id="5208e-133">Property</span></span>     | <span data-ttu-id="5208e-134">类型</span><span class="sxs-lookup"><span data-stu-id="5208e-134">Type</span></span> |<span data-ttu-id="5208e-135">说明</span><span class="sxs-lookup"><span data-stu-id="5208e-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5208e-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="5208e-136">accountEnabled</span></span>|<span data-ttu-id="5208e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="5208e-137">Boolean</span></span>| <span data-ttu-id="5208e-138">如果服务主体帐户已启用，则为 **true** ；否则，为 **false** 。</span><span class="sxs-lookup"><span data-stu-id="5208e-138">**true** if the service principal account is enabled; otherwise, **false**.</span></span>|
| <span data-ttu-id="5208e-139">addIns</span><span class="sxs-lookup"><span data-stu-id="5208e-139">addIns</span></span> | [<span data-ttu-id="5208e-140">addIn</span><span class="sxs-lookup"><span data-stu-id="5208e-140">addIn</span></span>](../resources/addin.md) | <span data-ttu-id="5208e-p106">Defines custom behavior that a consuming service can use to call an app in specific contexts. For example, applications that can render file streams [may set the addIns property](/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality. This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span><span class="sxs-lookup"><span data-stu-id="5208e-p106">Defines custom behavior that a consuming service can use to call an app in specific contexts. For example, applications that can render file streams [may set the addIns property](/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality. This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>|
|<span data-ttu-id="5208e-144">alternativeNames</span><span class="sxs-lookup"><span data-stu-id="5208e-144">alternativeNames</span></span>|<span data-ttu-id="5208e-145">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5208e-145">String collection</span></span>| <span data-ttu-id="5208e-146">用于按订阅、标识资源组和[托管标识](https://aka.ms/azuremanagedidentity)的完整资源 ID 检索服务主体。</span><span class="sxs-lookup"><span data-stu-id="5208e-146">Used to retrieve service principals by subscription, identify resource group and full resource ids for [managed identities](https://aka.ms/azuremanagedidentity).</span></span>|
|<span data-ttu-id="5208e-147">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="5208e-147">appRoleAssignmentRequired</span></span>|<span data-ttu-id="5208e-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="5208e-148">Boolean</span></span>|<span data-ttu-id="5208e-p107">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application. Not nullable.</span><span class="sxs-lookup"><span data-stu-id="5208e-p107">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application. Not nullable.</span></span> |
|<span data-ttu-id="5208e-151">appRoles</span><span class="sxs-lookup"><span data-stu-id="5208e-151">appRoles</span></span>|<span data-ttu-id="5208e-152">[appRole](../resources/approle.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5208e-152">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="5208e-p108">The application roles exposed by the associated application. For more information see the **appRoles** property definition on the [application](../resources/application.md) resource. Not nullable.</span><span class="sxs-lookup"><span data-stu-id="5208e-p108">The application roles exposed by the associated application. For more information see the **appRoles** property definition on the [application](../resources/application.md) resource. Not nullable.</span></span> |
|<span data-ttu-id="5208e-156">displayName</span><span class="sxs-lookup"><span data-stu-id="5208e-156">displayName</span></span>|<span data-ttu-id="5208e-157">String</span><span class="sxs-lookup"><span data-stu-id="5208e-157">String</span></span>|<span data-ttu-id="5208e-158">服务主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5208e-158">The display name for the service principal.</span></span>|
|<span data-ttu-id="5208e-159">homepage</span><span class="sxs-lookup"><span data-stu-id="5208e-159">homepage</span></span>|<span data-ttu-id="5208e-160">String</span><span class="sxs-lookup"><span data-stu-id="5208e-160">String</span></span>|<span data-ttu-id="5208e-161">应用程序的主页或登录页面。</span><span class="sxs-lookup"><span data-stu-id="5208e-161">Home page or landing page of the application.</span></span>|
|<span data-ttu-id="5208e-162">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="5208e-162">keyCredentials</span></span>|<span data-ttu-id="5208e-163">[keyCredential](../resources/keycredential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5208e-163">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="5208e-p109">与服务帐户关联的密码凭据集合。不可为空。</span><span class="sxs-lookup"><span data-stu-id="5208e-p109">The collection of key credentials associated with the service principal. Not nullable.</span></span>            |
|<span data-ttu-id="5208e-166">loginUrl</span><span class="sxs-lookup"><span data-stu-id="5208e-166">loginUrl</span></span>|<span data-ttu-id="5208e-167">String</span><span class="sxs-lookup"><span data-stu-id="5208e-167">String</span></span>|<span data-ttu-id="5208e-168">指定服务提供商将用户重定向到 Azure AD 进行身份验证的 URL。</span><span class="sxs-lookup"><span data-stu-id="5208e-168">Specifies the URL where the service provider redirects the user to Azure AD to authenticate.</span></span> <span data-ttu-id="5208e-169">Azure AD 使用 URL 从 Microsoft 365 或Azure AD My Apps 启动应用程序。</span><span class="sxs-lookup"><span data-stu-id="5208e-169">Azure AD uses the URL to launch the application from Microsoft 365 or the Azure AD My Apps.</span></span> <span data-ttu-id="5208e-170">该选项为空时，Azure AD 将对使用“[基于 SAML 的单一登录](/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso)”配置的应用程序执行 IdP 启动的登录。</span><span class="sxs-lookup"><span data-stu-id="5208e-170">When blank, Azure AD performs IdP-initiated sign-on for applications configured with [SAML-based single sign-on](/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso).</span></span> <span data-ttu-id="5208e-171">用户从 Microsoft 365、Azure AD My Apps 或Azure AD SSO URL 启动应用程序。</span><span class="sxs-lookup"><span data-stu-id="5208e-171">The user launches the application from Microsoft 365, the Azure AD My Apps, or the Azure AD SSO URL.</span></span>|
|<span data-ttu-id="5208e-172">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="5208e-172">logoutUrl</span></span>|<span data-ttu-id="5208e-173">String</span><span class="sxs-lookup"><span data-stu-id="5208e-173">String</span></span>| <span data-ttu-id="5208e-174">指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="5208e-174">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span>|
|<span data-ttu-id="5208e-175">notificationEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="5208e-175">notificationEmailAddresses</span></span>|<span data-ttu-id="5208e-176">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5208e-176">String collection</span></span>|<span data-ttu-id="5208e-177">指定在活动证书临近到期日期时，Azure AD 在其中发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="5208e-177">Specifies the list of email addresses where Azure AD sends a notification when the active certificate is near the expiration date.</span></span> <span data-ttu-id="5208e-178">这仅适用于用于签署为 Azure AD 库应用程序发行的 SAML 令牌的证书。</span><span class="sxs-lookup"><span data-stu-id="5208e-178">This is only for the certificates used to sign the SAML token issued for Azure AD Gallery applications.</span></span>|
|<span data-ttu-id="5208e-179">publishedPermissionScopes</span><span class="sxs-lookup"><span data-stu-id="5208e-179">publishedPermissionScopes</span></span>|<span data-ttu-id="5208e-180">[permissionScope](../resources/permissionScope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5208e-180">[permissionScope](../resources/permissionScope.md) collection</span></span>|<span data-ttu-id="5208e-181">关联应用程序的 OAuth 2.0 权限。</span><span class="sxs-lookup"><span data-stu-id="5208e-181">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="5208e-182">有关详细信息，请参阅 [应用程序](../resources/application.md)资源上的 **oauth2PermissionScopes** 属性定义。</span><span class="sxs-lookup"><span data-stu-id="5208e-182">For more information see the **oauth2PermissionScopes** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="5208e-183">不可为空。</span><span class="sxs-lookup"><span data-stu-id="5208e-183">Not nullable.</span></span>            |
|<span data-ttu-id="5208e-184">preferredSingleSignOnMode</span><span class="sxs-lookup"><span data-stu-id="5208e-184">preferredSingleSignOnMode</span></span>|<span data-ttu-id="5208e-185">string</span><span class="sxs-lookup"><span data-stu-id="5208e-185">string</span></span>|<span data-ttu-id="5208e-186">指定为此应用程序配置的单一登录模式。</span><span class="sxs-lookup"><span data-stu-id="5208e-186">Specifies the single sign-on mode configured for this application.</span></span> <span data-ttu-id="5208e-187">Azure AD 使用首选单一登录模式从 Microsoft 365 或Azure AD My Apps 启动应用程序。</span><span class="sxs-lookup"><span data-stu-id="5208e-187">Azure AD uses the preferred single sign-on mode to launch the application from Microsoft 365 or the Azure AD My Apps.</span></span> <span data-ttu-id="5208e-188">支持的值有 password、saml、external 和 oidc。</span><span class="sxs-lookup"><span data-stu-id="5208e-188">The supported values are password, saml, external, and oidc.</span></span>|
|<span data-ttu-id="5208e-189">preferredTokenSigningKeyEndDateTime</span><span class="sxs-lookup"><span data-stu-id="5208e-189">preferredTokenSigningKeyEndDateTime</span></span>|<span data-ttu-id="5208e-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5208e-190">DateTimeOffset</span></span>|<span data-ttu-id="5208e-191">指定用于令牌签名的 keyCredential 的到期日期，由 **preferredTokenSigningKeyThumbprint** 标记。</span><span class="sxs-lookup"><span data-stu-id="5208e-191">Specifies the expiration date of the keyCredential used for token signing, marked by **preferredTokenSigningKeyThumbprint**.</span></span>|
|<span data-ttu-id="5208e-192">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="5208e-192">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="5208e-193">String</span><span class="sxs-lookup"><span data-stu-id="5208e-193">String</span></span>|<span data-ttu-id="5208e-194">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="5208e-194">Reserved for internal use only.</span></span> <span data-ttu-id="5208e-195">请勿写入属性，否则将依赖该属性。</span><span class="sxs-lookup"><span data-stu-id="5208e-195">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="5208e-196">可能会在未来版本中删除。</span><span class="sxs-lookup"><span data-stu-id="5208e-196">May be removed in future versions.</span></span> |
|<span data-ttu-id="5208e-197">publisherName</span><span class="sxs-lookup"><span data-stu-id="5208e-197">publisherName</span></span>|<span data-ttu-id="5208e-198">String</span><span class="sxs-lookup"><span data-stu-id="5208e-198">String</span></span>|<span data-ttu-id="5208e-199">在其中指定关联应用程序的租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5208e-199">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="5208e-200">replyUrls</span><span class="sxs-lookup"><span data-stu-id="5208e-200">replyUrls</span></span>|<span data-ttu-id="5208e-201">String 集合</span><span class="sxs-lookup"><span data-stu-id="5208e-201">String collection</span></span>|<span data-ttu-id="5208e-202">向其发送用户令牌以使用关联应用程序登录的 URL，或者为关联应用程序向其发送 OAuth 2.0 authorization 代码和访问令牌的重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="5208e-202">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span> <span data-ttu-id="5208e-203">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="5208e-203">Not nullable.</span></span> |
|<span data-ttu-id="5208e-204">samlSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="5208e-204">samlSingleSignOnSettings</span></span>|[<span data-ttu-id="5208e-205">samlSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="5208e-205">samlSingleSignOnSettings</span></span>](../resources/samlsinglesignonsettings.md)|<span data-ttu-id="5208e-206">有关 saml 单一登录的设置的集合。</span><span class="sxs-lookup"><span data-stu-id="5208e-206">The collection for settings related to saml single sign-on.</span></span>|
|<span data-ttu-id="5208e-207">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="5208e-207">servicePrincipalNames</span></span>|<span data-ttu-id="5208e-208">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5208e-208">String collection</span></span>|<span data-ttu-id="5208e-209">包含从关联的 [应用程序](../resources/application.md)中复制的 **identifiersUris** 列表。</span><span class="sxs-lookup"><span data-stu-id="5208e-209">Contains the list of **identifiersUris** , copied over from the associated [application](../resources/application.md).</span></span> <span data-ttu-id="5208e-210">可以将其他值添加到混合应用程序。</span><span class="sxs-lookup"><span data-stu-id="5208e-210">Additional values can be added to hybrid applications.</span></span> <span data-ttu-id="5208e-211">这些值可用于标识此应用程序在 Azure AD 中公开的权限。</span><span class="sxs-lookup"><span data-stu-id="5208e-211">These values can be used to identify the permissions exposed by this app within Azure AD.</span></span> <span data-ttu-id="5208e-212">例如，</span><span class="sxs-lookup"><span data-stu-id="5208e-212">For example,</span></span><ul><li><span data-ttu-id="5208e-213">请求对此资源的权限的客户端应用可以使用这些 URI 在其应用程序清单的 **requiredResourceAccess** 属性中或在应用注册体验的“API 权限”边栏选项卡中指定所需的权限。</span><span class="sxs-lookup"><span data-stu-id="5208e-213">Client apps requesting permissions to this resource can use these URIs to specify needed permissions in the **requiredResourceAccess** property of their application manifest, or in the "API permissions" blade on the App registrations experience.</span></span></li><li><span data-ttu-id="5208e-214">客户端应用可以指定基于此属性的值的资源 URI（即“aud”声明中返回的 URI），以获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="5208e-214">Client apps can specify a resource URI which is based on the values of this property to acquire an access token, which is the URI returned in the “aud” claim.</span></span></li></ul><br><span data-ttu-id="5208e-215">需要多值属性筛选器表达式的 any 运算符。</span><span class="sxs-lookup"><span data-stu-id="5208e-215">The any operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="5208e-216">不可为空。</span><span class="sxs-lookup"><span data-stu-id="5208e-216">Not nullable.</span></span>|
|<span data-ttu-id="5208e-217">标记</span><span class="sxs-lookup"><span data-stu-id="5208e-217">tags</span></span>|<span data-ttu-id="5208e-218">String 集合</span><span class="sxs-lookup"><span data-stu-id="5208e-218">String collection</span></span>| <span data-ttu-id="5208e-219">不可为空。</span><span class="sxs-lookup"><span data-stu-id="5208e-219">Not nullable.</span></span> |
|<span data-ttu-id="5208e-220">tokenEncryptionKeyId</span><span class="sxs-lookup"><span data-stu-id="5208e-220">tokenEncryptionKeyId</span></span>|<span data-ttu-id="5208e-221">字符串</span><span class="sxs-lookup"><span data-stu-id="5208e-221">String</span></span>|<span data-ttu-id="5208e-222">指定 keyCredentials 集合中的公共密钥的 keyId。</span><span class="sxs-lookup"><span data-stu-id="5208e-222">Specifies the keyId of a public key from the keyCredentials collection.</span></span> <span data-ttu-id="5208e-223">配置后，Azure AD 为此应用程序发布使用此属性指定的密钥加密的令牌。</span><span class="sxs-lookup"><span data-stu-id="5208e-223">When configured, Azure AD issues tokens for this application encrypted using the key specified by this property.</span></span> <span data-ttu-id="5208e-224">接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。</span><span class="sxs-lookup"><span data-stu-id="5208e-224">The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.</span></span>|

## <a name="response"></a><span data-ttu-id="5208e-225">响应</span><span class="sxs-lookup"><span data-stu-id="5208e-225">Response</span></span>

<span data-ttu-id="5208e-226">如果成功，此方法在响应正文中返回 `204 No Content` 响应代码和更新的 [servicePrincipal](../resources/serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5208e-226">If successful, this method returns a `204 No Content` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="5208e-227">示例</span><span class="sxs-lookup"><span data-stu-id="5208e-227">Examples</span></span>
### <a name="request"></a><span data-ttu-id="5208e-228">请求</span><span class="sxs-lookup"><span data-stu-id="5208e-228">Request</span></span>
<span data-ttu-id="5208e-229">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5208e-229">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5208e-230">HTTP</span><span class="sxs-lookup"><span data-stu-id="5208e-230">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->

```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "appRoleAssignmentRequired": true
}
```
# <a name="c"></a>[<span data-ttu-id="5208e-231">C#</span><span class="sxs-lookup"><span data-stu-id="5208e-231">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5208e-232">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5208e-232">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5208e-233">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5208e-233">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5208e-234">Java</span><span class="sxs-lookup"><span data-stu-id="5208e-234">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5208e-235">响应</span><span class="sxs-lookup"><span data-stu-id="5208e-235">Response</span></span>
<span data-ttu-id="5208e-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5208e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


