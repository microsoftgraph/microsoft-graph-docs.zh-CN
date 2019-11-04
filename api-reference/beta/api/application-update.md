---
title: 更新应用程序
description: 更新 application 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5850de9653891e0eb4f8acac07d9bd6dd5ea6ada
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934933"
---
# <a name="update-application"></a><span data-ttu-id="017a8-103">更新应用程序</span><span class="sxs-lookup"><span data-stu-id="017a8-103">Update application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="017a8-104">更新[application](../resources/application.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="017a8-104">Update the properties of an [application](../resources/application.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="017a8-105">权限</span><span class="sxs-lookup"><span data-stu-id="017a8-105">Permissions</span></span>
<span data-ttu-id="017a8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="017a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="017a8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="017a8-108">Permission type</span></span>      | <span data-ttu-id="017a8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="017a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="017a8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="017a8-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="017a8-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="017a8-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="017a8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="017a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="017a8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="017a8-113">Not supported.</span></span>    |
|<span data-ttu-id="017a8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="017a8-114">Application</span></span> | <span data-ttu-id="017a8-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="017a8-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="017a8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="017a8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a><span data-ttu-id="017a8-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="017a8-117">Request headers</span></span>
| <span data-ttu-id="017a8-118">名称</span><span class="sxs-lookup"><span data-stu-id="017a8-118">Name</span></span>       | <span data-ttu-id="017a8-119">类型</span><span class="sxs-lookup"><span data-stu-id="017a8-119">Type</span></span> | <span data-ttu-id="017a8-120">说明</span><span class="sxs-lookup"><span data-stu-id="017a8-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="017a8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="017a8-121">Authorization</span></span>  | <span data-ttu-id="017a8-122">string</span><span class="sxs-lookup"><span data-stu-id="017a8-122">string</span></span>  | <span data-ttu-id="017a8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="017a8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="017a8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="017a8-125">Request body</span></span>
<span data-ttu-id="017a8-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="017a8-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="017a8-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="017a8-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="017a8-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="017a8-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="017a8-129">属性</span><span class="sxs-lookup"><span data-stu-id="017a8-129">Property</span></span> | <span data-ttu-id="017a8-130">类型</span><span class="sxs-lookup"><span data-stu-id="017a8-130">Type</span></span> | <span data-ttu-id="017a8-131">说明</span><span class="sxs-lookup"><span data-stu-id="017a8-131">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="017a8-132">api</span><span class="sxs-lookup"><span data-stu-id="017a8-132">api</span></span> | [<span data-ttu-id="017a8-133">apiApplication</span><span class="sxs-lookup"><span data-stu-id="017a8-133">apiApplication</span></span>](../resources/apiapplication.md) | <span data-ttu-id="017a8-134">指定实现 web API 的应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="017a8-134">Specifies settings for an application that implements a web API.</span></span> |
| <span data-ttu-id="017a8-135">appRoles</span><span class="sxs-lookup"><span data-stu-id="017a8-135">appRoles</span></span> | <span data-ttu-id="017a8-136">[appRole](../resources/approle.md) 集合</span><span class="sxs-lookup"><span data-stu-id="017a8-136">[appRole](../resources/approle.md) collection</span></span> | <span data-ttu-id="017a8-137">应用程序可声明的应用程序角色的集合。</span><span class="sxs-lookup"><span data-stu-id="017a8-137">The collection of application roles that an application may declare.</span></span> <span data-ttu-id="017a8-138">这些角色可以分配给用户、组或服务主体。</span><span class="sxs-lookup"><span data-stu-id="017a8-138">These roles can be assigned to users, groups, or service principals.</span></span> <span data-ttu-id="017a8-139">不可为空。</span><span class="sxs-lookup"><span data-stu-id="017a8-139">Not nullable.</span></span> |
| <span data-ttu-id="017a8-140">displayName</span><span class="sxs-lookup"><span data-stu-id="017a8-140">displayName</span></span> | <span data-ttu-id="017a8-141">String</span><span class="sxs-lookup"><span data-stu-id="017a8-141">String</span></span> | <span data-ttu-id="017a8-142">应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="017a8-142">The display name for the application.</span></span> |
| <span data-ttu-id="017a8-143">groupMembershipClaims</span><span class="sxs-lookup"><span data-stu-id="017a8-143">groupMembershipClaims</span></span> | <span data-ttu-id="017a8-144">字符串</span><span class="sxs-lookup"><span data-stu-id="017a8-144">String</span></span> | <span data-ttu-id="017a8-145">配置在应用程序需要的用户或 OAuth 2.0 访问令牌中颁发的**组**声明。</span><span class="sxs-lookup"><span data-stu-id="017a8-145">Configures the **groups** claim issued in a user or OAuth 2.0 access token that the application expects.</span></span> <span data-ttu-id="017a8-146">若要设置此属性，请使用下列有效的字符串值之一：</span><span class="sxs-lookup"><span data-stu-id="017a8-146">To set this attribute, use one of the following valid string values:</span></span><ul><li>`None`</li><li><span data-ttu-id="017a8-147">`SecurityGroup`：针对安全组和 Azure Active Directory （Azure AD）角色</span><span class="sxs-lookup"><span data-stu-id="017a8-147">`SecurityGroup`: For security groups and Azure Active Directory (Azure AD) roles</span></span></li><li><span data-ttu-id="017a8-148">`All`：这将获取已登录用户所属的所有安全组、通讯组和 Azure AD 目录角色</span><span class="sxs-lookup"><span data-stu-id="017a8-148">`All`: This will get all of the security groups, distribution groups, and Azure AD directory roles that the signed-in user is a member of</span></span></li></ul> |
| <span data-ttu-id="017a8-149">identifierUris</span><span class="sxs-lookup"><span data-stu-id="017a8-149">identifierUris</span></span> | <span data-ttu-id="017a8-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="017a8-150">String collection</span></span> | <span data-ttu-id="017a8-151">用于标识其 Azure AD 租户内的应用程序的 Uri，或在已验证的自定义域中（如果应用程序是多租户）。</span><span class="sxs-lookup"><span data-stu-id="017a8-151">The URIs that identify the application within its Azure AD tenant, or within a verified custom domain if the application is multi-tenant.</span></span> <span data-ttu-id="017a8-152">有关详细信息，请参阅[应用程序对象和服务主体对象](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)。</span><span class="sxs-lookup"><span data-stu-id="017a8-152">For more information, see [Application Objects and Service Principal Objects](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).</span></span> <span data-ttu-id="017a8-153">多值属性筛选器表达式需要 *any* 运算符。</span><span class="sxs-lookup"><span data-stu-id="017a8-153">The *any* operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="017a8-154">不可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="017a8-154">Not nullable.</span></span> |
| <span data-ttu-id="017a8-155">info</span><span class="sxs-lookup"><span data-stu-id="017a8-155">info</span></span> | [<span data-ttu-id="017a8-156">informationalUrl</span><span class="sxs-lookup"><span data-stu-id="017a8-156">informationalUrl</span></span>](../resources/informationalurl.md) | <span data-ttu-id="017a8-157">应用程序的基本配置文件信息，如应用程序的营销、支持、服务条款和隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="017a8-157">Basic profile information of the application such as  app's marketing, support, terms of service, and privacy statement URLs.</span></span> <span data-ttu-id="017a8-158">服务条款和隐私声明通过用户同意体验向用户呈现。</span><span class="sxs-lookup"><span data-stu-id="017a8-158">The terms of service and privacy statement are surfaced to users through the user consent experience.</span></span> <span data-ttu-id="017a8-159">有关详细信息，请参阅[为已注册的 AZURE AD 应用添加服务条款和隐私声明](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement)。</span><span class="sxs-lookup"><span data-stu-id="017a8-159">For more information, see [Add Terms of service and privacy statement for registered Azure AD apps](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement).</span></span> |
| <span data-ttu-id="017a8-160">isFallbackPublicClient</span><span class="sxs-lookup"><span data-stu-id="017a8-160">isFallbackPublicClient</span></span> | <span data-ttu-id="017a8-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="017a8-161">Boolean</span></span> | <span data-ttu-id="017a8-162">将回退应用程序类型指定为公共客户端，例如在移动设备上运行的已安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="017a8-162">Specifies the fallback application type as public client, such as an installed application running on a mobile device.</span></span> <span data-ttu-id="017a8-163">默认值是`false`，这意味着回退应用程序类型是机密客户端，如 web app。</span><span class="sxs-lookup"><span data-stu-id="017a8-163">The default value is `false`, which means the fallback application type is confidential client such as web app.</span></span> <span data-ttu-id="017a8-164">在某些情况下，Azure AD 无法确定客户端应用程序类型（例如，在未指定重定向 URI 的情况下配置它的[ROPC](https://tools.ietf.org/html/rfc6749#section-4.3)流）。</span><span class="sxs-lookup"><span data-stu-id="017a8-164">There are certain scenarios where Azure AD cannot determine the client application type (for example, [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) flow where it is configured without specifying a redirect URI).</span></span> <span data-ttu-id="017a8-165">在这些情况下，Azure AD 将根据此属性的值解释应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="017a8-165">In those cases, Azure AD will interpret the application type based on the value of this property.</span></span>|
| <span data-ttu-id="017a8-166">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="017a8-166">keyCredentials</span></span> | <span data-ttu-id="017a8-167">[keyCredential](../resources/keycredential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="017a8-167">[keyCredential](../resources/keycredential.md) collection</span></span> | <span data-ttu-id="017a8-168">与应用程序关联的密钥凭据的集合。</span><span class="sxs-lookup"><span data-stu-id="017a8-168">The collection of key credentials associated with the application.</span></span> <span data-ttu-id="017a8-169">不可为空。</span><span class="sxs-lookup"><span data-stu-id="017a8-169">Not nullable.</span></span> |
| <span data-ttu-id="017a8-170">logo</span><span class="sxs-lookup"><span data-stu-id="017a8-170">logo</span></span> | <span data-ttu-id="017a8-171">Stream</span><span class="sxs-lookup"><span data-stu-id="017a8-171">Stream</span></span> | <span data-ttu-id="017a8-172">应用程序的主徽标。</span><span class="sxs-lookup"><span data-stu-id="017a8-172">The main logo for the application.</span></span> <span data-ttu-id="017a8-173">不可为空。</span><span class="sxs-lookup"><span data-stu-id="017a8-173">Not nullable.</span></span> |
| <span data-ttu-id="017a8-174">optionalClaims</span><span class="sxs-lookup"><span data-stu-id="017a8-174">optionalClaims</span></span> | <span data-ttu-id="017a8-175">optionalClaims</span><span class="sxs-lookup"><span data-stu-id="017a8-175">optionalClaims</span></span> | <span data-ttu-id="017a8-176">应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以在 Microsoft 安全令牌服务向其应用程序发送令牌中指定要使用的声明。</span><span class="sxs-lookup"><span data-stu-id="017a8-176">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="017a8-177">有关详细信息，请参阅[可选声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="017a8-177">See [optional claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span> |
| <span data-ttu-id="017a8-178">parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="017a8-178">parentalControlSettings</span></span> | [<span data-ttu-id="017a8-179">parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="017a8-179">parentalControlSettings</span></span>](../resources/parentalcontrolsettings.md) |<span data-ttu-id="017a8-180">指定应用程序的家长控制设置。</span><span class="sxs-lookup"><span data-stu-id="017a8-180">Specifies parental control settings for an application.</span></span> |
| <span data-ttu-id="017a8-181">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="017a8-181">passwordCredentials</span></span> | <span data-ttu-id="017a8-182">[passwordCredential](../resources/passwordcredential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="017a8-182">[passwordCredential](../resources/passwordcredential.md) collection</span></span>|<span data-ttu-id="017a8-183">与应用程序关联的密码凭据集合。</span><span class="sxs-lookup"><span data-stu-id="017a8-183">The collection of password credentials associated with the application.</span></span> <span data-ttu-id="017a8-184">不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="017a8-184">Not nullable.</span></span>|
| <span data-ttu-id="017a8-185">publicClient</span><span class="sxs-lookup"><span data-stu-id="017a8-185">publicClient</span></span> | [<span data-ttu-id="017a8-186">publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="017a8-186">publicClientApplication</span></span>](../resources/publicclientapplication.md) | <span data-ttu-id="017a8-187">指定已安装客户端（如台式设备或移动设备）的设置。</span><span class="sxs-lookup"><span data-stu-id="017a8-187">Specifies settings for installed clients such as desktop or mobile devices.</span></span> |
| <span data-ttu-id="017a8-188">requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="017a8-188">requiredResourceAccess</span></span> |<span data-ttu-id="017a8-189">[requiredResourceAccess](../resources/requiredresourceaccess.md) 集合</span><span class="sxs-lookup"><span data-stu-id="017a8-189">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span></span>|<span data-ttu-id="017a8-190">指定此应用程序需要访问的资源以及在每个资源下所需的 OAuth 权限范围和应用程序角色集。</span><span class="sxs-lookup"><span data-stu-id="017a8-190">Specifies resources that this application requires access to and the set of OAuth permission scopes and application roles that it needs under each of those resources.</span></span> <span data-ttu-id="017a8-191">这种预配置的所需资源访问权限可驱动同意体验。</span><span class="sxs-lookup"><span data-stu-id="017a8-191">This pre-configuration of required resource access drives the consent experience.</span></span> <span data-ttu-id="017a8-192">不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="017a8-192">Not nullable.</span></span>|
| <span data-ttu-id="017a8-193">signInAudience</span><span class="sxs-lookup"><span data-stu-id="017a8-193">signInAudience</span></span> | <span data-ttu-id="017a8-194">String</span><span class="sxs-lookup"><span data-stu-id="017a8-194">String</span></span> | <span data-ttu-id="017a8-195">指定当前应用程序支持的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="017a8-195">Specifies what Microsoft accounts are supported for the current application.</span></span> <span data-ttu-id="017a8-196">支持的值为：</span><span class="sxs-lookup"><span data-stu-id="017a8-196">Supported values are:</span></span><ul><li><span data-ttu-id="017a8-197">`AzureADMyOrg`：在我的组织的 Azure AD 租户中使用 Microsoft 工作或学校帐户的用户（即单个租户）</span><span class="sxs-lookup"><span data-stu-id="017a8-197">`AzureADMyOrg`: Users with a Microsoft work or school account in my organization’s Azure AD tenant (i.e. single tenant)</span></span></li><li><span data-ttu-id="017a8-198">`AzureADMultipleOrgs`：在任何组织的 Azure AD 租户中具有 Microsoft 工作或学校帐户的用户（即多租户）</span><span class="sxs-lookup"><span data-stu-id="017a8-198">`AzureADMultipleOrgs`: Users with a Microsoft work or school account in any organization’s Azure AD tenant (i.e. multi-tenant)</span></span></li> <li><span data-ttu-id="017a8-199">`AzureADandPersonalMicrosoftAccount`：拥有个人 Microsoft 帐户的用户，或任何组织的 Azure AD 租户中的工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="017a8-199">`AzureADandPersonalMicrosoftAccount`: Users with a personal Microsoft account, or a work or school account in any organization’s Azure AD tenant</span></span></li></ul> | `AzureADandPersonalMicrosoftAccount` |
| <span data-ttu-id="017a8-200">标记</span><span class="sxs-lookup"><span data-stu-id="017a8-200">tags</span></span> |<span data-ttu-id="017a8-201">String collection</span><span class="sxs-lookup"><span data-stu-id="017a8-201">String collection</span></span>| <span data-ttu-id="017a8-202">可用于分类和标识应用程序的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="017a8-202">Custom strings that can be used to categorize and identify the application.</span></span> <span data-ttu-id="017a8-203">不可为空。</span><span class="sxs-lookup"><span data-stu-id="017a8-203">Not nullable.</span></span>|
| <span data-ttu-id="017a8-204">tokenEncryptionKeyId</span><span class="sxs-lookup"><span data-stu-id="017a8-204">tokenEncryptionKeyId</span></span> |<span data-ttu-id="017a8-205">字符串</span><span class="sxs-lookup"><span data-stu-id="017a8-205">String</span></span>|<span data-ttu-id="017a8-206">指定 keyCredentials 集合中的公钥的密钥 keyId。</span><span class="sxs-lookup"><span data-stu-id="017a8-206">Specifies the keyId of a public key from the keyCredentials collection.</span></span> <span data-ttu-id="017a8-207">配置后，Azure AD 将使用此属性指向的密钥对其发出的所有令牌进行加密。</span><span class="sxs-lookup"><span data-stu-id="017a8-207">When configured, Azure AD encrypts all the tokens it emits by using the key this property points to.</span></span> <span data-ttu-id="017a8-208">接收加密令牌的应用程序代码必须使用匹配私钥来解密令牌，然后才能将其用于登录用户。</span><span class="sxs-lookup"><span data-stu-id="017a8-208">The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.</span></span>|
| <span data-ttu-id="017a8-209">web</span><span class="sxs-lookup"><span data-stu-id="017a8-209">web</span></span> |[<span data-ttu-id="017a8-210">webApplication</span><span class="sxs-lookup"><span data-stu-id="017a8-210">webApplication</span></span>](../resources/webapplication.md)| <span data-ttu-id="017a8-211">指定 Web 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="017a8-211">Specifies settings for a web application.</span></span> |

## <a name="response"></a><span data-ttu-id="017a8-212">响应</span><span class="sxs-lookup"><span data-stu-id="017a8-212">Response</span></span>

<span data-ttu-id="017a8-213">如果成功，此方法将`204 No Content`返回响应代码，并且不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="017a8-213">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="017a8-214">示例</span><span class="sxs-lookup"><span data-stu-id="017a8-214">Example</span></span>
##### <a name="request"></a><span data-ttu-id="017a8-215">请求</span><span class="sxs-lookup"><span data-stu-id="017a8-215">Request</span></span>
<span data-ttu-id="017a8-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="017a8-216">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="017a8-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="017a8-217">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json
Content-length: 72

{
  "displayName": "New display name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="017a8-218">C#</span><span class="sxs-lookup"><span data-stu-id="017a8-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="017a8-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="017a8-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="017a8-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="017a8-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="017a8-221">响应</span><span class="sxs-lookup"><span data-stu-id="017a8-221">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
