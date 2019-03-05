---
title: 域资源类型
description: 表示与租户相关联的域。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bd141fe02ab7b2685f83ebcfb787aca4ced2294f
ms.sourcegitcommit: 159cf5aaa39d3721d96d3fd800f6a8b91159f74d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2019
ms.locfileid: "30379505"
---
# <a name="domain-resource-type"></a><span data-ttu-id="1cc4d-103">域资源类型</span><span class="sxs-lookup"><span data-stu-id="1cc4d-103">domain resource type</span></span>

<span data-ttu-id="1cc4d-104">表示与租户相关联的域。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-104">Represents a domain associated with the tenant.</span></span>

<span data-ttu-id="1cc4d-p101">使用域操作将域关联到租户，验证域所有关系并配置支持的服务。域操作让注册机构对服务（如 Office 365）的域关联启用自动化。例如，作为域注册的一部分，注册机构可以为电子邮件、网站、身份验证等启用虚域。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p101">Use domain operations to associate domains to a tenant, verify domain ownership, and configure supported services.  Domain operations enable registrars to automate domain association for services such as Office 365. For example, as part of domain sign up, a registrar can enable a vanity domain for email, websites, authentication, etc.</span></span>

<span data-ttu-id="1cc4d-108">若要将域与租户相关联，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="1cc4d-108">To associate a domain with a tenant:</span></span>

1. <span data-ttu-id="1cc4d-109">[关联](../api/domain-post-domains.md)域与租户。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-109">[Associate](../api/domain-post-domains.md) a domain with a tenant.</span></span>

2. <span data-ttu-id="1cc4d-p102">[检索](../api/domain-list-verificationdnsrecords.md)域验证记录。使用域注册机构或 DNS 服务器配置，向域区域文件添加验证记录详细信息。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p102">[Retrieve](../api/domain-list-verificationdnsrecords.md) the domain verification records. Add the verification record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

3. <span data-ttu-id="1cc4d-p103">[验证](../api/domain-verify.md)域的所有权。这将验证域，并将 *isVerified* 属性设置为 *true*。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p103">[Verify](../api/domain-verify.md) the ownership of the domain. This will verify the domain and set the *isVerified* property to *true*.</span></span>

4. <span data-ttu-id="1cc4d-114">[指明](../api/domain-update.md)计划与域配合使用的受支持服务。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-114">[Indicate](../api/domain-update.md) the supported services you plan to use with the domain.</span></span>

5. <span data-ttu-id="1cc4d-p104">通过检索需要为域启用服务的记录列表[配置](../api/domain-list-serviceconfigurationrecords.md)支持的服务。使用域注册机构或 DNS 服务器配置，向域区域文件添加配置记录详细信息。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p104">[Configure](../api/domain-list-serviceconfigurationrecords.md) supported services by retrieving a list of records needed to enable services for the domain. Add the configuration record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="1cc4d-117">方法</span><span class="sxs-lookup"><span data-stu-id="1cc4d-117">Methods</span></span>

| <span data-ttu-id="1cc4d-118">方法</span><span class="sxs-lookup"><span data-stu-id="1cc4d-118">Method</span></span>   | <span data-ttu-id="1cc4d-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="1cc4d-119">Return Type</span></span> |<span data-ttu-id="1cc4d-120">说明</span><span class="sxs-lookup"><span data-stu-id="1cc4d-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1cc4d-121">获取域</span><span class="sxs-lookup"><span data-stu-id="1cc4d-121">Get domain</span></span>](../api/domain-get.md) | [<span data-ttu-id="1cc4d-122">domain</span><span class="sxs-lookup"><span data-stu-id="1cc4d-122">domain</span></span>](domain.md) | <span data-ttu-id="1cc4d-123">读取 domain 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-123">Read properties and relationships of a domain object.</span></span>|
|[<span data-ttu-id="1cc4d-124">创建域</span><span class="sxs-lookup"><span data-stu-id="1cc4d-124">Create domain</span></span>](../api/domain-post-domains.md) | [<span data-ttu-id="1cc4d-125">domain</span><span class="sxs-lookup"><span data-stu-id="1cc4d-125">domain</span></span>](domain.md) | <span data-ttu-id="1cc4d-126">向租户添加域。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-126">Adds a domain to the tenant.</span></span> |
|[<span data-ttu-id="1cc4d-127">列出 domainNameReference</span><span class="sxs-lookup"><span data-stu-id="1cc4d-127">List domainNameReference</span></span>](../api/domain-list-domainnamereferences.md) |<span data-ttu-id="1cc4d-128">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="1cc4d-128">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1cc4d-129">通过对域的引用检索 directory 对象列表。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-129">Retrieve a list of directory objects with a reference to the domain.</span></span>|
|[<span data-ttu-id="1cc4d-130">列出 serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="1cc4d-130">List serviceConfigurationRecords</span></span>](../api/domain-list-serviceconfigurationrecords.md) |<span data-ttu-id="1cc4d-131">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1cc4d-131">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="1cc4d-132">检索域配置的域 DNS 记录列表。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-132">Retrieve a list of domain DNS records for domain configuration.</span></span>|
|[<span data-ttu-id="1cc4d-133">列出 verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="1cc4d-133">List verificationDnsRecords</span></span>](../api/domain-list-verificationdnsrecords.md) |<span data-ttu-id="1cc4d-134">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1cc4d-134">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="1cc4d-135">检索用于域验证的域 DNS 记录列表。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-135">Retrieve a list of domain DNS records for domain verification.</span></span>|
|[<span data-ttu-id="1cc4d-136">更新域</span><span class="sxs-lookup"><span data-stu-id="1cc4d-136">Update domain</span></span>](../api/domain-update.md) | [<span data-ttu-id="1cc4d-137">domain</span><span class="sxs-lookup"><span data-stu-id="1cc4d-137">domain</span></span>](domain.md) |<span data-ttu-id="1cc4d-138">更新域。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-138">Updates a domain.</span></span>|
|[<span data-ttu-id="1cc4d-139">删除域</span><span class="sxs-lookup"><span data-stu-id="1cc4d-139">Delete domain</span></span>](../api/domain-delete.md) | <span data-ttu-id="1cc4d-140">无</span><span class="sxs-lookup"><span data-stu-id="1cc4d-140">None</span></span> |<span data-ttu-id="1cc4d-141">删除域。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-141">Deletes a domain.</span></span>|
|[<span data-ttu-id="1cc4d-142">ForceDelete 域</span><span class="sxs-lookup"><span data-stu-id="1cc4d-142">ForceDelete domain</span></span>](../api/domain-forcedelete.md)|<span data-ttu-id="1cc4d-143">无</span><span class="sxs-lookup"><span data-stu-id="1cc4d-143">None</span></span>|<span data-ttu-id="1cc4d-144">使用异步操作删除域。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-144">Deletes a domain using an asynchronous operation.</span></span>|
|[<span data-ttu-id="1cc4d-145">验证域</span><span class="sxs-lookup"><span data-stu-id="1cc4d-145">Verify domain</span></span>](../api/domain-verify.md)|[<span data-ttu-id="1cc4d-146">域</span><span class="sxs-lookup"><span data-stu-id="1cc4d-146">domain</span></span>](domain.md)|<span data-ttu-id="1cc4d-147">验证域的所有权。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-147">Validates the ownership of the domain.</span></span>|

## <a name="properties"></a><span data-ttu-id="1cc4d-148">属性</span><span class="sxs-lookup"><span data-stu-id="1cc4d-148">Properties</span></span>

| <span data-ttu-id="1cc4d-149">属性</span><span class="sxs-lookup"><span data-stu-id="1cc4d-149">Property</span></span>   | <span data-ttu-id="1cc4d-150">类型</span><span class="sxs-lookup"><span data-stu-id="1cc4d-150">Type</span></span> | <span data-ttu-id="1cc4d-151">说明</span><span class="sxs-lookup"><span data-stu-id="1cc4d-151">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1cc4d-152">authenticationType</span><span class="sxs-lookup"><span data-stu-id="1cc4d-152">authenticationType</span></span>|<span data-ttu-id="1cc4d-153">String</span><span class="sxs-lookup"><span data-stu-id="1cc4d-153">String</span></span>| <span data-ttu-id="1cc4d-p105">表示为域配置的身份验证类型。此为*托管*或*联盟*值。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p105">Indicates the configured authentication type for the domain. The value is either *Managed* or *Federated*.</span></span><br> <span data-ttu-id="1cc4d-156">*托管*表示 Azure AD 执行用户身份验证的云托管域。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-156">*Managed* indicates a cloud managed domain where Azure AD performs user authentication.</span></span><br><span data-ttu-id="1cc4d-p106">*联盟*表示身份验证与标识提供程序（如通过 Active Directory 联合身份验证服务的租户的本地 Active Directory）联合。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p106">*Federated* indicates authentication is federated with an identity provider such as the tenant's on-premises Active Directory via Active Directory Federation Services. Not nullable</span></span> |
|<span data-ttu-id="1cc4d-159">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="1cc4d-159">availabilityStatus</span></span>|<span data-ttu-id="1cc4d-160">String</span><span class="sxs-lookup"><span data-stu-id="1cc4d-160">String</span></span>| <span data-ttu-id="1cc4d-p107">使用[验证](../api/domain-verify.md)操作时，此属性始终为 Null。使用[验证](../api/domain-verify.md)操作时，响应中返回**域**实体。响应中的**域**实体的 **availabilityStatus** 属性为 *AvailableImmediately* 或 *EmailVerifiedDomainTakeoverScheduled*。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p107">This property is always null except when the [verify](../api/domain-verify.md) action is used. When the [verify](../api/domain-verify.md) action is used, a **domain** entity is returned in the response. The **availabilityStatus** property of the **domain** entity in the response is either *AvailableImmediately* or *EmailVerifiedDomainTakeoverScheduled*.</span></span>|
|<span data-ttu-id="1cc4d-164">id</span><span class="sxs-lookup"><span data-stu-id="1cc4d-164">id</span></span>|<span data-ttu-id="1cc4d-165">字符串</span><span class="sxs-lookup"><span data-stu-id="1cc4d-165">String</span></span>| <span data-ttu-id="1cc4d-p108">域的完全限定的名称。密钥、不可变、不可为 Null、唯一</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p108">The fully qualified name of the domain. Key, immutable, not nullable, unique</span></span> |
|<span data-ttu-id="1cc4d-168">isAdminManaged</span><span class="sxs-lookup"><span data-stu-id="1cc4d-168">isAdminManaged</span></span>|<span data-ttu-id="1cc4d-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cc4d-169">Boolean</span></span>| <span data-ttu-id="1cc4d-p109">如果域的 DNS 记录管理已委派为 Office 365，则属性值为 false。否则，此值为 true。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p109">The value of the property is false if the DNS record management of the domain has been delegated to Office 365. Otherwise, the value is true. Not nullable</span></span> |
|<span data-ttu-id="1cc4d-173">isDefault</span><span class="sxs-lookup"><span data-stu-id="1cc4d-173">isDefault</span></span>|<span data-ttu-id="1cc4d-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cc4d-174">Boolean</span></span>| <span data-ttu-id="1cc4d-p110">如果这是用于创建用户的默认域，则为 true。每个公司仅有一个默认域。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p110">True if this is the default domain that is used for user creation. There is only one default domain per company. Not nullable</span></span> |
|<span data-ttu-id="1cc4d-178">isInitial</span><span class="sxs-lookup"><span data-stu-id="1cc4d-178">isInitial</span></span>|<span data-ttu-id="1cc4d-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cc4d-179">Boolean</span></span>| <span data-ttu-id="1cc4d-p111">如果这是由 Microsoft Online Services (companyname.onmicrosoft.com) 创建的初始域，则为 true。每个公司仅有一个初始域。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p111">True if this is the initial domain created by Microsoft Online Services (companyname.onmicrosoft.com). There is only one initial domain per company. Not nullable</span></span> |
|<span data-ttu-id="1cc4d-183">isRoot</span><span class="sxs-lookup"><span data-stu-id="1cc4d-183">isRoot</span></span>|<span data-ttu-id="1cc4d-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cc4d-184">Boolean</span></span>| <span data-ttu-id="1cc4d-p112">如果此域是一个已验证的根域，则为 true。否则，如果此域为子域或未经验证，则为 false。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p112">True if the domain is a verified root domain. Otherwise, false if the domain is a subdomain or unverified. Not nullable</span></span> |
|<span data-ttu-id="1cc4d-188">isVerified</span><span class="sxs-lookup"><span data-stu-id="1cc4d-188">isVerified</span></span>|<span data-ttu-id="1cc4d-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cc4d-189">Boolean</span></span>| <span data-ttu-id="1cc4d-p113">如果域已完成域所有权验证，则为 true。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p113">True if the domain has completed domain ownership verification. Not nullable</span></span> |
|<span data-ttu-id="1cc4d-192">passwordNotificationWindowInDays</span><span class="sxs-lookup"><span data-stu-id="1cc4d-192">passwordNotificationWindowInDays</span></span>|<span data-ttu-id="1cc4d-193">Int32</span><span class="sxs-lookup"><span data-stu-id="1cc4d-193">Int32</span></span>|<span data-ttu-id="1cc4d-194">指定用户收到其密码将到期的通知之前的天数。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-194">Specifies the number of days before a user receives notification that their password will expire.</span></span> <span data-ttu-id="1cc4d-195">如果未设置该属性, 则将使用默认值14天。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-195">If the property is not set, a default value of 14 days will be used.</span></span>|
|<span data-ttu-id="1cc4d-196">passwordValidityPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="1cc4d-196">passwordValidityPeriodInDays</span></span>|<span data-ttu-id="1cc4d-197">Int32</span><span class="sxs-lookup"><span data-stu-id="1cc4d-197">Int32</span></span>| <span data-ttu-id="1cc4d-198">指定密码在必须更改之前有效的时间长度。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-198">Specifies the length of time that a password is valid before it must be changed.</span></span> <span data-ttu-id="1cc4d-199">如果未设置该属性, 则将使用默认值90天。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-199">If the property is not set, a default value of 90 days will be used.</span></span> |
|<span data-ttu-id="1cc4d-200">supportedServices</span><span class="sxs-lookup"><span data-stu-id="1cc4d-200">supportedServices</span></span>|<span data-ttu-id="1cc4d-201">字符串集合</span><span class="sxs-lookup"><span data-stu-id="1cc4d-201">String collection</span></span>| <span data-ttu-id="1cc4d-202">分配给域的功能。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-202">The capabilities assigned to the domain.</span></span><br><br><span data-ttu-id="1cc4d-203">可以包含下列值中的 0 个、1 个或更多个：*电子邮件*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="1cc4d-203">Can include 0, 1 or more of following values: *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span><br><br> <span data-ttu-id="1cc4d-204">可以使用 Graph API 添加/删除的值包括：*电子邮件*、*OfficeCommunicationsOnline*、*Yammer*</span><span class="sxs-lookup"><span data-stu-id="1cc4d-204">The values which you can add/remove using Graph API include: *Email*, *OfficeCommunicationsOnline*, *Yammer*</span></span><br><span data-ttu-id="1cc4d-205">不可为 Null</span><span class="sxs-lookup"><span data-stu-id="1cc4d-205">Not nullable</span></span>|
|<span data-ttu-id="1cc4d-206">状态</span><span class="sxs-lookup"><span data-stu-id="1cc4d-206">state</span></span>|[<span data-ttu-id="1cc4d-207">domainState</span><span class="sxs-lookup"><span data-stu-id="1cc4d-207">domainState</span></span>](domainstate.md)| <span data-ttu-id="1cc4d-208">为域计划的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-208">Status of asynchronous operations scheduled for the domain.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1cc4d-209">关系</span><span class="sxs-lookup"><span data-stu-id="1cc4d-209">Relationships</span></span>

<span data-ttu-id="1cc4d-p116">通过导航属性公开目录中的域和其他对象之间的关系（如它们的验证记录和服务配置记录）。你可以通过在请求中定位这些导航属性来读取这些关系。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-p116">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties. You can read these relationships by targeting these navigation properties in your requests.</span></span>

| <span data-ttu-id="1cc4d-212">关系</span><span class="sxs-lookup"><span data-stu-id="1cc4d-212">Relationship</span></span> | <span data-ttu-id="1cc4d-213">类型</span><span class="sxs-lookup"><span data-stu-id="1cc4d-213">Type</span></span> |<span data-ttu-id="1cc4d-214">说明</span><span class="sxs-lookup"><span data-stu-id="1cc4d-214">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cc4d-215">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="1cc4d-215">domainNameReferences</span></span>|<span data-ttu-id="1cc4d-216">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1cc4d-216">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1cc4d-217">只读，可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-217">Read-only, Nullable</span></span>|
|<span data-ttu-id="1cc4d-218">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="1cc4d-218">serviceConfigurationRecords</span></span>|<span data-ttu-id="1cc4d-219">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1cc4d-219">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="1cc4d-220">Microsoft Online Services 可以使用域之前，客户添加到域 DNS 区域文件的 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-220">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span><br><span data-ttu-id="1cc4d-221">只读，可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-221">Read-only, Nullable</span></span> |
|<span data-ttu-id="1cc4d-222">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="1cc4d-222">verificationDnsRecords</span></span>|<span data-ttu-id="1cc4d-223">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1cc4d-223">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="1cc4d-224">客户可以使用 Azure AD 完成域所有权验证之前，客户添加到域 DNS 区域文件的 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-224">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span><br><span data-ttu-id="1cc4d-225">只读，可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-225">Read-only, Nullable</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1cc4d-226">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1cc4d-226">JSON representation</span></span>
<span data-ttu-id="1cc4d-227">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cc4d-227">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
