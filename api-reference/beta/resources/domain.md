---
title: 域资源类型
description: 表示与租户相关联的域。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d8dabf29285aea0b24613e584184dc13e02e499
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942393"
---
# <a name="domain-resource-type"></a><span data-ttu-id="52346-103">域资源类型</span><span class="sxs-lookup"><span data-stu-id="52346-103">domain resource type</span></span>

> <span data-ttu-id="52346-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="52346-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52346-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="52346-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52346-106">表示与租户相关联的域。</span><span class="sxs-lookup"><span data-stu-id="52346-106">Represents a domain associated with the tenant.</span></span>

<span data-ttu-id="52346-p102">使用域操作将域关联到租户，验证域所有关系并配置支持的服务。域操作让注册机构对服务（如 Office 365）的域关联启用自动化。例如，作为域注册的一部分，注册机构可以为电子邮件、网站、身份验证等启用虚域。</span><span class="sxs-lookup"><span data-stu-id="52346-p102">Use domain operations to associate domains to a tenant, verify domain ownership, and configure supported services.  Domain operations enable registrars to automate domain association for services such as Office 365. For example, as part of domain sign up, a registrar can enable a vanity domain for email, websites, authentication, etc.</span></span>

<span data-ttu-id="52346-110">若要将域与租户相关联，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="52346-110">To associate a domain with a tenant:</span></span>

1. <span data-ttu-id="52346-111">[关联](../api/domain-post-domains.md)域与租户。</span><span class="sxs-lookup"><span data-stu-id="52346-111">[Associate](../api/domain-post-domains.md) a domain with a tenant.</span></span>

2. <span data-ttu-id="52346-p103">[检索](../api/domain-list-verificationdnsrecords.md)域验证记录。使用域注册机构或 DNS 服务器配置，向域区域文件添加验证记录详细信息。</span><span class="sxs-lookup"><span data-stu-id="52346-p103">[Retrieve](../api/domain-list-verificationdnsrecords.md) the domain verification records. Add the verification record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

3. <span data-ttu-id="52346-p104">[验证](../api/domain-verify.md)域的所有权。这将验证域，并将 *isVerified* 属性设置为 *true*。</span><span class="sxs-lookup"><span data-stu-id="52346-p104">[Verify](../api/domain-verify.md) the ownership of the domain. This will verify the domain and set the *isVerified* property to *true*.</span></span>

4. <span data-ttu-id="52346-116">[指明](../api/domain-update.md)计划与域配合使用的受支持服务。</span><span class="sxs-lookup"><span data-stu-id="52346-116">[Indicate](../api/domain-update.md) the supported services you plan to use with the domain.</span></span>

5. <span data-ttu-id="52346-p105">通过检索需要为域启用服务的记录列表[配置](../api/domain-list-serviceconfigurationrecords.md)支持的服务。使用域注册机构或 DNS 服务器配置，向域区域文件添加配置记录详细信息。</span><span class="sxs-lookup"><span data-stu-id="52346-p105">[Configure](../api/domain-list-serviceconfigurationrecords.md) supported services by retrieving a list of records needed to enable services for the domain. Add the configuration record details to the domain's zone file using the domain registrar or DNS server configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="52346-119">方法</span><span class="sxs-lookup"><span data-stu-id="52346-119">Methods</span></span>

| <span data-ttu-id="52346-120">方法</span><span class="sxs-lookup"><span data-stu-id="52346-120">Method</span></span>   | <span data-ttu-id="52346-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="52346-121">Return Type</span></span> |<span data-ttu-id="52346-122">说明</span><span class="sxs-lookup"><span data-stu-id="52346-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52346-123">获取域</span><span class="sxs-lookup"><span data-stu-id="52346-123">Get domain</span></span>](../api/domain-get.md) | [<span data-ttu-id="52346-124">域</span><span class="sxs-lookup"><span data-stu-id="52346-124">domain</span></span>](domain.md) | <span data-ttu-id="52346-125">读取 domain 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="52346-125">Read properties and relationships of a domain object.</span></span>|
|[<span data-ttu-id="52346-126">创建域</span><span class="sxs-lookup"><span data-stu-id="52346-126">Create domain</span></span>](../api/domain-post-domains.md) | [<span data-ttu-id="52346-127">域</span><span class="sxs-lookup"><span data-stu-id="52346-127">domain</span></span>](domain.md) | <span data-ttu-id="52346-128">向租户添加域。</span><span class="sxs-lookup"><span data-stu-id="52346-128">Adds a domain to the tenant.</span></span> |
|[<span data-ttu-id="52346-129">列出 domainNameReference</span><span class="sxs-lookup"><span data-stu-id="52346-129">List domainNameReference</span></span>](../api/domain-list-domainnamereferences.md) |<span data-ttu-id="52346-130">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52346-130">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="52346-131">通过对域的引用检索 directory 对象列表。</span><span class="sxs-lookup"><span data-stu-id="52346-131">Retrieve a list of directory objects with a reference to the domain.</span></span>|
|[<span data-ttu-id="52346-132">列出 serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="52346-132">List serviceConfigurationRecords</span></span>](../api/domain-list-serviceconfigurationrecords.md) |<span data-ttu-id="52346-133">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52346-133">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="52346-134">检索域配置的域 DNS 记录列表。</span><span class="sxs-lookup"><span data-stu-id="52346-134">Retrieve a list of domain DNS records for domain configuration.</span></span>|
|[<span data-ttu-id="52346-135">列出 verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="52346-135">List verificationDnsRecords</span></span>](../api/domain-list-verificationdnsrecords.md) |<span data-ttu-id="52346-136">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52346-136">[domainDnsRecord](domaindnsrecord.md) collection</span></span>|  <span data-ttu-id="52346-137">检索用于域验证的域 DNS 记录列表。</span><span class="sxs-lookup"><span data-stu-id="52346-137">Retrieve a list of domain DNS records for domain verification.</span></span>|
|[<span data-ttu-id="52346-138">更新域</span><span class="sxs-lookup"><span data-stu-id="52346-138">Update domain</span></span>](../api/domain-update.md) | [<span data-ttu-id="52346-139">域</span><span class="sxs-lookup"><span data-stu-id="52346-139">domain</span></span>](domain.md) |<span data-ttu-id="52346-140">更新域。</span><span class="sxs-lookup"><span data-stu-id="52346-140">Updates a domain.</span></span>|
|[<span data-ttu-id="52346-141">删除域</span><span class="sxs-lookup"><span data-stu-id="52346-141">Delete domain</span></span>](../api/domain-delete.md) | <span data-ttu-id="52346-142">无</span><span class="sxs-lookup"><span data-stu-id="52346-142">None</span></span> |<span data-ttu-id="52346-143">删除域。</span><span class="sxs-lookup"><span data-stu-id="52346-143">Deletes a domain.</span></span>|
|[<span data-ttu-id="52346-144">ForceDelete 域</span><span class="sxs-lookup"><span data-stu-id="52346-144">ForceDelete domain</span></span>](../api/domain-forcedelete.md)|<span data-ttu-id="52346-145">无</span><span class="sxs-lookup"><span data-stu-id="52346-145">None</span></span>|<span data-ttu-id="52346-146">删除使用异步操作的域。</span><span class="sxs-lookup"><span data-stu-id="52346-146">Deletes a domain using an asynchronous operation.</span></span>|
|[<span data-ttu-id="52346-147">验证域</span><span class="sxs-lookup"><span data-stu-id="52346-147">Verify domain</span></span>](../api/domain-verify.md)|[<span data-ttu-id="52346-148">域</span><span class="sxs-lookup"><span data-stu-id="52346-148">domain</span></span>](domain.md)|<span data-ttu-id="52346-149">验证域的所有权。</span><span class="sxs-lookup"><span data-stu-id="52346-149">Validates the ownership of the domain.</span></span>|

## <a name="properties"></a><span data-ttu-id="52346-150">属性</span><span class="sxs-lookup"><span data-stu-id="52346-150">Properties</span></span>

| <span data-ttu-id="52346-151">属性</span><span class="sxs-lookup"><span data-stu-id="52346-151">Property</span></span>   | <span data-ttu-id="52346-152">类型</span><span class="sxs-lookup"><span data-stu-id="52346-152">Type</span></span> | <span data-ttu-id="52346-153">说明</span><span class="sxs-lookup"><span data-stu-id="52346-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="52346-154">authenticationType</span><span class="sxs-lookup"><span data-stu-id="52346-154">authenticationType</span></span>|<span data-ttu-id="52346-155">String</span><span class="sxs-lookup"><span data-stu-id="52346-155">String</span></span>| <span data-ttu-id="52346-p106">表示为域配置的身份验证类型。此为*托管*或*联盟*值。</span><span class="sxs-lookup"><span data-stu-id="52346-p106">Indicates the configured authentication type for the domain. The value is either *Managed* or *Federated*.</span></span><br> <span data-ttu-id="52346-158">*托管*表示 Azure AD 执行用户身份验证的云托管域。</span><span class="sxs-lookup"><span data-stu-id="52346-158">*Managed* indicates a cloud managed domain where Azure AD performs user authentication.</span></span><br><span data-ttu-id="52346-p107">*联盟*表示身份验证与标识提供程序（如通过 Active Directory 联合身份验证服务的租户的本地 Active Directory）联合。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="52346-p107">*Federated* indicates authentication is federated with an identity provider such as the tenant's on-premises Active Directory via Active Directory Federation Services. Not nullable</span></span> |
|<span data-ttu-id="52346-161">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="52346-161">availabilityStatus</span></span>|<span data-ttu-id="52346-162">String</span><span class="sxs-lookup"><span data-stu-id="52346-162">String</span></span>| <span data-ttu-id="52346-p108">使用[验证](../api/domain-verify.md)操作时，此属性始终为 Null。使用[验证](../api/domain-verify.md)操作时，响应中返回**域**实体。响应中的**域**实体的 **availabilityStatus** 属性为 *AvailableImmediately* 或 *EmailVerifiedDomainTakeoverScheduled*。</span><span class="sxs-lookup"><span data-stu-id="52346-p108">This property is always null except when the [verify](../api/domain-verify.md) action is used. When the [verify](../api/domain-verify.md) action is used, a **domain** entity is returned in the response. The **availabilityStatus** property of the **domain** entity in the response is either *AvailableImmediately* or *EmailVerifiedDomainTakeoverScheduled*.</span></span>|
|<span data-ttu-id="52346-166">id</span><span class="sxs-lookup"><span data-stu-id="52346-166">id</span></span>|<span data-ttu-id="52346-167">字符串</span><span class="sxs-lookup"><span data-stu-id="52346-167">String</span></span>| <span data-ttu-id="52346-p109">域的完全限定的名称。密钥、不可变、不可为 Null、唯一</span><span class="sxs-lookup"><span data-stu-id="52346-p109">The fully qualified name of the domain. Key, immutable, not nullable, unique</span></span> |
|<span data-ttu-id="52346-170">isAdminManaged</span><span class="sxs-lookup"><span data-stu-id="52346-170">isAdminManaged</span></span>|<span data-ttu-id="52346-171">布尔</span><span class="sxs-lookup"><span data-stu-id="52346-171">Boolean</span></span>| <span data-ttu-id="52346-p110">如果域的 DNS 记录管理已委派为 Office 365，则属性值为 false。否则，此值为 true。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="52346-p110">The value of the property is false if the DNS record management of the domain has been delegated to Office 365. Otherwise, the value is true. Not nullable</span></span> |
|<span data-ttu-id="52346-175">isDefault</span><span class="sxs-lookup"><span data-stu-id="52346-175">isDefault</span></span>|<span data-ttu-id="52346-176">布尔</span><span class="sxs-lookup"><span data-stu-id="52346-176">Boolean</span></span>| <span data-ttu-id="52346-p111">如果这是用于创建用户的默认域，则为 true。每个公司仅有一个默认域。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="52346-p111">True if this is the default domain that is used for user creation. There is only one default domain per company. Not nullable</span></span> |
|<span data-ttu-id="52346-180">isInitial</span><span class="sxs-lookup"><span data-stu-id="52346-180">isInitial</span></span>|<span data-ttu-id="52346-181">布尔</span><span class="sxs-lookup"><span data-stu-id="52346-181">Boolean</span></span>| <span data-ttu-id="52346-p112">如果这是由 Microsoft Online Services (companyname.onmicrosoft.com) 创建的初始域，则为 true。每个公司仅有一个初始域。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="52346-p112">True if this is the initial domain created by Microsoft Online Services (companyname.onmicrosoft.com). There is only one initial domain per company. Not nullable</span></span> |
|<span data-ttu-id="52346-185">isRoot</span><span class="sxs-lookup"><span data-stu-id="52346-185">isRoot</span></span>|<span data-ttu-id="52346-186">布尔</span><span class="sxs-lookup"><span data-stu-id="52346-186">Boolean</span></span>| <span data-ttu-id="52346-p113">如果此域是一个已验证的根域，则为 true。否则，如果此域为子域或未经验证，则为 false。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="52346-p113">True if the domain is a verified root domain. Otherwise, false if the domain is a subdomain or unverified. Not nullable</span></span> |
|<span data-ttu-id="52346-190">isVerified</span><span class="sxs-lookup"><span data-stu-id="52346-190">isVerified</span></span>|<span data-ttu-id="52346-191">布尔</span><span class="sxs-lookup"><span data-stu-id="52346-191">Boolean</span></span>| <span data-ttu-id="52346-p114">如果域已完成域所有权验证，则为 true。不可为 Null</span><span class="sxs-lookup"><span data-stu-id="52346-p114">True if the domain has completed domain ownership verification. Not nullable</span></span> |
|<span data-ttu-id="52346-194">supportedServices</span><span class="sxs-lookup"><span data-stu-id="52346-194">supportedServices</span></span>|<span data-ttu-id="52346-195">字符串集合</span><span class="sxs-lookup"><span data-stu-id="52346-195">String collection</span></span>| <span data-ttu-id="52346-196">分配给域的功能。</span><span class="sxs-lookup"><span data-stu-id="52346-196">The capabilities assigned to the domain.</span></span><br><br><span data-ttu-id="52346-197">可以包含下列值中的 0 个、1 个或更多个：*电子邮件*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="52346-197">Can include 0, 1 or more of following values: *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span><br><br> <span data-ttu-id="52346-198">可以使用 Graph API 添加/删除的值包括：*电子邮件*、*OfficeCommunicationsOnline*、*Yammer*</span><span class="sxs-lookup"><span data-stu-id="52346-198">The values which you can add/remove using Graph API include: *Email*, *OfficeCommunicationsOnline*, *Yammer*</span></span><br><span data-ttu-id="52346-199">不可为 Null</span><span class="sxs-lookup"><span data-stu-id="52346-199">Not nullable</span></span>|
|<span data-ttu-id="52346-200">状态</span><span class="sxs-lookup"><span data-stu-id="52346-200">state</span></span>|[<span data-ttu-id="52346-201">domainState</span><span class="sxs-lookup"><span data-stu-id="52346-201">domainState</span></span>](domainstate.md)| <span data-ttu-id="52346-202">为域计划的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="52346-202">Status of asynchronous operations scheduled for the domain.</span></span> |

## <a name="relationships"></a><span data-ttu-id="52346-203">关系</span><span class="sxs-lookup"><span data-stu-id="52346-203">Relationships</span></span>

<span data-ttu-id="52346-p115">通过导航属性公开目录中的域和其他对象之间的关系（如它们的验证记录和服务配置记录）。你可以通过在请求中定位这些导航属性来读取这些关系。</span><span class="sxs-lookup"><span data-stu-id="52346-p115">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties. You can read these relationships by targeting these navigation properties in your requests.</span></span>

| <span data-ttu-id="52346-206">关系</span><span class="sxs-lookup"><span data-stu-id="52346-206">Relationship</span></span> | <span data-ttu-id="52346-207">类型</span><span class="sxs-lookup"><span data-stu-id="52346-207">Type</span></span> |<span data-ttu-id="52346-208">说明</span><span class="sxs-lookup"><span data-stu-id="52346-208">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52346-209">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="52346-209">domainNameReferences</span></span>|<span data-ttu-id="52346-210">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52346-210">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="52346-211">只读，可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="52346-211">Read-only, Nullable</span></span>|
|<span data-ttu-id="52346-212">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="52346-212">serviceConfigurationRecords</span></span>|<span data-ttu-id="52346-213">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52346-213">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="52346-214">Microsoft Online Services 可以使用域之前，客户添加到域 DNS 区域文件的 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="52346-214">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span><br><span data-ttu-id="52346-215">只读，可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="52346-215">Read-only, Nullable</span></span> |
|<span data-ttu-id="52346-216">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="52346-216">verificationDnsRecords</span></span>|<span data-ttu-id="52346-217">[domainDnsRecord](domaindnsrecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52346-217">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="52346-218">客户可以使用 Azure AD 完成域所有权验证之前，客户添加到域 DNS 区域文件的 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="52346-218">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span><br><span data-ttu-id="52346-219">只读，可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="52346-219">Read-only, Nullable</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52346-220">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52346-220">JSON representation</span></span>
<span data-ttu-id="52346-221">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52346-221">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
