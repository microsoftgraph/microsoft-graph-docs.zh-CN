---
title: 更新应用程序
description: 更新 application 对象的属性。
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 366d6bf12cf620aa844e97cdbd8a4218b54a29ba
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289656"
---
# <a name="update-application"></a><span data-ttu-id="c1dac-103">更新应用程序</span><span class="sxs-lookup"><span data-stu-id="c1dac-103">Update application</span></span>

<span data-ttu-id="c1dac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1dac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1dac-105">更新[application](../resources/application.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c1dac-105">Update the properties of an [application](../resources/application.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c1dac-106">不支持使用修补程序设置[**passwordCredential**](../resources/passwordcredential.md) 。</span><span class="sxs-lookup"><span data-stu-id="c1dac-106">Using PATCH to set [**passwordCredential**](../resources/passwordcredential.md) is not supported.</span></span> <span data-ttu-id="c1dac-107">使用[addPassword](./application-addpassword.md)和[removePassword](./application-removepassword.md)方法更新应用程序的密码。</span><span class="sxs-lookup"><span data-stu-id="c1dac-107">Use the [addPassword](./application-addpassword.md) and [removePassword](./application-removepassword.md) methods to update the password for an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1dac-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="c1dac-108">Permissions</span></span>
<span data-ttu-id="c1dac-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1dac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c1dac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1dac-111">Permission type</span></span>      | <span data-ttu-id="c1dac-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1dac-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1dac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1dac-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c1dac-114">Directory.accessasuser.all 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="c1dac-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c1dac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1dac-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1dac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1dac-116">Not supported.</span></span>    |
|<span data-ttu-id="c1dac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1dac-117">Application</span></span> | <span data-ttu-id="c1dac-118">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1dac-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1dac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1dac-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c1dac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1dac-120">Request headers</span></span>
| <span data-ttu-id="c1dac-121">名称</span><span class="sxs-lookup"><span data-stu-id="c1dac-121">Name</span></span>       | <span data-ttu-id="c1dac-122">说明</span><span class="sxs-lookup"><span data-stu-id="c1dac-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c1dac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1dac-123">Authorization</span></span> | <span data-ttu-id="c1dac-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1dac-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c1dac-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1dac-126">Content-Type</span></span> | <span data-ttu-id="c1dac-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c1dac-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1dac-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1dac-129">Request body</span></span>
<span data-ttu-id="c1dac-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c1dac-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c1dac-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c1dac-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c1dac-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c1dac-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c1dac-133">属性</span><span class="sxs-lookup"><span data-stu-id="c1dac-133">Property</span></span> | <span data-ttu-id="c1dac-134">类型</span><span class="sxs-lookup"><span data-stu-id="c1dac-134">Type</span></span> | <span data-ttu-id="c1dac-135">Description</span><span class="sxs-lookup"><span data-stu-id="c1dac-135">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="c1dac-136">api</span><span class="sxs-lookup"><span data-stu-id="c1dac-136">api</span></span> | [<span data-ttu-id="c1dac-137">apiApplication</span><span class="sxs-lookup"><span data-stu-id="c1dac-137">apiApplication</span></span>](../resources/apiapplication.md) | <span data-ttu-id="c1dac-138">指定实现 Web API 的应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="c1dac-138">Specifies settings for an application that implements a web API.</span></span> |
| <span data-ttu-id="c1dac-139">appRoles</span><span class="sxs-lookup"><span data-stu-id="c1dac-139">appRoles</span></span> | <span data-ttu-id="c1dac-140">[appRole](../resources/approle.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c1dac-140">[appRole](../resources/approle.md) collection</span></span> | <span data-ttu-id="c1dac-141">应用程序可声明的应用程序角色的集合。</span><span class="sxs-lookup"><span data-stu-id="c1dac-141">The collection of application roles that an application may declare.</span></span> <span data-ttu-id="c1dac-142">这些角色可以分配给用户、组或服务主体。</span><span class="sxs-lookup"><span data-stu-id="c1dac-142">These roles can be assigned to users, groups, or service principals.</span></span> <span data-ttu-id="c1dac-143">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="c1dac-143">Not nullable.</span></span> |
| <span data-ttu-id="c1dac-144">displayName</span><span class="sxs-lookup"><span data-stu-id="c1dac-144">displayName</span></span> | <span data-ttu-id="c1dac-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c1dac-145">String</span></span> | <span data-ttu-id="c1dac-146">应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c1dac-146">The display name for the application.</span></span> |
| <span data-ttu-id="c1dac-147">groupMembershipClaims</span><span class="sxs-lookup"><span data-stu-id="c1dac-147">groupMembershipClaims</span></span> | <span data-ttu-id="c1dac-148">String</span><span class="sxs-lookup"><span data-stu-id="c1dac-148">String</span></span> | <span data-ttu-id="c1dac-149">配置在应用程序需要的用户或 OAuth 2.0 访问令牌中颁发的**组**声明。</span><span class="sxs-lookup"><span data-stu-id="c1dac-149">Configures the **groups** claim issued in a user or OAuth 2.0 access token that the application expects.</span></span> <span data-ttu-id="c1dac-150">要设置此属性，请使用以下有效字符串值之一：</span><span class="sxs-lookup"><span data-stu-id="c1dac-150">To set this attribute, use one of the following valid string values:</span></span><ul><li>`None`</li><li><span data-ttu-id="c1dac-151">`SecurityGroup`：针对安全组和 Azure Active Directory （Azure AD）角色</span><span class="sxs-lookup"><span data-stu-id="c1dac-151">`SecurityGroup`: For security groups and Azure Active Directory (Azure AD) roles</span></span></li><li><span data-ttu-id="c1dac-152">`All`：该操作可获取登录用户所属的所有安全组、通讯组和 Azure AD 目录角色</span><span class="sxs-lookup"><span data-stu-id="c1dac-152">`All`: This will get all of the security groups, distribution groups, and Azure AD directory roles that the signed-in user is a member of</span></span></li></ul> |
| <span data-ttu-id="c1dac-153">identifierUris</span><span class="sxs-lookup"><span data-stu-id="c1dac-153">identifierUris</span></span> | <span data-ttu-id="c1dac-154">String collection</span><span class="sxs-lookup"><span data-stu-id="c1dac-154">String collection</span></span> | <span data-ttu-id="c1dac-155">URI，用于在应用程序的 Azure AD 租户中标识该应用程序；如果应用程序是多租户的，则用于在已验证的自定义域中标识该应用程序。</span><span class="sxs-lookup"><span data-stu-id="c1dac-155">The URIs that identify the application within its Azure AD tenant, or within a verified custom domain if the application is multi-tenant.</span></span> <span data-ttu-id="c1dac-156">有关详细信息，请参阅[应用程序对象和服务主体对象](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)。</span><span class="sxs-lookup"><span data-stu-id="c1dac-156">For more information, see [Application Objects and Service Principal Objects](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).</span></span> <span data-ttu-id="c1dac-157">需要多值属性筛选器表达式的 *any* 运算符。</span><span class="sxs-lookup"><span data-stu-id="c1dac-157">The *any* operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="c1dac-158">不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c1dac-158">Not nullable.</span></span> |
| <span data-ttu-id="c1dac-159">info</span><span class="sxs-lookup"><span data-stu-id="c1dac-159">info</span></span> | [<span data-ttu-id="c1dac-160">informationalUrl</span><span class="sxs-lookup"><span data-stu-id="c1dac-160">informationalUrl</span></span>](../resources/informationalurl.md) | <span data-ttu-id="c1dac-161">应用程序的基本配置文件信息，如应用程序的营销、支持、服务条款和隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="c1dac-161">Basic profile information of the application such as  app's marketing, support, terms of service, and privacy statement URLs.</span></span> <span data-ttu-id="c1dac-162">服务条款和隐私声明通过用户同意体验展示给用户。</span><span class="sxs-lookup"><span data-stu-id="c1dac-162">The terms of service and privacy statement are surfaced to users through the user consent experience.</span></span> <span data-ttu-id="c1dac-163">有关详细信息，请参阅[为已注册的 AZURE AD 应用添加服务条款和隐私声明](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement)。</span><span class="sxs-lookup"><span data-stu-id="c1dac-163">For more information, see [Add Terms of service and privacy statement for registered Azure AD apps](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement).</span></span> |
| <span data-ttu-id="c1dac-164">isFallbackPublicClient</span><span class="sxs-lookup"><span data-stu-id="c1dac-164">isFallbackPublicClient</span></span> | <span data-ttu-id="c1dac-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1dac-165">Boolean</span></span> | <span data-ttu-id="c1dac-166">将回退应用程序类型指定为公共客户端，例如在移动设备上运行的已安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="c1dac-166">Specifies the fallback application type as public client, such as an installed application running on a mobile device.</span></span> <span data-ttu-id="c1dac-167">默认值是 `false` ，这意味着回退应用程序类型是机密客户端，如 web app。</span><span class="sxs-lookup"><span data-stu-id="c1dac-167">The default value is `false`, which means the fallback application type is confidential client such as web app.</span></span> <span data-ttu-id="c1dac-168">在某些情况下，Azure AD 无法确定客户端应用程序类型（例如，在未指定重定向 URI 的情况下配置它的[ROPC](https://tools.ietf.org/html/rfc6749#section-4.3)流）。</span><span class="sxs-lookup"><span data-stu-id="c1dac-168">There are certain scenarios where Azure AD cannot determine the client application type (for example, [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) flow where it is configured without specifying a redirect URI).</span></span> <span data-ttu-id="c1dac-169">在这些情况下，Azure AD 将根据此属性的值解释应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="c1dac-169">In those cases, Azure AD will interpret the application type based on the value of this property.</span></span>|
| <span data-ttu-id="c1dac-170">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="c1dac-170">keyCredentials</span></span> | <span data-ttu-id="c1dac-171">[keyCredential](../resources/keycredential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c1dac-171">[keyCredential](../resources/keycredential.md) collection</span></span> | <span data-ttu-id="c1dac-172">与应用程序关联的密钥凭据的集合。</span><span class="sxs-lookup"><span data-stu-id="c1dac-172">The collection of key credentials associated with the application.</span></span> <span data-ttu-id="c1dac-173">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="c1dac-173">Not nullable.</span></span> |
| <span data-ttu-id="c1dac-174">logo</span><span class="sxs-lookup"><span data-stu-id="c1dac-174">logo</span></span> | <span data-ttu-id="c1dac-175">Stream</span><span class="sxs-lookup"><span data-stu-id="c1dac-175">Stream</span></span> | <span data-ttu-id="c1dac-176">应用程序的主徽标。</span><span class="sxs-lookup"><span data-stu-id="c1dac-176">The main logo for the application.</span></span> <span data-ttu-id="c1dac-177">不可为空。</span><span class="sxs-lookup"><span data-stu-id="c1dac-177">Not nullable.</span></span> |
| <span data-ttu-id="c1dac-178">optionalClaims</span><span class="sxs-lookup"><span data-stu-id="c1dac-178">optionalClaims</span></span> | <span data-ttu-id="c1dac-179">optionalClaims</span><span class="sxs-lookup"><span data-stu-id="c1dac-179">optionalClaims</span></span> | <span data-ttu-id="c1dac-180">应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以指定 Microsoft 安全令牌服务发送到他们应用程序的令牌中所需的声明。</span><span class="sxs-lookup"><span data-stu-id="c1dac-180">Application developers can configure optional claims in their Azure AD apps to specify which claims they want in tokens sent to their application by the Microsoft security token service.</span></span> <span data-ttu-id="c1dac-181">有关详细信息，请参阅[可选声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="c1dac-181">See [optional claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims) for more information.</span></span> |
| <span data-ttu-id="c1dac-182">parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="c1dac-182">parentalControlSettings</span></span> | [<span data-ttu-id="c1dac-183">parentalControlSettings</span><span class="sxs-lookup"><span data-stu-id="c1dac-183">parentalControlSettings</span></span>](../resources/parentalcontrolsettings.md) |<span data-ttu-id="c1dac-184">指定应用程序的家长控制设置。</span><span class="sxs-lookup"><span data-stu-id="c1dac-184">Specifies parental control settings for an application.</span></span> |
| <span data-ttu-id="c1dac-185">publicClient</span><span class="sxs-lookup"><span data-stu-id="c1dac-185">publicClient</span></span> | [<span data-ttu-id="c1dac-186">publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="c1dac-186">publicClientApplication</span></span>](../resources/publicclientapplication.md) | <span data-ttu-id="c1dac-187">指定已安装客户端（如台式设备或移动设备）的设置。</span><span class="sxs-lookup"><span data-stu-id="c1dac-187">Specifies settings for installed clients such as desktop or mobile devices.</span></span> |
| <span data-ttu-id="c1dac-188">requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="c1dac-188">requiredResourceAccess</span></span> |<span data-ttu-id="c1dac-189">[requiredResourceAccess](../resources/requiredresourceaccess.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c1dac-189">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span></span>|<span data-ttu-id="c1dac-190">指定此应用程序需要访问的资源以及在每个资源下所需的 OAuth 权限范围和应用程序角色集。</span><span class="sxs-lookup"><span data-stu-id="c1dac-190">Specifies resources that this application requires access to and the set of OAuth permission scopes and application roles that it needs under each of those resources.</span></span> <span data-ttu-id="c1dac-191">这种预配置的所需资源访问权限可驱动同意体验。</span><span class="sxs-lookup"><span data-stu-id="c1dac-191">This pre-configuration of required resource access drives the consent experience.</span></span> <span data-ttu-id="c1dac-192">不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c1dac-192">Not nullable.</span></span>|
| <span data-ttu-id="c1dac-193">signInAudience</span><span class="sxs-lookup"><span data-stu-id="c1dac-193">signInAudience</span></span> | <span data-ttu-id="c1dac-194">String</span><span class="sxs-lookup"><span data-stu-id="c1dac-194">String</span></span> | <span data-ttu-id="c1dac-195">指定当前应用程序支持的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="c1dac-195">Specifies what Microsoft accounts are supported for the current application.</span></span> <span data-ttu-id="c1dac-196">支持的值为：</span><span class="sxs-lookup"><span data-stu-id="c1dac-196">Supported values are:</span></span><ul><li><span data-ttu-id="c1dac-197">`AzureADMyOrg`：在我的组织的 Azure AD 租户（即单租户）中拥有 Microsoft 工作或学校帐户的用户</span><span class="sxs-lookup"><span data-stu-id="c1dac-197">`AzureADMyOrg`: Users with a Microsoft work or school account in my organization’s Azure AD tenant (i.e. single tenant)</span></span></li><li><span data-ttu-id="c1dac-198">`AzureADMultipleOrgs`：在任何组织的 Azure AD 租户（即多租户）中拥有 Microsoft 工作或学校帐户的用户</span><span class="sxs-lookup"><span data-stu-id="c1dac-198">`AzureADMultipleOrgs`: Users with a Microsoft work or school account in any organization’s Azure AD tenant (i.e. multi-tenant)</span></span></li> <li><span data-ttu-id="c1dac-199">`AzureADandPersonalMicrosoftAccount`：拥有个人 Microsoft 帐户或任意组织的 Azure AD 租户中的工作或学校帐户的用户</span><span class="sxs-lookup"><span data-stu-id="c1dac-199">`AzureADandPersonalMicrosoftAccount`: Users with a personal Microsoft account, or a work or school account in any organization’s Azure AD tenant</span></span></li></ul> | `AzureADandPersonalMicrosoftAccount` |
| <span data-ttu-id="c1dac-200">tags</span><span class="sxs-lookup"><span data-stu-id="c1dac-200">tags</span></span> |<span data-ttu-id="c1dac-201">String 集合</span><span class="sxs-lookup"><span data-stu-id="c1dac-201">String collection</span></span>| <span data-ttu-id="c1dac-202">可用于分类和标识应用程序的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="c1dac-202">Custom strings that can be used to categorize and identify the application.</span></span> <span data-ttu-id="c1dac-203">不可为空。</span><span class="sxs-lookup"><span data-stu-id="c1dac-203">Not nullable.</span></span>|
| <span data-ttu-id="c1dac-204">tokenEncryptionKeyId</span><span class="sxs-lookup"><span data-stu-id="c1dac-204">tokenEncryptionKeyId</span></span> |<span data-ttu-id="c1dac-205">String</span><span class="sxs-lookup"><span data-stu-id="c1dac-205">String</span></span>|<span data-ttu-id="c1dac-206">指定 keyCredentials 集合中的公共密钥的 keyId。</span><span class="sxs-lookup"><span data-stu-id="c1dac-206">Specifies the keyId of a public key from the keyCredentials collection.</span></span> <span data-ttu-id="c1dac-207">配置后，Azure AD 将使用此属性指向的密钥对其发出的所有令牌进行加密。</span><span class="sxs-lookup"><span data-stu-id="c1dac-207">When configured, Azure AD encrypts all the tokens it emits by using the key this property points to.</span></span> <span data-ttu-id="c1dac-208">接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。</span><span class="sxs-lookup"><span data-stu-id="c1dac-208">The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.</span></span>|
| <span data-ttu-id="c1dac-209">web</span><span class="sxs-lookup"><span data-stu-id="c1dac-209">web</span></span> |[<span data-ttu-id="c1dac-210">webApplication</span><span class="sxs-lookup"><span data-stu-id="c1dac-210">webApplication</span></span>](../resources/webapplication.md)| <span data-ttu-id="c1dac-211">指定 Web 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="c1dac-211">Specifies settings for a web application.</span></span> |

## <a name="response"></a><span data-ttu-id="c1dac-212">响应</span><span class="sxs-lookup"><span data-stu-id="c1dac-212">Response</span></span>

<span data-ttu-id="c1dac-213">如果成功，此方法将返回 `204 No Content` 响应代码，并且不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c1dac-213">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1dac-214">示例</span><span class="sxs-lookup"><span data-stu-id="c1dac-214">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1dac-215">请求</span><span class="sxs-lookup"><span data-stu-id="c1dac-215">Request</span></span>
<span data-ttu-id="c1dac-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1dac-216">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1dac-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1dac-217">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c1dac-218">C#</span><span class="sxs-lookup"><span data-stu-id="c1dac-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1dac-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1dac-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1dac-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1dac-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1dac-221">Java</span><span class="sxs-lookup"><span data-stu-id="c1dac-221">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c1dac-222">响应</span><span class="sxs-lookup"><span data-stu-id="c1dac-222">Response</span></span>

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
