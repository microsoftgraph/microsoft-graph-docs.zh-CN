---
title: 域资源类型
description: 表示与租户关联的域。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b0c86f7ae40c5858301e3febb1a8aa9963119b0f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958799"
---
# <a name="domain-resource-type"></a><span data-ttu-id="b4d41-103">域资源类型</span><span class="sxs-lookup"><span data-stu-id="b4d41-103">domain resource type</span></span>

<span data-ttu-id="b4d41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4d41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4d41-105">表示与租户关联的域。</span><span class="sxs-lookup"><span data-stu-id="b4d41-105">Represents a domain associated with the tenant.</span></span>

<span data-ttu-id="b4d41-106">使用域操作将域与租户关联、验证域所有权并配置受支持的服务。</span><span class="sxs-lookup"><span data-stu-id="b4d41-106">Use domain operations to associate domains to a tenant, verify domain ownership, and configure supported services.</span></span>  <span data-ttu-id="b4d41-107">域操作使注册机构能够自动执行 Microsoft 365 等服务的域关联。</span><span class="sxs-lookup"><span data-stu-id="b4d41-107">Domain operations enable registrars to automate domain association for services such as Microsoft 365.</span></span> <span data-ttu-id="b4d41-108">例如，作为域注册的一部分，注册机构可以启用电子邮件、网站、身份验证等的虚域。</span><span class="sxs-lookup"><span data-stu-id="b4d41-108">For example, as part of domain sign up, a registrar can enable a vanity domain for email, websites, authentication, etc.</span></span>

<span data-ttu-id="b4d41-109">将域与租户关联：</span><span class="sxs-lookup"><span data-stu-id="b4d41-109">To associate a domain with a tenant:</span></span>

1. <span data-ttu-id="b4d41-110">[将](../api/domain-post-domains.md) 域与租户关联。</span><span class="sxs-lookup"><span data-stu-id="b4d41-110">[Associate](../api/domain-post-domains.md) a domain with a tenant.</span></span>

2. <span data-ttu-id="b4d41-111">[检索](../api/domain-list-verificationdnsrecords.md) 域验证记录。</span><span class="sxs-lookup"><span data-stu-id="b4d41-111">[Retrieve](../api/domain-list-verificationdnsrecords.md) the domain verification records.</span></span> <span data-ttu-id="b4d41-112">使用域注册器或 DNS 服务器配置将验证记录详细信息添加到域的区域文件。</span><span class="sxs-lookup"><span data-stu-id="b4d41-112">Add the verification record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

3. <span data-ttu-id="b4d41-113">[验证](../api/domain-verify.md) 域的所有权。</span><span class="sxs-lookup"><span data-stu-id="b4d41-113">[Verify](../api/domain-verify.md) the ownership of the domain.</span></span> <span data-ttu-id="b4d41-114">这将验证域，将 **isVerified** 属性设置为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="b4d41-114">This will verify the domain and set the **isVerified** property to `true`.</span></span>

4. <span data-ttu-id="b4d41-115">[指示](../api/domain-update.md) 计划用于域的受支持服务。</span><span class="sxs-lookup"><span data-stu-id="b4d41-115">[Indicate](../api/domain-update.md) the supported services you plan to use with the domain.</span></span>

5. <span data-ttu-id="b4d41-116">[通过](../api/domain-list-serviceconfigurationrecords.md) 检索为域启用服务所需的记录列表来配置支持的服务。</span><span class="sxs-lookup"><span data-stu-id="b4d41-116">[Configure](../api/domain-list-serviceconfigurationrecords.md) supported services by retrieving a list of records needed to enable services for the domain.</span></span> <span data-ttu-id="b4d41-117">使用域注册机构或 DNS 服务器配置将配置记录详细信息添加到域的区域文件。</span><span class="sxs-lookup"><span data-stu-id="b4d41-117">Add the configuration record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="b4d41-118">Methods</span><span class="sxs-lookup"><span data-stu-id="b4d41-118">Methods</span></span>

| <span data-ttu-id="b4d41-119">方法</span><span class="sxs-lookup"><span data-stu-id="b4d41-119">Method</span></span>   | <span data-ttu-id="b4d41-120">返回类型</span><span class="sxs-lookup"><span data-stu-id="b4d41-120">Return Type</span></span> |<span data-ttu-id="b4d41-121">说明</span><span class="sxs-lookup"><span data-stu-id="b4d41-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b4d41-122">获取域</span><span class="sxs-lookup"><span data-stu-id="b4d41-122">Get domain</span></span>](../api/domain-get.md) | [<span data-ttu-id="b4d41-123">domain</span><span class="sxs-lookup"><span data-stu-id="b4d41-123">domain</span></span>](domain.md) | <span data-ttu-id="b4d41-124">读取 domain 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b4d41-124">Read properties and relationships of a domain object.</span></span>|
|[<span data-ttu-id="b4d41-125">创建域</span><span class="sxs-lookup"><span data-stu-id="b4d41-125">Create domain</span></span>](../api/domain-post-domains.md) | [<span data-ttu-id="b4d41-126">domain</span><span class="sxs-lookup"><span data-stu-id="b4d41-126">domain</span></span>](domain.md) | <span data-ttu-id="b4d41-127">向租户添加域。</span><span class="sxs-lookup"><span data-stu-id="b4d41-127">Adds a domain to the tenant.</span></span> |
|[<span data-ttu-id="b4d41-128">列出 domainNameReference</span><span class="sxs-lookup"><span data-stu-id="b4d41-128">List domainNameReference</span></span>](../api/domain-list-domainnamereferences.md) |<span data-ttu-id="b4d41-129">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="b4d41-129">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="b4d41-130">检索引用域的目录对象列表。</span><span class="sxs-lookup"><span data-stu-id="b4d41-130">Retrieve a list of directory objects with a reference to the domain.</span></span>|
|[<span data-ttu-id="b4d41-131">列出 serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="b4d41-131">List serviceConfigurationRecords</span></span>](../api/domain-list-serviceconfigurationrecords.md) |<span data-ttu-id="b4d41-132">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4d41-132">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="b4d41-133">检索域配置的域 DNS 记录列表。</span><span class="sxs-lookup"><span data-stu-id="b4d41-133">Retrieve a list of domain DNS records for domain configuration.</span></span>|
|[<span data-ttu-id="b4d41-134">列出 verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="b4d41-134">List verificationDnsRecords</span></span>](../api/domain-list-verificationdnsrecords.md) |<span data-ttu-id="b4d41-135">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4d41-135">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="b4d41-136">检索域 DNS 记录列表以用于域验证。</span><span class="sxs-lookup"><span data-stu-id="b4d41-136">Retrieve a list of domain DNS records for domain verification.</span></span>|
|[<span data-ttu-id="b4d41-137">更新域</span><span class="sxs-lookup"><span data-stu-id="b4d41-137">Update domain</span></span>](../api/domain-update.md) | [<span data-ttu-id="b4d41-138">domain</span><span class="sxs-lookup"><span data-stu-id="b4d41-138">domain</span></span>](domain.md) |<span data-ttu-id="b4d41-139">更新域。</span><span class="sxs-lookup"><span data-stu-id="b4d41-139">Updates a domain.</span></span>|
|[<span data-ttu-id="b4d41-140">删除域</span><span class="sxs-lookup"><span data-stu-id="b4d41-140">Delete domain</span></span>](../api/domain-delete.md) | <span data-ttu-id="b4d41-141">无</span><span class="sxs-lookup"><span data-stu-id="b4d41-141">None</span></span> |<span data-ttu-id="b4d41-142">删除域。</span><span class="sxs-lookup"><span data-stu-id="b4d41-142">Deletes a domain.</span></span>|
|[<span data-ttu-id="b4d41-143">ForceDelete 域</span><span class="sxs-lookup"><span data-stu-id="b4d41-143">ForceDelete domain</span></span>](../api/domain-forcedelete.md)|<span data-ttu-id="b4d41-144">无</span><span class="sxs-lookup"><span data-stu-id="b4d41-144">None</span></span>|<span data-ttu-id="b4d41-145">使用异步操作删除域。</span><span class="sxs-lookup"><span data-stu-id="b4d41-145">Deletes a domain using an asynchronous operation.</span></span>|
|[<span data-ttu-id="b4d41-146">验证域</span><span class="sxs-lookup"><span data-stu-id="b4d41-146">Verify domain</span></span>](../api/domain-verify.md)|[<span data-ttu-id="b4d41-147">domain</span><span class="sxs-lookup"><span data-stu-id="b4d41-147">domain</span></span>](domain.md)|<span data-ttu-id="b4d41-148">验证域的所有权。</span><span class="sxs-lookup"><span data-stu-id="b4d41-148">Validates the ownership of the domain.</span></span>|

## <a name="properties"></a><span data-ttu-id="b4d41-149">属性</span><span class="sxs-lookup"><span data-stu-id="b4d41-149">Properties</span></span>

| <span data-ttu-id="b4d41-150">属性</span><span class="sxs-lookup"><span data-stu-id="b4d41-150">Property</span></span>   | <span data-ttu-id="b4d41-151">类型</span><span class="sxs-lookup"><span data-stu-id="b4d41-151">Type</span></span> | <span data-ttu-id="b4d41-152">说明</span><span class="sxs-lookup"><span data-stu-id="b4d41-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b4d41-153">authenticationType</span><span class="sxs-lookup"><span data-stu-id="b4d41-153">authenticationType</span></span>|<span data-ttu-id="b4d41-154">String</span><span class="sxs-lookup"><span data-stu-id="b4d41-154">String</span></span>| <span data-ttu-id="b4d41-155">指示域的已配置的身份验证类型。</span><span class="sxs-lookup"><span data-stu-id="b4d41-155">Indicates the configured authentication type for the domain.</span></span> <span data-ttu-id="b4d41-156">值为 或 `Managed` `Federated` 。</span><span class="sxs-lookup"><span data-stu-id="b4d41-156">The value is either `Managed` or `Federated`.</span></span> <span data-ttu-id="b4d41-157">`Managed` 指示 Azure AD 执行用户身份验证的云托管域。</span><span class="sxs-lookup"><span data-stu-id="b4d41-157">`Managed` indicates a cloud managed domain where Azure AD performs user authentication.</span></span> <span data-ttu-id="b4d41-158">`Federated` 指示通过 Active Directory 联合身份验证服务与标识提供程序（如租户本地 Active Directory）联合身份验证。</span><span class="sxs-lookup"><span data-stu-id="b4d41-158">`Federated` indicates authentication is federated with an identity provider such as the tenant's on-premises Active Directory via Active Directory Federation Services.</span></span> <span data-ttu-id="b4d41-159">此属性是只读的，并且不可为 null。</span><span class="sxs-lookup"><span data-stu-id="b4d41-159">This property is read-only and is not nullable.</span></span> |
|<span data-ttu-id="b4d41-160">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="b4d41-160">availabilityStatus</span></span>|<span data-ttu-id="b4d41-161">String</span><span class="sxs-lookup"><span data-stu-id="b4d41-161">String</span></span>| <span data-ttu-id="b4d41-162">此属性始终在使用 `null` verify 操作[](../api/domain-verify.md)时除外。</span><span class="sxs-lookup"><span data-stu-id="b4d41-162">This property is always `null` except when the [verify](../api/domain-verify.md) action is used.</span></span> <span data-ttu-id="b4d41-163">使用 [verify](../api/domain-verify.md) 操作 **时，响应** 中将返回一个域实体。</span><span class="sxs-lookup"><span data-stu-id="b4d41-163">When the [verify](../api/domain-verify.md) action is used, a **domain** entity is returned in the response.</span></span> <span data-ttu-id="b4d41-164">响应中 **domain** 实体的 **availabilityStatus** 属性是 `AvailableImmediately` 或 `EmailVerifiedDomainTakeoverScheduled` 。</span><span class="sxs-lookup"><span data-stu-id="b4d41-164">The **availabilityStatus** property of the **domain** entity in the response is either `AvailableImmediately` or `EmailVerifiedDomainTakeoverScheduled`.</span></span>|
|<span data-ttu-id="b4d41-165">id</span><span class="sxs-lookup"><span data-stu-id="b4d41-165">id</span></span>|<span data-ttu-id="b4d41-166">String</span><span class="sxs-lookup"><span data-stu-id="b4d41-166">String</span></span>| <span data-ttu-id="b4d41-167">域的完全限定名称。</span><span class="sxs-lookup"><span data-stu-id="b4d41-167">The fully qualified name of the domain.</span></span> <span data-ttu-id="b4d41-168">键、不可变、不可为 null、唯一。</span><span class="sxs-lookup"><span data-stu-id="b4d41-168">Key, immutable, not nullable, unique.</span></span> |
|<span data-ttu-id="b4d41-169">isAdminManaged</span><span class="sxs-lookup"><span data-stu-id="b4d41-169">isAdminManaged</span></span>|<span data-ttu-id="b4d41-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4d41-170">Boolean</span></span>| <span data-ttu-id="b4d41-171">如果域的 DNS 记录管理已委派给 `false` Microsoft 365，则属性的值为 。</span><span class="sxs-lookup"><span data-stu-id="b4d41-171">The value of the property is `false` if the DNS record management of the domain has been delegated to Microsoft 365.</span></span> <span data-ttu-id="b4d41-172">否则，值为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="b4d41-172">Otherwise, the value is `true`.</span></span> <span data-ttu-id="b4d41-173">不可为 null</span><span class="sxs-lookup"><span data-stu-id="b4d41-173">Not nullable</span></span> |
|<span data-ttu-id="b4d41-174">isDefault</span><span class="sxs-lookup"><span data-stu-id="b4d41-174">isDefault</span></span>|<span data-ttu-id="b4d41-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4d41-175">Boolean</span></span>| <span data-ttu-id="b4d41-176">`true` 如果这是用于用户创建的默认域。</span><span class="sxs-lookup"><span data-stu-id="b4d41-176">`true` if this is the default domain that is used for user creation.</span></span> <span data-ttu-id="b4d41-177">每个公司只有一个默认域。</span><span class="sxs-lookup"><span data-stu-id="b4d41-177">There is only one default domain per company.</span></span> <span data-ttu-id="b4d41-178">不可为 null</span><span class="sxs-lookup"><span data-stu-id="b4d41-178">Not nullable</span></span> |
|<span data-ttu-id="b4d41-179">isInitial</span><span class="sxs-lookup"><span data-stu-id="b4d41-179">isInitial</span></span>|<span data-ttu-id="b4d41-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4d41-180">Boolean</span></span>| <span data-ttu-id="b4d41-181">`true` 如果这是由用户创建的初始Microsoft Online Services (companyname.onmicrosoft.com) 。</span><span class="sxs-lookup"><span data-stu-id="b4d41-181">`true` if this is the initial domain created by Microsoft Online Services (companyname.onmicrosoft.com).</span></span> <span data-ttu-id="b4d41-182">每个公司只有一个初始域。</span><span class="sxs-lookup"><span data-stu-id="b4d41-182">There is only one initial domain per company.</span></span> <span data-ttu-id="b4d41-183">不可为 null</span><span class="sxs-lookup"><span data-stu-id="b4d41-183">Not nullable</span></span> |
|<span data-ttu-id="b4d41-184">isRoot</span><span class="sxs-lookup"><span data-stu-id="b4d41-184">isRoot</span></span>|<span data-ttu-id="b4d41-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4d41-185">Boolean</span></span>| <span data-ttu-id="b4d41-186">`true` 如果域是已验证的根域。</span><span class="sxs-lookup"><span data-stu-id="b4d41-186">`true` if the domain is a verified root domain.</span></span> <span data-ttu-id="b4d41-187">否则 `false` ，如果域是子域或未经验证。</span><span class="sxs-lookup"><span data-stu-id="b4d41-187">Otherwise, `false` if the domain is a subdomain or unverified.</span></span> <span data-ttu-id="b4d41-188">不可为 null</span><span class="sxs-lookup"><span data-stu-id="b4d41-188">Not nullable</span></span> |
|<span data-ttu-id="b4d41-189">isVerified</span><span class="sxs-lookup"><span data-stu-id="b4d41-189">isVerified</span></span>|<span data-ttu-id="b4d41-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4d41-190">Boolean</span></span>| <span data-ttu-id="b4d41-191">`true` 如果域已完成域所有权验证。</span><span class="sxs-lookup"><span data-stu-id="b4d41-191">`true` if the domain has completed domain ownership verification.</span></span> <span data-ttu-id="b4d41-192">不可为 null</span><span class="sxs-lookup"><span data-stu-id="b4d41-192">Not nullable</span></span> |
|<span data-ttu-id="b4d41-193">passwordNotificationWindowInDays</span><span class="sxs-lookup"><span data-stu-id="b4d41-193">passwordNotificationWindowInDays</span></span>|<span data-ttu-id="b4d41-194">Int32</span><span class="sxs-lookup"><span data-stu-id="b4d41-194">Int32</span></span>|<span data-ttu-id="b4d41-195">指定用户收到其密码将过期的通知前的天数。</span><span class="sxs-lookup"><span data-stu-id="b4d41-195">Specifies the number of days before a user receives notification that their password will expire.</span></span> <span data-ttu-id="b4d41-196">如果未设置该属性，则使用默认值 14 天。</span><span class="sxs-lookup"><span data-stu-id="b4d41-196">If the property is not set, a default value of 14 days will be used.</span></span>|
|<span data-ttu-id="b4d41-197">passwordValidityPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="b4d41-197">passwordValidityPeriodInDays</span></span>|<span data-ttu-id="b4d41-198">Int32</span><span class="sxs-lookup"><span data-stu-id="b4d41-198">Int32</span></span>| <span data-ttu-id="b4d41-199">指定密码在必须更改之前的有效时间长度。</span><span class="sxs-lookup"><span data-stu-id="b4d41-199">Specifies the length of time that a password is valid before it must be changed.</span></span> <span data-ttu-id="b4d41-200">如果未设置该属性，则使用默认值 90 天。</span><span class="sxs-lookup"><span data-stu-id="b4d41-200">If the property is not set, a default value of 90 days will be used.</span></span> |
|<span data-ttu-id="b4d41-201">supportedServices</span><span class="sxs-lookup"><span data-stu-id="b4d41-201">supportedServices</span></span>|<span data-ttu-id="b4d41-202">String collection</span><span class="sxs-lookup"><span data-stu-id="b4d41-202">String collection</span></span>| <span data-ttu-id="b4d41-203">分配给域的功能。</span><span class="sxs-lookup"><span data-stu-id="b4d41-203">The capabilities assigned to the domain.</span></span> <span data-ttu-id="b4d41-204">可以包含 `0` 、 `1` 或更多以下值： `Email` 、 、 、 、 、 、 、 `Sharepoint` `EmailInternalRelayOnly` `OfficeCommunicationsOnline` `SharePointDefaultDomain` `FullRedelegation` `SharePointPublic` `OrgIdAuthentication` `Yammer` `Intune` 。</span><span class="sxs-lookup"><span data-stu-id="b4d41-204">Can include `0`, `1` or more of following values: `Email`, `Sharepoint`, `EmailInternalRelayOnly`, `OfficeCommunicationsOnline`,`SharePointDefaultDomain`, `FullRedelegation`, `SharePointPublic`, `OrgIdAuthentication`, `Yammer`, `Intune`.</span></span> <span data-ttu-id="b4d41-205">可以使用 Graph API 添加/删除的值包括 `Email` `OfficeCommunicationsOnline` ：、、。 `Yammer`</span><span class="sxs-lookup"><span data-stu-id="b4d41-205">The values which you can add/remove using Graph API include: `Email`, `OfficeCommunicationsOnline`, `Yammer`.</span></span> <span data-ttu-id="b4d41-206">不可为 null</span><span class="sxs-lookup"><span data-stu-id="b4d41-206">Not nullable</span></span>|
|<span data-ttu-id="b4d41-207">state</span><span class="sxs-lookup"><span data-stu-id="b4d41-207">state</span></span>|[<span data-ttu-id="b4d41-208">domainState</span><span class="sxs-lookup"><span data-stu-id="b4d41-208">domainState</span></span>](domainstate.md)| <span data-ttu-id="b4d41-209">为域安排的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="b4d41-209">Status of asynchronous operations scheduled for the domain.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b4d41-210">关系</span><span class="sxs-lookup"><span data-stu-id="b4d41-210">Relationships</span></span>

<span data-ttu-id="b4d41-211">域与目录中的其他对象（如其验证记录和服务配置记录）之间的关系通过导航属性公开。</span><span class="sxs-lookup"><span data-stu-id="b4d41-211">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties.</span></span> <span data-ttu-id="b4d41-212">可以通过在请求中定位这些导航属性来读取这些关系。</span><span class="sxs-lookup"><span data-stu-id="b4d41-212">You can read these relationships by targeting these navigation properties in your requests.</span></span>

| <span data-ttu-id="b4d41-213">关系</span><span class="sxs-lookup"><span data-stu-id="b4d41-213">Relationship</span></span> | <span data-ttu-id="b4d41-214">类型</span><span class="sxs-lookup"><span data-stu-id="b4d41-214">Type</span></span> |<span data-ttu-id="b4d41-215">说明</span><span class="sxs-lookup"><span data-stu-id="b4d41-215">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4d41-216">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="b4d41-216">domainNameReferences</span></span>|<span data-ttu-id="b4d41-217">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="b4d41-217">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="b4d41-218">只读，可为空</span><span class="sxs-lookup"><span data-stu-id="b4d41-218">Read-only, Nullable</span></span>|
|<span data-ttu-id="b4d41-219">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="b4d41-219">serviceConfigurationRecords</span></span>|<span data-ttu-id="b4d41-220">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4d41-220">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="b4d41-221">在 Microsoft Online Services 使用域之前，客户添加到域的 DNS 区域文件的 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="b4d41-221">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span> <span data-ttu-id="b4d41-222">只读，可为空</span><span class="sxs-lookup"><span data-stu-id="b4d41-222">Read-only, Nullable</span></span> |
|<span data-ttu-id="b4d41-223">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="b4d41-223">verificationDnsRecords</span></span>|<span data-ttu-id="b4d41-224">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4d41-224">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="b4d41-225">客户添加到域的 DNS 区域文件的 DNS 记录，客户可以使用 Azure AD 完成域所有权验证。</span><span class="sxs-lookup"><span data-stu-id="b4d41-225">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span> <span data-ttu-id="b4d41-226">只读，可为空</span><span class="sxs-lookup"><span data-stu-id="b4d41-226">Read-only, Nullable</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4d41-227">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4d41-227">JSON representation</span></span>
<span data-ttu-id="b4d41-228">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4d41-228">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "passwordNotificationWindowInDays": 14,
  "passwordValidityPeriodInDays": 90,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


