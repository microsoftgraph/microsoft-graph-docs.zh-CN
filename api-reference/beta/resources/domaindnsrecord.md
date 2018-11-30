---
title: domainDnsRecord 资源类型
description: 对于租户中的每个域，您可能需要先域可由 Microsoft Online Services 将 DNS 记录添加到域的 DNS 区域文件。 **DomainDnsRecord**实体用于显示此类的 DNS 记录。 DomainDnsCnameRecord、 DomainDnsMxRecord、 DomainDnsSrvRecord 和 DomainDnsSrvRecord 实体的基准实体。
ms.openlocfilehash: 766e3b241550ac1b0c7abdecaa22fe010955d05a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042204"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="7b2fd-105">domainDnsRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b2fd-105">domainDnsRecord resource type</span></span>

> <span data-ttu-id="7b2fd-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7b2fd-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b2fd-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7b2fd-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b2fd-p103">对于租户中的每个域，可能需要先将 DNS 记录添加到相应域的 DNS 区域文件，然后 Microsoft Online Services 才能使用该域。**DomainDnsRecord** 实体用于显示这些 DNS 记录。[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) 和 [DomainDnsSrvRecord](domaindnssrvrecord.md) 实体的基本实体。</span><span class="sxs-lookup"><span data-stu-id="7b2fd-p103">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="7b2fd-111">方法</span><span class="sxs-lookup"><span data-stu-id="7b2fd-111">Methods</span></span>
<span data-ttu-id="7b2fd-p104">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="7b2fd-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="7b2fd-114">属性</span><span class="sxs-lookup"><span data-stu-id="7b2fd-114">Properties</span></span>
| <span data-ttu-id="7b2fd-115">属性</span><span class="sxs-lookup"><span data-stu-id="7b2fd-115">Property</span></span>     | <span data-ttu-id="7b2fd-116">类型</span><span class="sxs-lookup"><span data-stu-id="7b2fd-116">Type</span></span>   |<span data-ttu-id="7b2fd-117">说明</span><span class="sxs-lookup"><span data-stu-id="7b2fd-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b2fd-118">id</span><span class="sxs-lookup"><span data-stu-id="7b2fd-118">id</span></span>|<span data-ttu-id="7b2fd-119">字符串</span><span class="sxs-lookup"><span data-stu-id="7b2fd-119">String</span></span>| <span data-ttu-id="7b2fd-p105">分配给此实体的唯一标识符。不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="7b2fd-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="7b2fd-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="7b2fd-122">isOptional</span></span>|<span data-ttu-id="7b2fd-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b2fd-123">Boolean</span></span>| <span data-ttu-id="7b2fd-124">如果为 false，则客户必须在 DNS 主机上配置此记录才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="7b2fd-124">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="7b2fd-125">label</span><span class="sxs-lookup"><span data-stu-id="7b2fd-125">label</span></span>|<span data-ttu-id="7b2fd-126">String</span><span class="sxs-lookup"><span data-stu-id="7b2fd-126">String</span></span>| <span data-ttu-id="7b2fd-127">配置 DNS 主机上的 DNS 记录的名称时使用的值。</span><span class="sxs-lookup"><span data-stu-id="7b2fd-127">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="7b2fd-128">recordType</span><span class="sxs-lookup"><span data-stu-id="7b2fd-128">recordType</span></span>|<span data-ttu-id="7b2fd-129">String</span><span class="sxs-lookup"><span data-stu-id="7b2fd-129">String</span></span>| <span data-ttu-id="7b2fd-130">指示此实体表示的 DNS 记录类型。</span><span class="sxs-lookup"><span data-stu-id="7b2fd-130">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="7b2fd-131">值可以是下列值之一：*CName*、*Mx*、*Srv*、*Txt*</span><span class="sxs-lookup"><span data-stu-id="7b2fd-131">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="7b2fd-132">Key</span><span class="sxs-lookup"><span data-stu-id="7b2fd-132">Key</span></span> |
|<span data-ttu-id="7b2fd-133">supportedService</span><span class="sxs-lookup"><span data-stu-id="7b2fd-133">supportedService</span></span>|<span data-ttu-id="7b2fd-134">String</span><span class="sxs-lookup"><span data-stu-id="7b2fd-134">String</span></span>| <span data-ttu-id="7b2fd-135">Microsoft Online Service 或与该 DNS 记录存在依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="7b2fd-135">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="7b2fd-136">可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="7b2fd-136">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="7b2fd-137">ttl</span><span class="sxs-lookup"><span data-stu-id="7b2fd-137">ttl</span></span>|<span data-ttu-id="7b2fd-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7b2fd-138">Int32</span></span>| <span data-ttu-id="7b2fd-p106">配置 DNS 主机上的 DNS 记录的生存时间 (ttl) 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="7b2fd-p106">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="7b2fd-141">关系</span><span class="sxs-lookup"><span data-stu-id="7b2fd-141">Relationships</span></span>
<span data-ttu-id="7b2fd-142">无</span><span class="sxs-lookup"><span data-stu-id="7b2fd-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b2fd-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b2fd-143">JSON representation</span></span>
<span data-ttu-id="7b2fd-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b2fd-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->