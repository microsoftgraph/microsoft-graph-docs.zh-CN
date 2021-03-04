---
title: 域资源类型
description: 表示与租户关联的域。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d22df53e3d274601d58f17cbbf859de47ae3d1f9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440400"
---
# <a name="domain-resource-type"></a><span data-ttu-id="9cc15-103">域资源类型</span><span class="sxs-lookup"><span data-stu-id="9cc15-103">domain resource type</span></span>

<span data-ttu-id="9cc15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cc15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cc15-105">表示与租户关联的域。</span><span class="sxs-lookup"><span data-stu-id="9cc15-105">Represents a domain associated with the tenant.</span></span>

<span data-ttu-id="9cc15-106">使用域操作将域与租户关联、验证域所有权并配置受支持的服务。</span><span class="sxs-lookup"><span data-stu-id="9cc15-106">Use domain operations to associate domains to a tenant, verify domain ownership, and configure supported services.</span></span>  <span data-ttu-id="9cc15-107">域操作使注册机构能够自动执行 Microsoft 365 等服务的域关联。</span><span class="sxs-lookup"><span data-stu-id="9cc15-107">Domain operations enable registrars to automate domain association for services such as Microsoft 365.</span></span> <span data-ttu-id="9cc15-108">例如，作为域注册的一部分，注册机构可以启用电子邮件、网站、身份验证等虚域。</span><span class="sxs-lookup"><span data-stu-id="9cc15-108">For example, as part of domain sign up, a registrar can enable a vanity domain for email, websites, authentication, etc.</span></span>

<span data-ttu-id="9cc15-109">若要将域与租户关联，</span><span class="sxs-lookup"><span data-stu-id="9cc15-109">To associate a domain with a tenant:</span></span>

1. <span data-ttu-id="9cc15-110">[将](../api/domain-post-domains.md) 域与租户关联。</span><span class="sxs-lookup"><span data-stu-id="9cc15-110">[Associate](../api/domain-post-domains.md) a domain with a tenant.</span></span>

2. <span data-ttu-id="9cc15-111">[检索](../api/domain-list-verificationdnsrecords.md) 域验证记录。</span><span class="sxs-lookup"><span data-stu-id="9cc15-111">[Retrieve](../api/domain-list-verificationdnsrecords.md) the domain verification records.</span></span> <span data-ttu-id="9cc15-112">使用域注册器或 DNS 服务器配置将验证记录详细信息添加到域的区域文件。</span><span class="sxs-lookup"><span data-stu-id="9cc15-112">Add the verification record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

3. <span data-ttu-id="9cc15-113">[验证](../api/domain-verify.md) 域的所有权。</span><span class="sxs-lookup"><span data-stu-id="9cc15-113">[Verify](../api/domain-verify.md) the ownership of the domain.</span></span> <span data-ttu-id="9cc15-114">这将验证域，将 *isVerified* 属性设置为 *true。*</span><span class="sxs-lookup"><span data-stu-id="9cc15-114">This will verify the domain and set the *isVerified* property to *true*.</span></span>

4. <span data-ttu-id="9cc15-115">[指示](../api/domain-update.md) 计划用于域的受支持服务。</span><span class="sxs-lookup"><span data-stu-id="9cc15-115">[Indicate](../api/domain-update.md) the supported services you plan to use with the domain.</span></span>

5. <span data-ttu-id="9cc15-116">[通过](../api/domain-list-serviceconfigurationrecords.md) 检索为域启用服务所需的记录列表来配置支持的服务。</span><span class="sxs-lookup"><span data-stu-id="9cc15-116">[Configure](../api/domain-list-serviceconfigurationrecords.md) supported services by retrieving a list of records needed to enable services for the domain.</span></span> <span data-ttu-id="9cc15-117">使用域注册器或 DNS 服务器配置将配置记录详细信息添加到域的区域文件。</span><span class="sxs-lookup"><span data-stu-id="9cc15-117">Add the configuration record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="9cc15-118">Methods</span><span class="sxs-lookup"><span data-stu-id="9cc15-118">Methods</span></span>

| <span data-ttu-id="9cc15-119">方法</span><span class="sxs-lookup"><span data-stu-id="9cc15-119">Method</span></span>   | <span data-ttu-id="9cc15-120">返回类型</span><span class="sxs-lookup"><span data-stu-id="9cc15-120">Return Type</span></span> |<span data-ttu-id="9cc15-121">说明</span><span class="sxs-lookup"><span data-stu-id="9cc15-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9cc15-122">获取域</span><span class="sxs-lookup"><span data-stu-id="9cc15-122">Get domain</span></span>](../api/domain-get.md) | [<span data-ttu-id="9cc15-123">domain</span><span class="sxs-lookup"><span data-stu-id="9cc15-123">domain</span></span>](domain.md) | <span data-ttu-id="9cc15-124">读取域对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9cc15-124">Read properties and relationships of a domain object.</span></span>|
|[<span data-ttu-id="9cc15-125">创建域</span><span class="sxs-lookup"><span data-stu-id="9cc15-125">Create domain</span></span>](../api/domain-post-domains.md) | [<span data-ttu-id="9cc15-126">domain</span><span class="sxs-lookup"><span data-stu-id="9cc15-126">domain</span></span>](domain.md) | <span data-ttu-id="9cc15-127">向租户添加域。</span><span class="sxs-lookup"><span data-stu-id="9cc15-127">Adds a domain to the tenant.</span></span> |
|[<span data-ttu-id="9cc15-128">列出 domainNameReference</span><span class="sxs-lookup"><span data-stu-id="9cc15-128">List domainNameReference</span></span>](../api/domain-list-domainnamereferences.md) |<span data-ttu-id="9cc15-129">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9cc15-129">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9cc15-130">检索引用域的目录对象列表。</span><span class="sxs-lookup"><span data-stu-id="9cc15-130">Retrieve a list of directory objects with a reference to the domain.</span></span>|
|[<span data-ttu-id="9cc15-131">列出 serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="9cc15-131">List serviceConfigurationRecords</span></span>](../api/domain-list-serviceconfigurationrecords.md) |<span data-ttu-id="9cc15-132">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9cc15-132">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="9cc15-133">检索域配置的域 DNS 记录列表。</span><span class="sxs-lookup"><span data-stu-id="9cc15-133">Retrieve a list of domain DNS records for domain configuration.</span></span>|
|[<span data-ttu-id="9cc15-134">列出 verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="9cc15-134">List verificationDnsRecords</span></span>](../api/domain-list-verificationdnsrecords.md) |<span data-ttu-id="9cc15-135">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9cc15-135">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="9cc15-136">检索域 DNS 记录列表进行域验证。</span><span class="sxs-lookup"><span data-stu-id="9cc15-136">Retrieve a list of domain DNS records for domain verification.</span></span>|
|[<span data-ttu-id="9cc15-137">更新域</span><span class="sxs-lookup"><span data-stu-id="9cc15-137">Update domain</span></span>](../api/domain-update.md) | [<span data-ttu-id="9cc15-138">domain</span><span class="sxs-lookup"><span data-stu-id="9cc15-138">domain</span></span>](domain.md) |<span data-ttu-id="9cc15-139">更新域。</span><span class="sxs-lookup"><span data-stu-id="9cc15-139">Updates a domain.</span></span>|
|[<span data-ttu-id="9cc15-140">删除域</span><span class="sxs-lookup"><span data-stu-id="9cc15-140">Delete domain</span></span>](../api/domain-delete.md) | <span data-ttu-id="9cc15-141">无</span><span class="sxs-lookup"><span data-stu-id="9cc15-141">None</span></span> |<span data-ttu-id="9cc15-142">删除域。</span><span class="sxs-lookup"><span data-stu-id="9cc15-142">Deletes a domain.</span></span>|
|[<span data-ttu-id="9cc15-143">ForceDelete 域</span><span class="sxs-lookup"><span data-stu-id="9cc15-143">ForceDelete domain</span></span>](../api/domain-forcedelete.md)|<span data-ttu-id="9cc15-144">无</span><span class="sxs-lookup"><span data-stu-id="9cc15-144">None</span></span>|<span data-ttu-id="9cc15-145">使用异步操作删除域。</span><span class="sxs-lookup"><span data-stu-id="9cc15-145">Deletes a domain using an asynchronous operation.</span></span>|
|[<span data-ttu-id="9cc15-146">验证域</span><span class="sxs-lookup"><span data-stu-id="9cc15-146">Verify domain</span></span>](../api/domain-verify.md)|[<span data-ttu-id="9cc15-147">domain</span><span class="sxs-lookup"><span data-stu-id="9cc15-147">domain</span></span>](domain.md)|<span data-ttu-id="9cc15-148">验证域的所有权。</span><span class="sxs-lookup"><span data-stu-id="9cc15-148">Validates the ownership of the domain.</span></span>|

## <a name="properties"></a><span data-ttu-id="9cc15-149">属性</span><span class="sxs-lookup"><span data-stu-id="9cc15-149">Properties</span></span>

| <span data-ttu-id="9cc15-150">属性</span><span class="sxs-lookup"><span data-stu-id="9cc15-150">Property</span></span>   | <span data-ttu-id="9cc15-151">类型</span><span class="sxs-lookup"><span data-stu-id="9cc15-151">Type</span></span> | <span data-ttu-id="9cc15-152">说明</span><span class="sxs-lookup"><span data-stu-id="9cc15-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9cc15-153">authenticationType</span><span class="sxs-lookup"><span data-stu-id="9cc15-153">authenticationType</span></span>|<span data-ttu-id="9cc15-154">String</span><span class="sxs-lookup"><span data-stu-id="9cc15-154">String</span></span>| <span data-ttu-id="9cc15-155">指示域配置的身份验证类型。</span><span class="sxs-lookup"><span data-stu-id="9cc15-155">Indicates the configured authentication type for the domain.</span></span> <span data-ttu-id="9cc15-156">值为 *托管值或\*\*联合值*。</span><span class="sxs-lookup"><span data-stu-id="9cc15-156">The value is either *Managed* or *Federated*.</span></span><br> <span data-ttu-id="9cc15-157">*托管* 表示 Azure AD 执行用户身份验证的云托管域。</span><span class="sxs-lookup"><span data-stu-id="9cc15-157">*Managed* indicates a cloud managed domain where Azure AD performs user authentication.</span></span><br><span data-ttu-id="9cc15-158">*联合* 表示身份验证通过 Active Directory 联合身份验证服务与标识提供程序（如租户本地 Active Directory）联合。</span><span class="sxs-lookup"><span data-stu-id="9cc15-158">*Federated* indicates authentication is federated with an identity provider such as the tenant's on-premises Active Directory via Active Directory Federation Services.</span></span> <span data-ttu-id="9cc15-159">此参数为只读，不可为 null。</span><span class="sxs-lookup"><span data-stu-id="9cc15-159">This propert is read-only and is not nullable.</span></span> |
|<span data-ttu-id="9cc15-160">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="9cc15-160">availabilityStatus</span></span>|<span data-ttu-id="9cc15-161">String</span><span class="sxs-lookup"><span data-stu-id="9cc15-161">String</span></span>| <span data-ttu-id="9cc15-162">此属性始终为 null，除非使用 [验证](../api/domain-verify.md) 操作。</span><span class="sxs-lookup"><span data-stu-id="9cc15-162">This property is always null except when the [verify](../api/domain-verify.md) action is used.</span></span> <span data-ttu-id="9cc15-163">使用 [验证](../api/domain-verify.md) 操作时 **，响应中** 返回域实体。</span><span class="sxs-lookup"><span data-stu-id="9cc15-163">When the [verify](../api/domain-verify.md) action is used, a **domain** entity is returned in the response.</span></span> <span data-ttu-id="9cc15-164">**响应中域实体的 availabilityStatus** 属性是 *AvailableImmediately* 或 *EmailVerifiedDomainScheduleoverScheduled*。 </span><span class="sxs-lookup"><span data-stu-id="9cc15-164">The **availabilityStatus** property of the **domain** entity in the response is either *AvailableImmediately* or *EmailVerifiedDomainTakeoverScheduled*.</span></span>|
|<span data-ttu-id="9cc15-165">id</span><span class="sxs-lookup"><span data-stu-id="9cc15-165">id</span></span>|<span data-ttu-id="9cc15-166">String</span><span class="sxs-lookup"><span data-stu-id="9cc15-166">String</span></span>| <span data-ttu-id="9cc15-167">域的完全限定名称。</span><span class="sxs-lookup"><span data-stu-id="9cc15-167">The fully qualified name of the domain.</span></span> <span data-ttu-id="9cc15-168">键、不可变、不可为空、唯一</span><span class="sxs-lookup"><span data-stu-id="9cc15-168">Key, immutable, not nullable, unique</span></span> |
|<span data-ttu-id="9cc15-169">isAdminManaged</span><span class="sxs-lookup"><span data-stu-id="9cc15-169">isAdminManaged</span></span>|<span data-ttu-id="9cc15-170">布尔</span><span class="sxs-lookup"><span data-stu-id="9cc15-170">Boolean</span></span>| <span data-ttu-id="9cc15-171">如果域的 DNS 记录管理已委派给 Microsoft 365，则属性值为 false。</span><span class="sxs-lookup"><span data-stu-id="9cc15-171">The value of the property is false if the DNS record management of the domain has been delegated to Microsoft 365.</span></span> <span data-ttu-id="9cc15-172">否则，值为 true。</span><span class="sxs-lookup"><span data-stu-id="9cc15-172">Otherwise, the value is true.</span></span> <span data-ttu-id="9cc15-173">不可为 null</span><span class="sxs-lookup"><span data-stu-id="9cc15-173">Not nullable</span></span> |
|<span data-ttu-id="9cc15-174">isDefault</span><span class="sxs-lookup"><span data-stu-id="9cc15-174">isDefault</span></span>|<span data-ttu-id="9cc15-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cc15-175">Boolean</span></span>| <span data-ttu-id="9cc15-176">如果这是用于用户创建的默认域，则其值为 True。</span><span class="sxs-lookup"><span data-stu-id="9cc15-176">True if this is the default domain that is used for user creation.</span></span> <span data-ttu-id="9cc15-177">每个公司只有一个默认域。</span><span class="sxs-lookup"><span data-stu-id="9cc15-177">There is only one default domain per company.</span></span> <span data-ttu-id="9cc15-178">不可为 null</span><span class="sxs-lookup"><span data-stu-id="9cc15-178">Not nullable</span></span> |
|<span data-ttu-id="9cc15-179">isInitial</span><span class="sxs-lookup"><span data-stu-id="9cc15-179">isInitial</span></span>|<span data-ttu-id="9cc15-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cc15-180">Boolean</span></span>| <span data-ttu-id="9cc15-181">如果这是由用户创建的初始域，Microsoft Online Services (companyname.onmicrosoft.com) 。</span><span class="sxs-lookup"><span data-stu-id="9cc15-181">True if this is the initial domain created by Microsoft Online Services (companyname.onmicrosoft.com).</span></span> <span data-ttu-id="9cc15-182">每个公司只有一个初始域。</span><span class="sxs-lookup"><span data-stu-id="9cc15-182">There is only one initial domain per company.</span></span> <span data-ttu-id="9cc15-183">不可为 null</span><span class="sxs-lookup"><span data-stu-id="9cc15-183">Not nullable</span></span> |
|<span data-ttu-id="9cc15-184">isRoot</span><span class="sxs-lookup"><span data-stu-id="9cc15-184">isRoot</span></span>|<span data-ttu-id="9cc15-185">布尔</span><span class="sxs-lookup"><span data-stu-id="9cc15-185">Boolean</span></span>| <span data-ttu-id="9cc15-186">如果域是已验证的根域，则其为 True。</span><span class="sxs-lookup"><span data-stu-id="9cc15-186">True if the domain is a verified root domain.</span></span> <span data-ttu-id="9cc15-187">否则，如果域是子域或未经验证，则其为 false。</span><span class="sxs-lookup"><span data-stu-id="9cc15-187">Otherwise, false if the domain is a subdomain or unverified.</span></span> <span data-ttu-id="9cc15-188">不可为 null</span><span class="sxs-lookup"><span data-stu-id="9cc15-188">Not nullable</span></span> |
|<span data-ttu-id="9cc15-189">isVerified</span><span class="sxs-lookup"><span data-stu-id="9cc15-189">isVerified</span></span>|<span data-ttu-id="9cc15-190">布尔</span><span class="sxs-lookup"><span data-stu-id="9cc15-190">Boolean</span></span>| <span data-ttu-id="9cc15-191">如此 如果域已完成域所有权验证。</span><span class="sxs-lookup"><span data-stu-id="9cc15-191">True if the domain has completed domain ownership verification.</span></span> <span data-ttu-id="9cc15-192">不可为 null</span><span class="sxs-lookup"><span data-stu-id="9cc15-192">Not nullable</span></span> |
|<span data-ttu-id="9cc15-193">passwordNotificationWindowInDays</span><span class="sxs-lookup"><span data-stu-id="9cc15-193">passwordNotificationWindowInDays</span></span>|<span data-ttu-id="9cc15-194">Int32</span><span class="sxs-lookup"><span data-stu-id="9cc15-194">Int32</span></span>|<span data-ttu-id="9cc15-195">指定用户收到密码过期通知前的天数。</span><span class="sxs-lookup"><span data-stu-id="9cc15-195">Specifies the number of days before a user receives notification that their password will expire.</span></span> <span data-ttu-id="9cc15-196">如果未设置该属性，则使用默认值 14 天。</span><span class="sxs-lookup"><span data-stu-id="9cc15-196">If the property is not set, a default value of 14 days will be used.</span></span>|
|<span data-ttu-id="9cc15-197">passwordValidityPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="9cc15-197">passwordValidityPeriodInDays</span></span>|<span data-ttu-id="9cc15-198">Int32</span><span class="sxs-lookup"><span data-stu-id="9cc15-198">Int32</span></span>| <span data-ttu-id="9cc15-199">指定密码在必须更改之前的有效时间长度。</span><span class="sxs-lookup"><span data-stu-id="9cc15-199">Specifies the length of time that a password is valid before it must be changed.</span></span> <span data-ttu-id="9cc15-200">如果未设置该属性，则使用默认值 90 天。</span><span class="sxs-lookup"><span data-stu-id="9cc15-200">If the property is not set, a default value of 90 days will be used.</span></span> |
|<span data-ttu-id="9cc15-201">supportedServices</span><span class="sxs-lookup"><span data-stu-id="9cc15-201">supportedServices</span></span>|<span data-ttu-id="9cc15-202">字符串集合</span><span class="sxs-lookup"><span data-stu-id="9cc15-202">String collection</span></span>| <span data-ttu-id="9cc15-203">分配给域的功能。</span><span class="sxs-lookup"><span data-stu-id="9cc15-203">The capabilities assigned to the domain.</span></span><br><br><span data-ttu-id="9cc15-204">可以包含 0、1 个或多个以下值：Email、Sharepoint、EmailInternalRelayOnly、OfficeCommunicationsOnline、SharePointDefaultDomain、FullRedelegation、SharePointPublic、OrgIdAuthentication、Yammer、Intune          </span><span class="sxs-lookup"><span data-stu-id="9cc15-204">Can include 0, 1 or more of following values: *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span><br><br> <span data-ttu-id="9cc15-205">可以使用 Graph API 添加/删除的值包括 *：Email、OfficeCommunicationsOnline、Yammer*  </span><span class="sxs-lookup"><span data-stu-id="9cc15-205">The values which you can add/remove using Graph API include: *Email*, *OfficeCommunicationsOnline*, *Yammer*</span></span><br><span data-ttu-id="9cc15-206">不可为 null</span><span class="sxs-lookup"><span data-stu-id="9cc15-206">Not nullable</span></span>|
|<span data-ttu-id="9cc15-207">state</span><span class="sxs-lookup"><span data-stu-id="9cc15-207">state</span></span>|[<span data-ttu-id="9cc15-208">domainState</span><span class="sxs-lookup"><span data-stu-id="9cc15-208">domainState</span></span>](domainstate.md)| <span data-ttu-id="9cc15-209">为域安排的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="9cc15-209">Status of asynchronous operations scheduled for the domain.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9cc15-210">关系</span><span class="sxs-lookup"><span data-stu-id="9cc15-210">Relationships</span></span>

<span data-ttu-id="9cc15-211">域与目录中的其他对象（如其验证记录和服务配置记录）之间的关系通过导航属性公开。</span><span class="sxs-lookup"><span data-stu-id="9cc15-211">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties.</span></span> <span data-ttu-id="9cc15-212">可以通过在请求中定位这些导航属性来读取这些关系。</span><span class="sxs-lookup"><span data-stu-id="9cc15-212">You can read these relationships by targeting these navigation properties in your requests.</span></span>

| <span data-ttu-id="9cc15-213">关系</span><span class="sxs-lookup"><span data-stu-id="9cc15-213">Relationship</span></span> | <span data-ttu-id="9cc15-214">类型</span><span class="sxs-lookup"><span data-stu-id="9cc15-214">Type</span></span> |<span data-ttu-id="9cc15-215">说明</span><span class="sxs-lookup"><span data-stu-id="9cc15-215">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cc15-216">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="9cc15-216">domainNameReferences</span></span>|<span data-ttu-id="9cc15-217">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9cc15-217">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9cc15-218">只读，可为空</span><span class="sxs-lookup"><span data-stu-id="9cc15-218">Read-only, Nullable</span></span>|
|<span data-ttu-id="9cc15-219">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="9cc15-219">serviceConfigurationRecords</span></span>|<span data-ttu-id="9cc15-220">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9cc15-220">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="9cc15-221">在 Microsoft Online 服务可以使用域之前，客户添加到域的 DNS 区域文件的 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="9cc15-221">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span><br><span data-ttu-id="9cc15-222">只读，可为空</span><span class="sxs-lookup"><span data-stu-id="9cc15-222">Read-only, Nullable</span></span> |
|<span data-ttu-id="9cc15-223">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="9cc15-223">verificationDnsRecords</span></span>|<span data-ttu-id="9cc15-224">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9cc15-224">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="9cc15-225">客户在客户可以使用 Azure AD 完成域所有权验证之前添加到域的 DNS 区域文件的 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="9cc15-225">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span><br><span data-ttu-id="9cc15-226">只读，可为空</span><span class="sxs-lookup"><span data-stu-id="9cc15-226">Read-only, Nullable</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9cc15-227">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9cc15-227">JSON representation</span></span>
<span data-ttu-id="9cc15-228">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cc15-228">Here is a JSON representation of the resource.</span></span>

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


