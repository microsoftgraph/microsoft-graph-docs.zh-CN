---
title: 更新 serviceprincipal
description: 更新 serviceprincipal 对象的属性。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d10ffe883b316449a0b0fb58d57dd018e4e395ca
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958171"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="7f481-103">更新 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="7f481-103">Update servicePrincipal</span></span>

<span data-ttu-id="7f481-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f481-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7f481-105">更新 [servicePrincipal](../resources/serviceprincipal.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7f481-105">Update the properties of [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7f481-106">不支持使用 PATCH 设置 [**passwordCredential**](../resources/passwordcredential.md)。</span><span class="sxs-lookup"><span data-stu-id="7f481-106">Using PATCH to set [**passwordCredential**](../resources/passwordcredential.md) is not supported.</span></span> <span data-ttu-id="7f481-107">使用 [addPassword](./serviceprincipal-addpassword.md) 和 [removePassword](./serviceprincipal-removepassword.md) 方法更新 servicePrincipal 的密码。</span><span class="sxs-lookup"><span data-stu-id="7f481-107">Use the [addPassword](./serviceprincipal-addpassword.md) and [removePassword](./serviceprincipal-removepassword.md) methods to update the password for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f481-108">权限</span><span class="sxs-lookup"><span data-stu-id="7f481-108">Permissions</span></span>
<span data-ttu-id="7f481-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f481-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f481-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f481-111">Permission type</span></span>      | <span data-ttu-id="7f481-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f481-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f481-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f481-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7f481-114">Application.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f481-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7f481-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f481-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f481-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f481-116">Not supported.</span></span>    |
|<span data-ttu-id="7f481-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f481-117">Application</span></span> | <span data-ttu-id="7f481-118">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f481-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f481-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f481-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7f481-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f481-120">Request headers</span></span>
| <span data-ttu-id="7f481-121">名称</span><span class="sxs-lookup"><span data-stu-id="7f481-121">Name</span></span>       | <span data-ttu-id="7f481-122">说明</span><span class="sxs-lookup"><span data-stu-id="7f481-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="7f481-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f481-123">Authorization</span></span> | <span data-ttu-id="7f481-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f481-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7f481-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f481-126">Content-Type</span></span> | <span data-ttu-id="7f481-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7f481-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f481-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f481-129">Request body</span></span>
<span data-ttu-id="7f481-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7f481-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7f481-133">属性</span><span class="sxs-lookup"><span data-stu-id="7f481-133">Property</span></span>     | <span data-ttu-id="7f481-134">类型</span><span class="sxs-lookup"><span data-stu-id="7f481-134">Type</span></span> |<span data-ttu-id="7f481-135">说明</span><span class="sxs-lookup"><span data-stu-id="7f481-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f481-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="7f481-136">accountEnabled</span></span>|<span data-ttu-id="7f481-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f481-137">Boolean</span></span>| <span data-ttu-id="7f481-138">如果服务主体帐户已启用，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="7f481-138">**true** if the service principal account is enabled; otherwise, **false**.</span></span>|
|<span data-ttu-id="7f481-139">addIns</span><span class="sxs-lookup"><span data-stu-id="7f481-139">addIns</span></span>| [<span data-ttu-id="7f481-140">addIn</span><span class="sxs-lookup"><span data-stu-id="7f481-140">addIn</span></span>](../resources/addin.md) | <span data-ttu-id="7f481-141">定义使用服务可用于调用特定上下文中的应用的自定义行为。</span><span class="sxs-lookup"><span data-stu-id="7f481-141">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="7f481-142">例如，呈现文件流的应用程序可能会为其“FileHandler”功能[设置 addIns 属性](/onedrive/developer/file-handlers/?view=odsp-graph-online)。</span><span class="sxs-lookup"><span data-stu-id="7f481-142">For example, applications that can render file streams [may set the addIns property](/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="7f481-143">这将使 Microsoft 365 之类的服务在用户正在处理的文档上下文中调用应用程序。</span><span class="sxs-lookup"><span data-stu-id="7f481-143">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>|
|<span data-ttu-id="7f481-144">alternativeNames</span><span class="sxs-lookup"><span data-stu-id="7f481-144">alternativeNames</span></span>|<span data-ttu-id="7f481-145">字符串集合</span><span class="sxs-lookup"><span data-stu-id="7f481-145">String collection</span></span>| <span data-ttu-id="7f481-146">用于按订阅、标识资源组和[托管标识](https://aka.ms/azuremanagedidentity)的完整资源 ID 检索服务主体。</span><span class="sxs-lookup"><span data-stu-id="7f481-146">Used to retrieve service principals by subscription, identify resource group and full resource ids for [managed identities](https://aka.ms/azuremanagedidentity).</span></span>|
|<span data-ttu-id="7f481-147">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="7f481-147">appRoleAssignmentRequired</span></span>|<span data-ttu-id="7f481-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f481-148">Boolean</span></span>|<span data-ttu-id="7f481-149">指定在 Azure AD 在向应用程序签发用户或访问令牌之前用户或组是否需要 **appRoleAssignment**。</span><span class="sxs-lookup"><span data-stu-id="7f481-149">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span> <span data-ttu-id="7f481-150">不可为空。</span><span class="sxs-lookup"><span data-stu-id="7f481-150">Not nullable.</span></span> |
|<span data-ttu-id="7f481-151">appRoles</span><span class="sxs-lookup"><span data-stu-id="7f481-151">appRoles</span></span>|<span data-ttu-id="7f481-152">[appRole](../resources/approle.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f481-152">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="7f481-153">关联应用程序公开的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="7f481-153">The application roles exposed by the associated application.</span></span> <span data-ttu-id="7f481-154">有关详细信息，请参阅 [应用程序](../resources/application.md)资源上的 **appRoles** 属性定义。</span><span class="sxs-lookup"><span data-stu-id="7f481-154">For more information see the **appRoles** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="7f481-155">不可为空。</span><span class="sxs-lookup"><span data-stu-id="7f481-155">Not nullable.</span></span> |
|<span data-ttu-id="7f481-156">displayName</span><span class="sxs-lookup"><span data-stu-id="7f481-156">displayName</span></span>|<span data-ttu-id="7f481-157">String</span><span class="sxs-lookup"><span data-stu-id="7f481-157">String</span></span>|<span data-ttu-id="7f481-158">服务主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7f481-158">The display name for the service principal.</span></span>|
|<span data-ttu-id="7f481-159">homepage</span><span class="sxs-lookup"><span data-stu-id="7f481-159">homepage</span></span>|<span data-ttu-id="7f481-160">String</span><span class="sxs-lookup"><span data-stu-id="7f481-160">String</span></span>|<span data-ttu-id="7f481-161">应用程序的主页或登录页面。</span><span class="sxs-lookup"><span data-stu-id="7f481-161">Home page or landing page of the application.</span></span>|
|<span data-ttu-id="7f481-162">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="7f481-162">keyCredentials</span></span>|<span data-ttu-id="7f481-163">[keyCredential](../resources/keycredential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f481-163">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="7f481-164">与服务帐户关联的密钥凭据集合。</span><span class="sxs-lookup"><span data-stu-id="7f481-164">The collection of key credentials associated with the service principal.</span></span> <span data-ttu-id="7f481-165">不可为空。</span><span class="sxs-lookup"><span data-stu-id="7f481-165">Not nullable.</span></span>            |
|<span data-ttu-id="7f481-166">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="7f481-166">logoutUrl</span></span>|<span data-ttu-id="7f481-167">String</span><span class="sxs-lookup"><span data-stu-id="7f481-167">String</span></span>| <span data-ttu-id="7f481-168">指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="7f481-168">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span>|
|<span data-ttu-id="7f481-169">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="7f481-169">oauth2PermissionScopes</span></span>|<span data-ttu-id="7f481-170">[permissionScope](../resources/permissionScope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f481-170">[permissionScope](../resources/permissionScope.md) collection</span></span>|<span data-ttu-id="7f481-171">关联应用程序公开的 OAuth 2.0 权限范围。</span><span class="sxs-lookup"><span data-stu-id="7f481-171">The OAuth 2.0 permission scopes exposed by the associated application.</span></span> <span data-ttu-id="7f481-172">有关详细信息，请参阅 [应用程序](../resources/application.md)资源上的 **oauth2PermissionScopes** 属性定义。</span><span class="sxs-lookup"><span data-stu-id="7f481-172">For more information see the **oauth2PermissionScopes** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="7f481-173">不可为空。</span><span class="sxs-lookup"><span data-stu-id="7f481-173">Not nullable.</span></span>|
|<span data-ttu-id="7f481-174">preferredSingleSignOnMode</span><span class="sxs-lookup"><span data-stu-id="7f481-174">preferredSingleSignOnMode</span></span>|<span data-ttu-id="7f481-175">string</span><span class="sxs-lookup"><span data-stu-id="7f481-175">string</span></span>|<span data-ttu-id="7f481-176">指定为此应用程序配置的单一登录模式。</span><span class="sxs-lookup"><span data-stu-id="7f481-176">Specifies the single sign-on mode configured for this application.</span></span> <span data-ttu-id="7f481-177">Azure AD 使用首选单一登录模式从 Microsoft 365 或Azure AD My Apps 启动应用程序。</span><span class="sxs-lookup"><span data-stu-id="7f481-177">Azure AD uses the preferred single sign-on mode to launch the application from Microsoft 365 or the Azure AD My Apps.</span></span> <span data-ttu-id="7f481-178">支持的值是：`password`、`saml`、`external` 和 `oidc`。</span><span class="sxs-lookup"><span data-stu-id="7f481-178">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|
|<span data-ttu-id="7f481-179">replyUrls</span><span class="sxs-lookup"><span data-stu-id="7f481-179">replyUrls</span></span>|<span data-ttu-id="7f481-180">String 集合</span><span class="sxs-lookup"><span data-stu-id="7f481-180">String collection</span></span>|<span data-ttu-id="7f481-181">向其发送用户令牌以使用关联应用程序登录的 URL，或者为关联应用程序向其发送 OAuth 2.0 authorization 代码和访问令牌的重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="7f481-181">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span> <span data-ttu-id="7f481-182">不可为空。</span><span class="sxs-lookup"><span data-stu-id="7f481-182">Not nullable.</span></span> |
|<span data-ttu-id="7f481-183">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="7f481-183">servicePrincipalNames</span></span>|<span data-ttu-id="7f481-184">字符串集合</span><span class="sxs-lookup"><span data-stu-id="7f481-184">String collection</span></span>|<span data-ttu-id="7f481-185">包含从关联的 [应用程序](../resources/application.md)中复制的 **identifiersUris** 列表。</span><span class="sxs-lookup"><span data-stu-id="7f481-185">Contains the list of **identifiersUris**, copied over from the associated [application](../resources/application.md).</span></span> <span data-ttu-id="7f481-186">可以将其他值添加到混合应用程序。</span><span class="sxs-lookup"><span data-stu-id="7f481-186">Additional values can be added to hybrid applications.</span></span> <span data-ttu-id="7f481-187">这些值可用于标识此应用程序在 Azure AD 中公开的权限。</span><span class="sxs-lookup"><span data-stu-id="7f481-187">These values can be used to identify the permissions exposed by this app within Azure AD.</span></span> <span data-ttu-id="7f481-188">例如，</span><span class="sxs-lookup"><span data-stu-id="7f481-188">For example,</span></span><ul><li><span data-ttu-id="7f481-189">请求对此资源的权限的客户端应用可以使用这些 URI 在其应用程序清单的 **requiredResourceAccess** 属性中或在应用注册体验的“API 权限”边栏选项卡中指定所需的权限。</span><span class="sxs-lookup"><span data-stu-id="7f481-189">Client apps requesting permissions to this resource can use these URIs to specify needed permissions in the **requiredResourceAccess** property of their application manifest, or in the "API permissions" blade on the App registrations experience.</span></span></li><li><span data-ttu-id="7f481-190">客户端应用可以指定基于此属性的值的资源 URI（即“aud”声明中返回的 URI），以获取访问令牌。</span><span class="sxs-lookup"><span data-stu-id="7f481-190">Client apps can specify a resource URI which is based on the values of this property to acquire an access token, which is the URI returned in the “aud” claim.</span></span></li></ul><br><span data-ttu-id="7f481-191">需要多值属性筛选器表达式的 any 运算符。</span><span class="sxs-lookup"><span data-stu-id="7f481-191">The any operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="7f481-192">不可为空。</span><span class="sxs-lookup"><span data-stu-id="7f481-192">Not nullable.</span></span>|
|<span data-ttu-id="7f481-193">标记</span><span class="sxs-lookup"><span data-stu-id="7f481-193">tags</span></span>|<span data-ttu-id="7f481-194">String 集合</span><span class="sxs-lookup"><span data-stu-id="7f481-194">String collection</span></span>| <span data-ttu-id="7f481-195">可用于分类和标识应用程序的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="7f481-195">Custom strings that can be used to categorize and identify the application.</span></span> <span data-ttu-id="7f481-196">不可为空。</span><span class="sxs-lookup"><span data-stu-id="7f481-196">Not nullable.</span></span> |
| <span data-ttu-id="7f481-197">tokenEncryptionKeyId</span><span class="sxs-lookup"><span data-stu-id="7f481-197">tokenEncryptionKeyId</span></span> |<span data-ttu-id="7f481-198">String</span><span class="sxs-lookup"><span data-stu-id="7f481-198">String</span></span>|<span data-ttu-id="7f481-199">指定 keyCredentials 集合中的公共密钥的 keyId。</span><span class="sxs-lookup"><span data-stu-id="7f481-199">Specifies the keyId of a public key from the keyCredentials collection.</span></span> <span data-ttu-id="7f481-200">配置后，Azure AD 为此应用程序发布使用此属性指定的密钥加密的令牌。</span><span class="sxs-lookup"><span data-stu-id="7f481-200">When configured, Azure AD issues tokens for this application encrypted using the key specified by this property.</span></span> <span data-ttu-id="7f481-201">接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。</span><span class="sxs-lookup"><span data-stu-id="7f481-201">The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.</span></span>|

## <a name="response"></a><span data-ttu-id="7f481-202">响应</span><span class="sxs-lookup"><span data-stu-id="7f481-202">Response</span></span>

<span data-ttu-id="7f481-203">如果成功，此方法将在响应正文中返回 `204 No Content` 响应代码和更新的 [servicePrincipal](../resources/serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f481-203">If successful, this method returns a `204 No Content` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f481-204">示例</span><span class="sxs-lookup"><span data-stu-id="7f481-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f481-205">请求</span><span class="sxs-lookup"><span data-stu-id="7f481-205">Request</span></span>
<span data-ttu-id="7f481-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f481-206">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7f481-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f481-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "appRoleAssignmentRequired": true
}
```
# <a name="c"></a>[<span data-ttu-id="7f481-208">C#</span><span class="sxs-lookup"><span data-stu-id="7f481-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f481-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f481-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f481-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f481-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f481-211">Java</span><span class="sxs-lookup"><span data-stu-id="7f481-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7f481-212">响应</span><span class="sxs-lookup"><span data-stu-id="7f481-212">Response</span></span>
<span data-ttu-id="7f481-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f481-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

