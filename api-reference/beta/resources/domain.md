---
title: 域资源类型
description: 表示与租户关联的域。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cd1cc0e199848243fd9957f0741f609e052af6e6
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43178938"
---
# <a name="domain-resource-type"></a><span data-ttu-id="11062-103">域资源类型</span><span class="sxs-lookup"><span data-stu-id="11062-103">domain resource type</span></span>

<span data-ttu-id="11062-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11062-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11062-105">表示与租户关联的域。</span><span class="sxs-lookup"><span data-stu-id="11062-105">Represents a domain associated with the tenant.</span></span>

<span data-ttu-id="11062-106">使用域操作将域与租户相关联，验证域所有权并配置受支持的服务。</span><span class="sxs-lookup"><span data-stu-id="11062-106">Use domain operations to associate domains to a tenant, verify domain ownership, and configure supported services.</span></span>  <span data-ttu-id="11062-107">域操作使注册机构能够自动为 Office 365 等服务的域关联。</span><span class="sxs-lookup"><span data-stu-id="11062-107">Domain operations enable registrars to automate domain association for services such as Office 365.</span></span> <span data-ttu-id="11062-108">例如，在注册域的过程中，注册机构可以为电子邮件、网站、身份验证等启用虚域。</span><span class="sxs-lookup"><span data-stu-id="11062-108">For example, as part of domain sign up, a registrar can enable a vanity domain for email, websites, authentication, etc.</span></span>

<span data-ttu-id="11062-109">将域与租户相关联：</span><span class="sxs-lookup"><span data-stu-id="11062-109">To associate a domain with a tenant:</span></span>

1. <span data-ttu-id="11062-110">将域与租户[相关联](../api/domain-post-domains.md)。</span><span class="sxs-lookup"><span data-stu-id="11062-110">[Associate](../api/domain-post-domains.md) a domain with a tenant.</span></span>

2. <span data-ttu-id="11062-111">[检索](../api/domain-list-verificationdnsrecords.md)域验证记录。</span><span class="sxs-lookup"><span data-stu-id="11062-111">[Retrieve](../api/domain-list-verificationdnsrecords.md) the domain verification records.</span></span> <span data-ttu-id="11062-112">使用域注册机构或 DNS 服务器配置将验证记录详细信息添加到域的区域文件。</span><span class="sxs-lookup"><span data-stu-id="11062-112">Add the verification record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

3. <span data-ttu-id="11062-113">[验证](../api/domain-verify.md)域的所有权。</span><span class="sxs-lookup"><span data-stu-id="11062-113">[Verify](../api/domain-verify.md) the ownership of the domain.</span></span> <span data-ttu-id="11062-114">这将验证域并将*isVerified*属性设置为*true*。</span><span class="sxs-lookup"><span data-stu-id="11062-114">This will verify the domain and set the *isVerified* property to *true*.</span></span>

4. <span data-ttu-id="11062-115">[指明](../api/domain-update.md)计划与域一起使用的受支持服务。</span><span class="sxs-lookup"><span data-stu-id="11062-115">[Indicate](../api/domain-update.md) the supported services you plan to use with the domain.</span></span>

5. <span data-ttu-id="11062-116">通过检索为域启用服务所需的记录列表来[配置](../api/domain-list-serviceconfigurationrecords.md)受支持的服务。</span><span class="sxs-lookup"><span data-stu-id="11062-116">[Configure](../api/domain-list-serviceconfigurationrecords.md) supported services by retrieving a list of records needed to enable services for the domain.</span></span> <span data-ttu-id="11062-117">使用域注册机构或 DNS 服务器配置将配置记录详细信息添加到域的区域文件中。</span><span class="sxs-lookup"><span data-stu-id="11062-117">Add the configuration record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="11062-118">方法</span><span class="sxs-lookup"><span data-stu-id="11062-118">Methods</span></span>

| <span data-ttu-id="11062-119">方法</span><span class="sxs-lookup"><span data-stu-id="11062-119">Method</span></span>   | <span data-ttu-id="11062-120">返回类型</span><span class="sxs-lookup"><span data-stu-id="11062-120">Return Type</span></span> |<span data-ttu-id="11062-121">说明</span><span class="sxs-lookup"><span data-stu-id="11062-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11062-122">获取域</span><span class="sxs-lookup"><span data-stu-id="11062-122">Get domain</span></span>](../api/domain-get.md) | [<span data-ttu-id="11062-123">domain</span><span class="sxs-lookup"><span data-stu-id="11062-123">domain</span></span>](domain.md) | <span data-ttu-id="11062-124">读取域对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="11062-124">Read properties and relationships of a domain object.</span></span>|
|[<span data-ttu-id="11062-125">创建域</span><span class="sxs-lookup"><span data-stu-id="11062-125">Create domain</span></span>](../api/domain-post-domains.md) | [<span data-ttu-id="11062-126">domain</span><span class="sxs-lookup"><span data-stu-id="11062-126">domain</span></span>](domain.md) | <span data-ttu-id="11062-127">向租户添加域。</span><span class="sxs-lookup"><span data-stu-id="11062-127">Adds a domain to the tenant.</span></span> |
|[<span data-ttu-id="11062-128">列出 domainNameReference</span><span class="sxs-lookup"><span data-stu-id="11062-128">List domainNameReference</span></span>](../api/domain-list-domainnamereferences.md) |<span data-ttu-id="11062-129">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="11062-129">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="11062-130">使用对域的引用检索目录对象的列表。</span><span class="sxs-lookup"><span data-stu-id="11062-130">Retrieve a list of directory objects with a reference to the domain.</span></span>|
|[<span data-ttu-id="11062-131">列出 serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="11062-131">List serviceConfigurationRecords</span></span>](../api/domain-list-serviceconfigurationrecords.md) |<span data-ttu-id="11062-132">[domainDnsRecord](domaindnsrecord.md)集合</span><span class="sxs-lookup"><span data-stu-id="11062-132">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="11062-133">检索域配置的域 DNS 记录列表。</span><span class="sxs-lookup"><span data-stu-id="11062-133">Retrieve a list of domain DNS records for domain configuration.</span></span>|
|[<span data-ttu-id="11062-134">列出 verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="11062-134">List verificationDnsRecords</span></span>](../api/domain-list-verificationdnsrecords.md) |<span data-ttu-id="11062-135">[domainDnsRecord](domaindnsrecord.md)集合</span><span class="sxs-lookup"><span data-stu-id="11062-135">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="11062-136">检索域验证的域 DNS 记录列表。</span><span class="sxs-lookup"><span data-stu-id="11062-136">Retrieve a list of domain DNS records for domain verification.</span></span>|
|[<span data-ttu-id="11062-137">更新域</span><span class="sxs-lookup"><span data-stu-id="11062-137">Update domain</span></span>](../api/domain-update.md) | [<span data-ttu-id="11062-138">domain</span><span class="sxs-lookup"><span data-stu-id="11062-138">domain</span></span>](domain.md) |<span data-ttu-id="11062-139">更新域。</span><span class="sxs-lookup"><span data-stu-id="11062-139">Updates a domain.</span></span>|
|[<span data-ttu-id="11062-140">删除域</span><span class="sxs-lookup"><span data-stu-id="11062-140">Delete domain</span></span>](../api/domain-delete.md) | <span data-ttu-id="11062-141">无</span><span class="sxs-lookup"><span data-stu-id="11062-141">None</span></span> |<span data-ttu-id="11062-142">删除域。</span><span class="sxs-lookup"><span data-stu-id="11062-142">Deletes a domain.</span></span>|
|[<span data-ttu-id="11062-143">ForceDelete 域</span><span class="sxs-lookup"><span data-stu-id="11062-143">ForceDelete domain</span></span>](../api/domain-forcedelete.md)|<span data-ttu-id="11062-144">无</span><span class="sxs-lookup"><span data-stu-id="11062-144">None</span></span>|<span data-ttu-id="11062-145">使用异步操作删除域。</span><span class="sxs-lookup"><span data-stu-id="11062-145">Deletes a domain using an asynchronous operation.</span></span>|
|[<span data-ttu-id="11062-146">验证域</span><span class="sxs-lookup"><span data-stu-id="11062-146">Verify domain</span></span>](../api/domain-verify.md)|[<span data-ttu-id="11062-147">domain</span><span class="sxs-lookup"><span data-stu-id="11062-147">domain</span></span>](domain.md)|<span data-ttu-id="11062-148">验证域的所有权。</span><span class="sxs-lookup"><span data-stu-id="11062-148">Validates the ownership of the domain.</span></span>|

## <a name="properties"></a><span data-ttu-id="11062-149">属性</span><span class="sxs-lookup"><span data-stu-id="11062-149">Properties</span></span>

| <span data-ttu-id="11062-150">属性</span><span class="sxs-lookup"><span data-stu-id="11062-150">Property</span></span>   | <span data-ttu-id="11062-151">类型</span><span class="sxs-lookup"><span data-stu-id="11062-151">Type</span></span> | <span data-ttu-id="11062-152">说明</span><span class="sxs-lookup"><span data-stu-id="11062-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="11062-153">authenticationType</span><span class="sxs-lookup"><span data-stu-id="11062-153">authenticationType</span></span>|<span data-ttu-id="11062-154">String</span><span class="sxs-lookup"><span data-stu-id="11062-154">String</span></span>| <span data-ttu-id="11062-155">指示为域配置的身份验证类型。</span><span class="sxs-lookup"><span data-stu-id="11062-155">Indicates the configured authentication type for the domain.</span></span> <span data-ttu-id="11062-156">值为 "*托管*" 或 "*联合*"。</span><span class="sxs-lookup"><span data-stu-id="11062-156">The value is either *Managed* or *Federated*.</span></span><br> <span data-ttu-id="11062-157">*托管*表示 Azure AD 执行用户身份验证的云托管域。</span><span class="sxs-lookup"><span data-stu-id="11062-157">*Managed* indicates a cloud managed domain where Azure AD performs user authentication.</span></span><br><span data-ttu-id="11062-158">*联合*指示身份验证通过使用标识提供程序（如通过 Active Directory 联合身份验证服务的租户的本地 Active directory）进行联合。</span><span class="sxs-lookup"><span data-stu-id="11062-158">*Federated* indicates authentication is federated with an identity provider such as the tenant's on-premises Active Directory via Active Directory Federation Services.</span></span> <span data-ttu-id="11062-159">此属性为只读，且不可为 null。</span><span class="sxs-lookup"><span data-stu-id="11062-159">This propert is read-only and is not nullable.</span></span> |
|<span data-ttu-id="11062-160">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="11062-160">availabilityStatus</span></span>|<span data-ttu-id="11062-161">String</span><span class="sxs-lookup"><span data-stu-id="11062-161">String</span></span>| <span data-ttu-id="11062-162">除非使用了[verify](../api/domain-verify.md)操作，否则此属性始终为 null。</span><span class="sxs-lookup"><span data-stu-id="11062-162">This property is always null except when the [verify](../api/domain-verify.md) action is used.</span></span> <span data-ttu-id="11062-163">使用[验证](../api/domain-verify.md)操作时，会在响应中返回**域**实体。</span><span class="sxs-lookup"><span data-stu-id="11062-163">When the [verify](../api/domain-verify.md) action is used, a **domain** entity is returned in the response.</span></span> <span data-ttu-id="11062-164">响应中的**域**实体的**AvailabilityStatus**属性为*AvailableImmediately*或*EmailVerifiedDomainTakeoverScheduled*。</span><span class="sxs-lookup"><span data-stu-id="11062-164">The **availabilityStatus** property of the **domain** entity in the response is either *AvailableImmediately* or *EmailVerifiedDomainTakeoverScheduled*.</span></span>|
|<span data-ttu-id="11062-165">id</span><span class="sxs-lookup"><span data-stu-id="11062-165">id</span></span>|<span data-ttu-id="11062-166">String</span><span class="sxs-lookup"><span data-stu-id="11062-166">String</span></span>| <span data-ttu-id="11062-167">域的完全限定的名称。</span><span class="sxs-lookup"><span data-stu-id="11062-167">The fully qualified name of the domain.</span></span> <span data-ttu-id="11062-168">键、不可变、不可为 null、唯一</span><span class="sxs-lookup"><span data-stu-id="11062-168">Key, immutable, not nullable, unique</span></span> |
|<span data-ttu-id="11062-169">isAdminManaged</span><span class="sxs-lookup"><span data-stu-id="11062-169">isAdminManaged</span></span>|<span data-ttu-id="11062-170">布尔值</span><span class="sxs-lookup"><span data-stu-id="11062-170">Boolean</span></span>| <span data-ttu-id="11062-171">如果域的 DNS 记录管理已委派给 Office 365，则该属性的值为 false。</span><span class="sxs-lookup"><span data-stu-id="11062-171">The value of the property is false if the DNS record management of the domain has been delegated to Office 365.</span></span> <span data-ttu-id="11062-172">否则，该值为 true。</span><span class="sxs-lookup"><span data-stu-id="11062-172">Otherwise, the value is true.</span></span> <span data-ttu-id="11062-173">不可为 null</span><span class="sxs-lookup"><span data-stu-id="11062-173">Not nullable</span></span> |
|<span data-ttu-id="11062-174">isDefault</span><span class="sxs-lookup"><span data-stu-id="11062-174">isDefault</span></span>|<span data-ttu-id="11062-175">布尔值</span><span class="sxs-lookup"><span data-stu-id="11062-175">Boolean</span></span>| <span data-ttu-id="11062-176">如果这是用于创建用户的默认域，则为 True。</span><span class="sxs-lookup"><span data-stu-id="11062-176">True if this is the default domain that is used for user creation.</span></span> <span data-ttu-id="11062-177">每个公司只有一个默认域。</span><span class="sxs-lookup"><span data-stu-id="11062-177">There is only one default domain per company.</span></span> <span data-ttu-id="11062-178">不可为 null</span><span class="sxs-lookup"><span data-stu-id="11062-178">Not nullable</span></span> |
|<span data-ttu-id="11062-179">isInitial</span><span class="sxs-lookup"><span data-stu-id="11062-179">isInitial</span></span>|<span data-ttu-id="11062-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="11062-180">Boolean</span></span>| <span data-ttu-id="11062-181">如果这是 Microsoft Online Services （companyname.onmicrosoft.com）创建的初始域，则为 True。</span><span class="sxs-lookup"><span data-stu-id="11062-181">True if this is the initial domain created by Microsoft Online Services (companyname.onmicrosoft.com).</span></span> <span data-ttu-id="11062-182">每个公司只有一个初始域。</span><span class="sxs-lookup"><span data-stu-id="11062-182">There is only one initial domain per company.</span></span> <span data-ttu-id="11062-183">不可为 null</span><span class="sxs-lookup"><span data-stu-id="11062-183">Not nullable</span></span> |
|<span data-ttu-id="11062-184">isRoot</span><span class="sxs-lookup"><span data-stu-id="11062-184">isRoot</span></span>|<span data-ttu-id="11062-185">布尔值</span><span class="sxs-lookup"><span data-stu-id="11062-185">Boolean</span></span>| <span data-ttu-id="11062-186">如果域是经过验证的根域，则为 True。</span><span class="sxs-lookup"><span data-stu-id="11062-186">True if the domain is a verified root domain.</span></span> <span data-ttu-id="11062-187">否则，如果域是子域或未验证，则为 false。</span><span class="sxs-lookup"><span data-stu-id="11062-187">Otherwise, false if the domain is a subdomain or unverified.</span></span> <span data-ttu-id="11062-188">不可为 null</span><span class="sxs-lookup"><span data-stu-id="11062-188">Not nullable</span></span> |
|<span data-ttu-id="11062-189">isVerified</span><span class="sxs-lookup"><span data-stu-id="11062-189">isVerified</span></span>|<span data-ttu-id="11062-190">布尔值</span><span class="sxs-lookup"><span data-stu-id="11062-190">Boolean</span></span>| <span data-ttu-id="11062-191">如果域已完成域所有权验证，则为 True。</span><span class="sxs-lookup"><span data-stu-id="11062-191">True if the domain has completed domain ownership verification.</span></span> <span data-ttu-id="11062-192">不可为 null</span><span class="sxs-lookup"><span data-stu-id="11062-192">Not nullable</span></span> |
|<span data-ttu-id="11062-193">passwordNotificationWindowInDays</span><span class="sxs-lookup"><span data-stu-id="11062-193">passwordNotificationWindowInDays</span></span>|<span data-ttu-id="11062-194">Int32</span><span class="sxs-lookup"><span data-stu-id="11062-194">Int32</span></span>|<span data-ttu-id="11062-195">指定用户收到其密码将到期的通知之前的天数。</span><span class="sxs-lookup"><span data-stu-id="11062-195">Specifies the number of days before a user receives notification that their password will expire.</span></span> <span data-ttu-id="11062-196">如果未设置该属性，则将使用默认值14天。</span><span class="sxs-lookup"><span data-stu-id="11062-196">If the property is not set, a default value of 14 days will be used.</span></span>|
|<span data-ttu-id="11062-197">passwordValidityPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="11062-197">passwordValidityPeriodInDays</span></span>|<span data-ttu-id="11062-198">Int32</span><span class="sxs-lookup"><span data-stu-id="11062-198">Int32</span></span>| <span data-ttu-id="11062-199">指定密码在必须更改之前有效的时间长度。</span><span class="sxs-lookup"><span data-stu-id="11062-199">Specifies the length of time that a password is valid before it must be changed.</span></span> <span data-ttu-id="11062-200">如果未设置该属性，则将使用默认值90天。</span><span class="sxs-lookup"><span data-stu-id="11062-200">If the property is not set, a default value of 90 days will be used.</span></span> |
|<span data-ttu-id="11062-201">supportedServices</span><span class="sxs-lookup"><span data-stu-id="11062-201">supportedServices</span></span>|<span data-ttu-id="11062-202">String 集合</span><span class="sxs-lookup"><span data-stu-id="11062-202">String collection</span></span>| <span data-ttu-id="11062-203">分配给域的功能。</span><span class="sxs-lookup"><span data-stu-id="11062-203">The capabilities assigned to the domain.</span></span><br><br><span data-ttu-id="11062-204">可以包含0个、1个或更多的以下值： *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="11062-204">Can include 0, 1 or more of following values: *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span><br><br> <span data-ttu-id="11062-205">您可以使用 Graph API 添加/删除的值包括： *Email*、 *OfficeCommunicationsOnline*、 *Yammer*</span><span class="sxs-lookup"><span data-stu-id="11062-205">The values which you can add/remove using Graph API include: *Email*, *OfficeCommunicationsOnline*, *Yammer*</span></span><br><span data-ttu-id="11062-206">不可为 null</span><span class="sxs-lookup"><span data-stu-id="11062-206">Not nullable</span></span>|
|<span data-ttu-id="11062-207">state</span><span class="sxs-lookup"><span data-stu-id="11062-207">state</span></span>|[<span data-ttu-id="11062-208">domainState</span><span class="sxs-lookup"><span data-stu-id="11062-208">domainState</span></span>](domainstate.md)| <span data-ttu-id="11062-209">为域计划的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="11062-209">Status of asynchronous operations scheduled for the domain.</span></span> |

## <a name="relationships"></a><span data-ttu-id="11062-210">关系</span><span class="sxs-lookup"><span data-stu-id="11062-210">Relationships</span></span>

<span data-ttu-id="11062-211">域和目录中的其他对象（如其验证记录和服务配置记录）之间的关系通过导航属性公开。</span><span class="sxs-lookup"><span data-stu-id="11062-211">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties.</span></span> <span data-ttu-id="11062-212">您可以通过在请求中将这些导航属性作为目标来读取这些关系。</span><span class="sxs-lookup"><span data-stu-id="11062-212">You can read these relationships by targeting these navigation properties in your requests.</span></span>

| <span data-ttu-id="11062-213">关系</span><span class="sxs-lookup"><span data-stu-id="11062-213">Relationship</span></span> | <span data-ttu-id="11062-214">类型</span><span class="sxs-lookup"><span data-stu-id="11062-214">Type</span></span> |<span data-ttu-id="11062-215">说明</span><span class="sxs-lookup"><span data-stu-id="11062-215">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11062-216">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="11062-216">domainNameReferences</span></span>|<span data-ttu-id="11062-217">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="11062-217">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="11062-218">只读、可以为 Null</span><span class="sxs-lookup"><span data-stu-id="11062-218">Read-only, Nullable</span></span>|
|<span data-ttu-id="11062-219">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="11062-219">serviceConfigurationRecords</span></span>|<span data-ttu-id="11062-220">[domainDnsRecord](domaindnsrecord.md)集合</span><span class="sxs-lookup"><span data-stu-id="11062-220">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="11062-221">在 Microsoft Online services 可以使用域之前，客户添加到域的 DNS 区域文件中的 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="11062-221">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span><br><span data-ttu-id="11062-222">只读、可以为 Null</span><span class="sxs-lookup"><span data-stu-id="11062-222">Read-only, Nullable</span></span> |
|<span data-ttu-id="11062-223">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="11062-223">verificationDnsRecords</span></span>|<span data-ttu-id="11062-224">[domainDnsRecord](domaindnsrecord.md)集合</span><span class="sxs-lookup"><span data-stu-id="11062-224">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="11062-225">在客户可以使用 Azure AD 完成域所有权验证之前，客户添加到域的 DNS 区域文件中的 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="11062-225">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span><br><span data-ttu-id="11062-226">只读、可以为 Null</span><span class="sxs-lookup"><span data-stu-id="11062-226">Read-only, Nullable</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11062-227">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11062-227">JSON representation</span></span>
<span data-ttu-id="11062-228">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11062-228">Here is a JSON representation of the resource.</span></span>

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
