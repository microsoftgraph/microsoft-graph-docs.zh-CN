---
title: 更新应用程序
description: 更新 application 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b06d9d998af2300d8114c98822ed7c76a6ec115
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518845"
---
# <a name="update-application"></a><span data-ttu-id="5ddca-103">更新应用程序</span><span class="sxs-lookup"><span data-stu-id="5ddca-103">Update application</span></span>

<span data-ttu-id="5ddca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ddca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ddca-105">更新[application](../resources/application.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5ddca-105">Update the properties of an [application](../resources/application.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ddca-106">权限</span><span class="sxs-lookup"><span data-stu-id="5ddca-106">Permissions</span></span>
<span data-ttu-id="5ddca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ddca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5ddca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ddca-109">Permission type</span></span>      | <span data-ttu-id="5ddca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ddca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ddca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ddca-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="5ddca-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5ddca-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5ddca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ddca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ddca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ddca-114">Not supported.</span></span>    |
|<span data-ttu-id="5ddca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ddca-115">Application</span></span> | <span data-ttu-id="5ddca-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ddca-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ddca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ddca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5ddca-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ddca-118">Request headers</span></span>
| <span data-ttu-id="5ddca-119">名称</span><span class="sxs-lookup"><span data-stu-id="5ddca-119">Name</span></span>       | <span data-ttu-id="5ddca-120">说明</span><span class="sxs-lookup"><span data-stu-id="5ddca-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5ddca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ddca-121">Authorization</span></span> | <span data-ttu-id="5ddca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ddca-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5ddca-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="5ddca-124">Content-type</span></span> | <span data-ttu-id="5ddca-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5ddca-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ddca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ddca-127">Request body</span></span>
<span data-ttu-id="5ddca-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="5ddca-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5ddca-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="5ddca-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5ddca-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5ddca-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5ddca-131">属性</span><span class="sxs-lookup"><span data-stu-id="5ddca-131">Property</span></span> | <span data-ttu-id="5ddca-132">类型</span><span class="sxs-lookup"><span data-stu-id="5ddca-132">Type</span></span> | <span data-ttu-id="5ddca-133">说明</span><span class="sxs-lookup"><span data-stu-id="5ddca-133">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="5ddca-134">api</span><span class="sxs-lookup"><span data-stu-id="5ddca-134">api</span></span> | [<span data-ttu-id="5ddca-135">apiApplication</span><span class="sxs-lookup"><span data-stu-id="5ddca-135">apiApplication</span></span>](../resources/apiapplication.md) | <span data-ttu-id="5ddca-136">指定实现 Web API 的应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="5ddca-136">Specifies settings for an application that implements a web API.</span></span> |
| <span data-ttu-id="5ddca-137">appRoles</span><span class="sxs-lookup"><span data-stu-id="5ddca-137">appRoles</span></span> | <span data-ttu-id="5ddca-138">[appRole](../resources/approle.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ddca-138">[appRole](../resources/approle.md) collection</span></span> | <span data-ttu-id="5ddca-139">应用程序可声明的应用程序角色的集合。</span><span class="sxs-lookup"><span data-stu-id="5ddca-139">The collection of application roles that an application may declare.</span></span> <span data-ttu-id="5ddca-140">这些角色可以分配给用户、组或服务主体。</span><span class="sxs-lookup"><span data-stu-id="5ddca-140">These roles can be assigned to users, groups, or service principals.</span></span> <span data-ttu-id="5ddca-141">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="5ddca-141">Not nullable.</span></span> |
| <span data-ttu-id="5ddca-142">displayName</span><span class="sxs-lookup"><span data-stu-id="5ddca-142">displayName</span></span> | <span data-ttu-id="5ddca-143">String</span><span class="sxs-lookup"><span data-stu-id="5ddca-143">String</span></span> | <span data-ttu-id="5ddca-144">应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5ddca-144">The display name for the application.</span></span> |
| <span data-ttu-id="5ddca-145">groupMembershipClaims</span><span class="sxs-lookup"><span data-stu-id="5ddca-145">groupMembershipClaims</span></span> | <span data-ttu-id="5ddca-146">字符串</span><span class="sxs-lookup"><span data-stu-id="5ddca-146">String</span></span> | <span data-ttu-id="5ddca-147">配置在应用程序需要的用户或 OAuth 2.0 访问令牌中颁发的**组**声明。</span><span class="sxs-lookup"><span data-stu-id="5ddca-147">Configures the **groups** claim issued in a user or OAuth 2.0 access token that the application expects.</span></span> <span data-ttu-id="5ddca-148">要设置此属性，请使用以下有效字符串值之一：</span><span class="sxs-lookup"><span data-stu-id="5ddca-148">To set this attribute, use one of the following valid string values:</span></span><ul><li>`None`</li><li><span data-ttu-id="5ddca-149">`SecurityGroup`：针对安全组和 Azure Active Directory （Azure AD）角色</span><span class="sxs-lookup"><span data-stu-id="5ddca-149">`SecurityGroup`: For security groups and Azure Active Directory (Azure AD) roles</span></span></li><li><span data-ttu-id="5ddca-150">`All`：该操作可获取登录用户所属的所有安全组、通讯组和 Azure AD 目录角色</span><span class="sxs-lookup"><span data-stu-id="5ddca-150">`All`: This will get all of the security groups, distribution groups, and Azure AD directory roles that the signed-in user is a member of</span></span></li></ul> |
| <span data-ttu-id="5ddca-151">identifierUris</span><span class="sxs-lookup"><span data-stu-id="5ddca-151">identifierUris</span></span> | <span data-ttu-id="5ddca-152">String collection</span><span class="sxs-lookup"><span data-stu-id="5ddca-152">String collection</span></span> | <span data-ttu-id="5ddca-153">URI，用于在应用程序的 Azure AD 租户中标识该应用程序；如果应用程序是多租户的，则用于在已验证的自定义域中标识该应用程序。</span><span class="sxs-lookup"><span data-stu-id="5ddca-153">The URIs that identify the application within its Azure AD tenant, or within a verified custom domain if the application is multi-tenant.</span></span> <span data-ttu-id="5ddca-154">有关详细信息，请参阅[应用程序对象和服务主体对象](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)。</span><span class="sxs-lookup"><span data-stu-id="5ddca-154">For more information, see [Application Objects and Service Principal Objects](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).</span></span> <span data-ttu-id="5ddca-155">需要多值属性筛选器表达式的 *any* 运算符。</span><span class="sxs-lookup"><span data-stu-id="5ddca-155">The *any* operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="5ddca-156">不可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="5ddca-156">Not nullable.</span></span> |
| <span data-ttu-id="5ddca-157">info</span><span class="sxs-lookup"><span data-stu-id="5ddca-157">info</span></span> | [<span data-ttu-id="5ddca-158">informationalUrl</span><span class="sxs-lookup"><span data-stu-id="5ddca-158">informationalUrl</span></span>](../resources/informationalurl.md) | <span data-ttu-id="5ddca-159">应用程序的基本配置文件信息，如应用程序的营销、支持、服务条款和隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="5ddca-159">Basic profile information of the application such as  app's marketing, support, terms of service, and privacy statement URLs.</span></span> <span data-ttu-id="5ddca-160">服务条款和隐私声明通过用户同意体验展示给用户。</span><span class="sxs-lookup"><span data-stu-id="5ddca-160">The terms of service and privacy statement are surfaced to users through the user consent experience.</span></span> <span data-ttu-id="5ddca-161">有关详细信息，请参阅[为已注册的 AZURE AD 应用添加服务条款和隐私声明](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement)。</span><span class="sxs-lookup"><span data-stu-id="5ddca-161">For more information, see [Add Terms of service and privacy statement for registered Azure AD apps](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement).</span></span> |
| <span data-ttu-id="5ddca-162">isFallbackPublicClient</span><span class="sxs-lookup"><span data-stu-id="5ddca-162">isFallbackPublicClient</span></span> | <span data-ttu-id="5ddca-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ddca-163">Boolean</span></span> | <span data-ttu-id="5ddca-164">将回退应用程序类型指定为公共客户端，例如在移动设备上运行的已安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="5ddca-164">Specifies the fallback application type as public client, such as an installed application running on a mobile device.</span></span> <span data-ttu-id="5ddca-165">默认值是`false`，这意味着回退应用程序类型是机密客户端，如 web app。</span><span class="sxs-lookup"><span data-stu-id="5ddca-165">The default value is `false`, which means the fallback application type is confidential client such as web app.</span></span> <span data-ttu-id="5ddca-166">在某些情况下，Azure AD 无法确定客户端应用程序类型（例如，在未指定重定向 URI 的情况下配置它的[ROPC](https://tools.ietf.org/html/rfc6749#section-4.3)流）。</span><span class="sxs-lookup"><span data-stu-id="5ddca-166">There are certain scenarios where Azure AD cannot determine the client application type (for example, [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) flow where it is configured without specifying a redirect URI).</span></span> <span data-ttu-id="5ddca-167">在这些情况下，Azure AD 将根据此属性的值解释应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="5ddca-167">In those cases, Azure AD will interpret the application type based on the value of this property.</span></span>|
| <span data-ttu-id="5ddca-168">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="5ddca-168">keyCredentials</span></span> | <span data-ttu-id="5ddca-169">[keyCredential](../resources/keycredential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ddca-169">[keyCredential](../resources/keycredential.md) collection</span></span> | <span data-ttu-id="5ddca-170">与应用程序关联的密钥凭据的集合。</span><span class="sxs-lookup"><span data-stu-id="5ddca-170">The collection of key credentials associated with the application.</span></span> <span data-ttu-id="5ddca-171">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="5ddca-171">Not nullable.</span></span> |
| <span data-ttu-id="5ddca-172">logo</span><span class="sxs-lookup"><span data-stu-id="5ddca-172">logo</span></span> | <span data-ttu-id="5ddca-173">Stream</span><span class="sxs-lookup"><span data-stu-id="5ddca-173">Stream</span></span> | <span data-ttu-id="5ddca-174">应用程序的主徽标。</span><span class="sxs-lookup"><span data-stu-id="5ddca-174">The main logo for the application.</span></span> <span data-ttu-id="5ddca-175">不可为空。</span><span class="sxs-lookup"><span data-stu-id="5ddca-175">Not nullable.</span></span> |
| <span data-ttu-id="5ddca-176">optionalClaims</span><span class="sxs-lookup"><span data-stu-id="5ddca-176">optionalClaims</span></span> | <span data-ttu-id="5ddca-177">optionalClaims</span><span class="sxs-lookup"><span data-stu-id="5ddca-177">optionalClaims</span></span> | <span data-ttu-id="5ddca-178">应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以指定 Microsoft 安全令牌服务发送到他们应用程序的令牌中所需的声明。</span><span class="sxs-lookup"><span data-stu-id="5ddca-178">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="5ddca-179">有关详细信息，请参阅[可选声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="5ddca-179">See [optional claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span> |
| <span data-ttu-id="5ddca-180">parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="5ddca-180">parentalControlSettings</span></span> | [<span data-ttu-id="5ddca-181">parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="5ddca-181">parentalControlSettings</span></span>](../resources/parentalcontrolsettings.md) |<span data-ttu-id="5ddca-182">指定应用程序的家长控制设置。</span><span class="sxs-lookup"><span data-stu-id="5ddca-182">Specifies parental control settings for an application.</span></span> |
| <span data-ttu-id="5ddca-183">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="5ddca-183">passwordCredentials</span></span> | <span data-ttu-id="5ddca-184">[passwordCredential](../resources/passwordcredential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ddca-184">[passwordCredential](../resources/passwordcredential.md) collection</span></span>|<span data-ttu-id="5ddca-185">与应用程序关联的密码凭据集合。</span><span class="sxs-lookup"><span data-stu-id="5ddca-185">The collection of password credentials associated with the application.</span></span> <span data-ttu-id="5ddca-186">不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="5ddca-186">Not nullable.</span></span>|
| <span data-ttu-id="5ddca-187">publicClient</span><span class="sxs-lookup"><span data-stu-id="5ddca-187">publicClient</span></span> | [<span data-ttu-id="5ddca-188">publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="5ddca-188">publicClientApplication</span></span>](../resources/publicclientapplication.md) | <span data-ttu-id="5ddca-189">指定已安装客户端（如台式设备或移动设备）的设置。</span><span class="sxs-lookup"><span data-stu-id="5ddca-189">Specifies settings for installed clients such as desktop or mobile devices.</span></span> |
| <span data-ttu-id="5ddca-190">requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="5ddca-190">requiredResourceAccess</span></span> |<span data-ttu-id="5ddca-191">[requiredResourceAccess](../resources/requiredresourceaccess.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ddca-191">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span></span>|<span data-ttu-id="5ddca-192">指定此应用程序需要访问的资源以及在每个资源下所需的 OAuth 权限范围和应用程序角色集。</span><span class="sxs-lookup"><span data-stu-id="5ddca-192">Specifies resources that this application requires access to and the set of OAuth permission scopes and application roles that it needs under each of those resources.</span></span> <span data-ttu-id="5ddca-193">这种预配置的所需资源访问权限可驱动同意体验。</span><span class="sxs-lookup"><span data-stu-id="5ddca-193">This pre-configuration of required resource access drives the consent experience.</span></span> <span data-ttu-id="5ddca-194">不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="5ddca-194">Not nullable.</span></span>|
| <span data-ttu-id="5ddca-195">signInAudience</span><span class="sxs-lookup"><span data-stu-id="5ddca-195">signInAudience</span></span> | <span data-ttu-id="5ddca-196">String</span><span class="sxs-lookup"><span data-stu-id="5ddca-196">String</span></span> | <span data-ttu-id="5ddca-197">指定当前应用程序支持的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="5ddca-197">Specifies what Microsoft accounts are supported for the current application.</span></span> <span data-ttu-id="5ddca-198">支持的值为：</span><span class="sxs-lookup"><span data-stu-id="5ddca-198">Supported values are:</span></span><ul><li><span data-ttu-id="5ddca-199">`AzureADMyOrg`：在我的组织的 Azure AD 租户（即单租户）中拥有 Microsoft 工作或学校帐户的用户</span><span class="sxs-lookup"><span data-stu-id="5ddca-199">`AzureADMyOrg`: Users with a Microsoft work or school account in my organization’s Azure AD tenant (i.e. single tenant)</span></span></li><li><span data-ttu-id="5ddca-200">`AzureADMultipleOrgs`：在任何组织的 Azure AD 租户（即多租户）中拥有 Microsoft 工作或学校帐户的用户</span><span class="sxs-lookup"><span data-stu-id="5ddca-200">`AzureADMultipleOrgs`: Users with a Microsoft work or school account in any organization’s Azure AD tenant (i.e. multi-tenant)</span></span></li> <li><span data-ttu-id="5ddca-201">`AzureADandPersonalMicrosoftAccount`：拥有个人 Microsoft 帐户或任意组织的 Azure AD 租户中的工作或学校帐户的用户</span><span class="sxs-lookup"><span data-stu-id="5ddca-201">`AzureADandPersonalMicrosoftAccount`: Users with a personal Microsoft account, or a work or school account in any organization’s Azure AD tenant</span></span></li></ul> | `AzureADandPersonalMicrosoftAccount` |
| <span data-ttu-id="5ddca-202">tags</span><span class="sxs-lookup"><span data-stu-id="5ddca-202">tags</span></span> |<span data-ttu-id="5ddca-203">String 集合</span><span class="sxs-lookup"><span data-stu-id="5ddca-203">String collection</span></span>| <span data-ttu-id="5ddca-204">可用于分类和标识应用程序的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="5ddca-204">Custom strings that can be used to categorize and identify the application.</span></span> <span data-ttu-id="5ddca-205">不可为空。</span><span class="sxs-lookup"><span data-stu-id="5ddca-205">Not nullable.</span></span>|
| <span data-ttu-id="5ddca-206">tokenEncryptionKeyId</span><span class="sxs-lookup"><span data-stu-id="5ddca-206">tokenEncryptionKeyId</span></span> |<span data-ttu-id="5ddca-207">字符串</span><span class="sxs-lookup"><span data-stu-id="5ddca-207">String</span></span>|<span data-ttu-id="5ddca-208">指定 keyCredentials 集合中的公共密钥的 keyId。</span><span class="sxs-lookup"><span data-stu-id="5ddca-208">Specifies the keyId of a public key from the keyCredentials collection.</span></span> <span data-ttu-id="5ddca-209">配置后，Azure AD 将使用此属性指向的密钥对其发出的所有令牌进行加密。</span><span class="sxs-lookup"><span data-stu-id="5ddca-209">When configured, Azure AD encrypts all the tokens it emits by using the key this property points to.</span></span> <span data-ttu-id="5ddca-210">接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。</span><span class="sxs-lookup"><span data-stu-id="5ddca-210">The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.</span></span>|
| <span data-ttu-id="5ddca-211">web</span><span class="sxs-lookup"><span data-stu-id="5ddca-211">web</span></span> |[<span data-ttu-id="5ddca-212">webApplication</span><span class="sxs-lookup"><span data-stu-id="5ddca-212">webApplication</span></span>](../resources/webapplication.md)| <span data-ttu-id="5ddca-213">指定 Web 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="5ddca-213">Specifies settings for a web application.</span></span> |

## <a name="response"></a><span data-ttu-id="5ddca-214">响应</span><span class="sxs-lookup"><span data-stu-id="5ddca-214">Response</span></span>

<span data-ttu-id="5ddca-215">如果成功，此方法将`204 No Content`返回响应代码，并且不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5ddca-215">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ddca-216">示例</span><span class="sxs-lookup"><span data-stu-id="5ddca-216">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ddca-217">请求</span><span class="sxs-lookup"><span data-stu-id="5ddca-217">Request</span></span>
<span data-ttu-id="5ddca-218">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ddca-218">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5ddca-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ddca-219">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/applications/{id}
Content-type: application/json
Content-length: 72

{
  "displayName": "New display name"
}
```
# <a name="c"></a>[<span data-ttu-id="5ddca-220">C#</span><span class="sxs-lookup"><span data-stu-id="5ddca-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ddca-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ddca-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ddca-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ddca-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ddca-223">Java</span><span class="sxs-lookup"><span data-stu-id="5ddca-223">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5ddca-224">响应</span><span class="sxs-lookup"><span data-stu-id="5ddca-224">Response</span></span>

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
