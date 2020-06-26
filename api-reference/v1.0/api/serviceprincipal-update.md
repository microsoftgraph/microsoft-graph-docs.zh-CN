---
title: 更新 serviceprincipal
description: 更新 serviceprincipal 对象的属性。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 49f9d1f19b1c77eb2b0b4873e75ec44cb5a43422
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895963"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="3611d-103">更新 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="3611d-103">Update servicePrincipal</span></span>

<span data-ttu-id="3611d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3611d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3611d-105">更新[servicePrincipal](../resources/serviceprincipal.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3611d-105">Update the properties of [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3611d-106">不支持使用修补程序设置[**passwordCredential**](../resources/passwordcredential.md) 。</span><span class="sxs-lookup"><span data-stu-id="3611d-106">Using PATCH to set [**passwordCredential**](../resources/passwordcredential.md) is not supported.</span></span> <span data-ttu-id="3611d-107">使用[addPassword](./serviceprincipal-addpassword.md)和[RemovePassword](./serviceprincipal-removepassword.md)方法更新 servicePrincipal 的密码。</span><span class="sxs-lookup"><span data-stu-id="3611d-107">Use the [addPassword](./serviceprincipal-addpassword.md) and [removePassword](./serviceprincipal-removepassword.md) methods to update the password for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="3611d-108">权限</span><span class="sxs-lookup"><span data-stu-id="3611d-108">Permissions</span></span>
<span data-ttu-id="3611d-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3611d-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3611d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3611d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3611d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3611d-111">Permission type</span></span>      | <span data-ttu-id="3611d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3611d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3611d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3611d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3611d-114">Directory.accessasuser.all 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="3611d-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3611d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3611d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3611d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3611d-116">Not supported.</span></span>    |
|<span data-ttu-id="3611d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3611d-117">Application</span></span> | <span data-ttu-id="3611d-118">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3611d-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3611d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3611d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3611d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3611d-120">Request headers</span></span>
| <span data-ttu-id="3611d-121">名称</span><span class="sxs-lookup"><span data-stu-id="3611d-121">Name</span></span>       | <span data-ttu-id="3611d-122">说明</span><span class="sxs-lookup"><span data-stu-id="3611d-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="3611d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3611d-123">Authorization</span></span> | <span data-ttu-id="3611d-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="3611d-124">Bearer {token}.</span></span> <span data-ttu-id="3611d-125">Required.</span><span class="sxs-lookup"><span data-stu-id="3611d-125">Required.</span></span>  |
| <span data-ttu-id="3611d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3611d-126">Content-Type</span></span> | <span data-ttu-id="3611d-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="3611d-127">application/json.</span></span> <span data-ttu-id="3611d-128">Required.</span><span class="sxs-lookup"><span data-stu-id="3611d-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3611d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3611d-129">Request body</span></span>
<span data-ttu-id="3611d-130">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="3611d-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3611d-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="3611d-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3611d-132">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="3611d-132">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3611d-133">属性</span><span class="sxs-lookup"><span data-stu-id="3611d-133">Property</span></span>     | <span data-ttu-id="3611d-134">类型</span><span class="sxs-lookup"><span data-stu-id="3611d-134">Type</span></span> |<span data-ttu-id="3611d-135">说明</span><span class="sxs-lookup"><span data-stu-id="3611d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3611d-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="3611d-136">accountEnabled</span></span>|<span data-ttu-id="3611d-137">布尔</span><span class="sxs-lookup"><span data-stu-id="3611d-137">Boolean</span></span>| <span data-ttu-id="3611d-138">如果服务主体帐户已启用，则为 **true**；否则，为 **false**。</span><span class="sxs-lookup"><span data-stu-id="3611d-138">**true** if the service principal account is enabled; otherwise, **false**.</span></span>|
|<span data-ttu-id="3611d-139">addIns</span><span class="sxs-lookup"><span data-stu-id="3611d-139">addIns</span></span>| [<span data-ttu-id="3611d-140">addIn</span><span class="sxs-lookup"><span data-stu-id="3611d-140">addIn</span></span>](../resources/addin.md) | <span data-ttu-id="3611d-141">定义使用服务可用于调用特定上下文中的应用的自定义行为。</span><span class="sxs-lookup"><span data-stu-id="3611d-141">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="3611d-142">例如，呈现文件流的应用程序可能会为其“FileHandler”功能[设置 addIns 属性](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online)。</span><span class="sxs-lookup"><span data-stu-id="3611d-142">For example, applications that can render file streams [may set the addIns property](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="3611d-143">这将使 Microsoft 365 等服务能够在用户正在使用的文档的上下文中调用应用程序。</span><span class="sxs-lookup"><span data-stu-id="3611d-143">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>|
|<span data-ttu-id="3611d-144">alternativeNames</span><span class="sxs-lookup"><span data-stu-id="3611d-144">alternativeNames</span></span>|<span data-ttu-id="3611d-145">String collection</span><span class="sxs-lookup"><span data-stu-id="3611d-145">String collection</span></span>| <span data-ttu-id="3611d-146">用于按订阅检索服务主体，标识[托管标识](https://aka.ms/azuremanagedidentity)的资源组和完整资源 id。</span><span class="sxs-lookup"><span data-stu-id="3611d-146">Used to retrieve service principals by subscription, identify resource group and full resource ids for [managed identities](https://aka.ms/azuremanagedidentity).</span></span>|
|<span data-ttu-id="3611d-147">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="3611d-147">appRoleAssignmentRequired</span></span>|<span data-ttu-id="3611d-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="3611d-148">Boolean</span></span>|<span data-ttu-id="3611d-149">指定在 Azure AD 在向应用程序签发用户或访问令牌之前用户或组是否需要 **appRoleAssignment**。</span><span class="sxs-lookup"><span data-stu-id="3611d-149">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span> <span data-ttu-id="3611d-150">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3611d-150">Not nullable.</span></span> |
|<span data-ttu-id="3611d-151">appRoles</span><span class="sxs-lookup"><span data-stu-id="3611d-151">appRoles</span></span>|<span data-ttu-id="3611d-152">[appRole](../resources/approle.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3611d-152">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="3611d-153">关联应用程序公开的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="3611d-153">The application roles exposed by the associated application.</span></span> <span data-ttu-id="3611d-154">有关详细信息，请参阅[应用程序](../resources/application.md)资源上的**appRoles**属性定义。</span><span class="sxs-lookup"><span data-stu-id="3611d-154">For more information see the **appRoles** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="3611d-155">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3611d-155">Not nullable.</span></span> |
|<span data-ttu-id="3611d-156">displayName</span><span class="sxs-lookup"><span data-stu-id="3611d-156">displayName</span></span>|<span data-ttu-id="3611d-157">String</span><span class="sxs-lookup"><span data-stu-id="3611d-157">String</span></span>|<span data-ttu-id="3611d-158">服务主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3611d-158">The display name for the service principal.</span></span>|
|<span data-ttu-id="3611d-159">homepage</span><span class="sxs-lookup"><span data-stu-id="3611d-159">homepage</span></span>|<span data-ttu-id="3611d-160">String</span><span class="sxs-lookup"><span data-stu-id="3611d-160">String</span></span>|<span data-ttu-id="3611d-161">应用程序的主页或登录页。</span><span class="sxs-lookup"><span data-stu-id="3611d-161">Home page or landing page of the application.</span></span>|
|<span data-ttu-id="3611d-162">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="3611d-162">keyCredentials</span></span>|<span data-ttu-id="3611d-163">[keyCredential](../resources/keycredential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3611d-163">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="3611d-164">与服务帐户关联的密钥凭据集合。</span><span class="sxs-lookup"><span data-stu-id="3611d-164">The collection of key credentials associated with the service principal.</span></span> <span data-ttu-id="3611d-165">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3611d-165">Not nullable.</span></span>            |
|<span data-ttu-id="3611d-166">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="3611d-166">logoutUrl</span></span>|<span data-ttu-id="3611d-167">String</span><span class="sxs-lookup"><span data-stu-id="3611d-167">String</span></span>| <span data-ttu-id="3611d-168">指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。</span><span class="sxs-lookup"><span data-stu-id="3611d-168">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span>|
|<span data-ttu-id="3611d-169">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="3611d-169">oauth2PermissionScopes</span></span>|<span data-ttu-id="3611d-170">[permissionScope](../resources/permissionScope.md)集合</span><span class="sxs-lookup"><span data-stu-id="3611d-170">[permissionScope](../resources/permissionScope.md) collection</span></span>|<span data-ttu-id="3611d-171">由关联的应用程序公开的 OAuth 2.0 权限范围。</span><span class="sxs-lookup"><span data-stu-id="3611d-171">The OAuth 2.0 permission scopes exposed by the associated application.</span></span> <span data-ttu-id="3611d-172">有关详细信息，请参阅[应用程序](../resources/application.md)资源上的**oauth2PermissionScopes**属性定义。</span><span class="sxs-lookup"><span data-stu-id="3611d-172">For more information see the **oauth2PermissionScopes** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="3611d-173">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3611d-173">Not nullable.</span></span>|
|<span data-ttu-id="3611d-174">replyUrls</span><span class="sxs-lookup"><span data-stu-id="3611d-174">replyUrls</span></span>|<span data-ttu-id="3611d-175">String collection</span><span class="sxs-lookup"><span data-stu-id="3611d-175">String collection</span></span>|<span data-ttu-id="3611d-176">向其发送用户令牌以使用关联应用程序登录的 URL，或者为关联应用程序向其发送 OAuth 2.0 authorization 代码和访问令牌的重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="3611d-176">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span> <span data-ttu-id="3611d-177">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3611d-177">Not nullable.</span></span> |
|<span data-ttu-id="3611d-178">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="3611d-178">servicePrincipalNames</span></span>|<span data-ttu-id="3611d-179">String collection</span><span class="sxs-lookup"><span data-stu-id="3611d-179">String collection</span></span>|<span data-ttu-id="3611d-180">包含从关联的[应用程序](../resources/application.md)复制的**identifiersUris**的列表。</span><span class="sxs-lookup"><span data-stu-id="3611d-180">Contains the list of **identifiersUris**, copied over from the associated [application](../resources/application.md).</span></span> <span data-ttu-id="3611d-181">可以向混合应用程序中添加其他值。</span><span class="sxs-lookup"><span data-stu-id="3611d-181">Additional values can be added to hybrid applications.</span></span> <span data-ttu-id="3611d-182">这些值可用于标识此应用在 Azure AD 中公开的权限。</span><span class="sxs-lookup"><span data-stu-id="3611d-182">These values can be used to identify the permissions exposed by this app within Azure AD.</span></span> <span data-ttu-id="3611d-183">For example,</span><span class="sxs-lookup"><span data-stu-id="3611d-183">For example,</span></span><ul><li><span data-ttu-id="3611d-184">请求对此资源的权限的客户端应用程序可以使用这些 Uri 在其应用程序清单的**requiredResourceAccess**属性中，或在应用程序注册体验中的 "API 权限" 中指定所需的权限。</span><span class="sxs-lookup"><span data-stu-id="3611d-184">Client apps requesting permissions to this resource can use these URIs to specify needed permissions in the **requiredResourceAccess** property of their application manifest, or in the "API permissions" blade on the App registrations experience.</span></span></li><li><span data-ttu-id="3611d-185">客户端应用可以指定基于此属性的值获取访问令牌的资源 URI，这是在 "aud" 声明中返回的 URI。</span><span class="sxs-lookup"><span data-stu-id="3611d-185">Client apps can specify a resource URI which is based on the values of this property to acquire an access token, which is the URI returned in the “aud” claim.</span></span></li></ul><br><span data-ttu-id="3611d-186">需要多值属性筛选器表达式的 any 运算符。</span><span class="sxs-lookup"><span data-stu-id="3611d-186">The any operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="3611d-187">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3611d-187">Not nullable.</span></span>|
|<span data-ttu-id="3611d-188">标记</span><span class="sxs-lookup"><span data-stu-id="3611d-188">tags</span></span>|<span data-ttu-id="3611d-189">String 集合</span><span class="sxs-lookup"><span data-stu-id="3611d-189">String collection</span></span>| <span data-ttu-id="3611d-190">可用于分类和标识应用程序的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="3611d-190">Custom strings that can be used to categorize and identify the application.</span></span> <span data-ttu-id="3611d-191">不可为空。</span><span class="sxs-lookup"><span data-stu-id="3611d-191">Not nullable.</span></span> |
| <span data-ttu-id="3611d-192">tokenEncryptionKeyId</span><span class="sxs-lookup"><span data-stu-id="3611d-192">tokenEncryptionKeyId</span></span> |<span data-ttu-id="3611d-193">String</span><span class="sxs-lookup"><span data-stu-id="3611d-193">String</span></span>|<span data-ttu-id="3611d-194">指定 keyCredentials 集合中的公共密钥的 keyId。</span><span class="sxs-lookup"><span data-stu-id="3611d-194">Specifies the keyId of a public key from the keyCredentials collection.</span></span> <span data-ttu-id="3611d-195">配置后，Azure AD 将使用此属性指定的密钥为此应用程序颁发令牌。</span><span class="sxs-lookup"><span data-stu-id="3611d-195">When configured, Azure AD issues tokens for this application encrypted using the key specified by this property.</span></span> <span data-ttu-id="3611d-196">接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。</span><span class="sxs-lookup"><span data-stu-id="3611d-196">The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.</span></span>|

## <a name="response"></a><span data-ttu-id="3611d-197">响应</span><span class="sxs-lookup"><span data-stu-id="3611d-197">Response</span></span>

<span data-ttu-id="3611d-198">如果成功，此方法 `204 No Content` 在响应正文中返回响应代码和更新的[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3611d-198">If successful, this method returns a `204 No Content` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3611d-199">示例</span><span class="sxs-lookup"><span data-stu-id="3611d-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="3611d-200">请求</span><span class="sxs-lookup"><span data-stu-id="3611d-200">Request</span></span>
<span data-ttu-id="3611d-201">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3611d-201">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3611d-202">HTTP</span><span class="sxs-lookup"><span data-stu-id="3611d-202">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3611d-203">C#</span><span class="sxs-lookup"><span data-stu-id="3611d-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3611d-204">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3611d-204">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3611d-205">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3611d-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3611d-206">Java</span><span class="sxs-lookup"><span data-stu-id="3611d-206">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3611d-207">响应</span><span class="sxs-lookup"><span data-stu-id="3611d-207">Response</span></span>
<span data-ttu-id="3611d-208">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3611d-208">Here is an example of the response.</span></span> <span data-ttu-id="3611d-209">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3611d-209">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3611d-210">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3611d-210">All of the properties will be returned from an actual call.</span></span>
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
