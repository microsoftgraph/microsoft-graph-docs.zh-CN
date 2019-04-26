---
title: domainDnsRecord 资源类型
description: 对于租户中的每个域, 您可能需要将 dns 记录添加到域的 dns 区域文件中, 然后 Microsoft Online Services 才能使用域。 **DomainDnsRecord**实体用于提供此类 DNS 记录。 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord 和 DomainDnsSrvRecord 实体的基本实体。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: da969956616d22f5b13041b1a7bc4ebcdb510565
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340649"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="4db0f-105">domainDnsRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="4db0f-105">domainDnsRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4db0f-106">对于租户中的每个域, 您可能需要将 dns 记录添加到域的 dns 区域文件中, 然后 Microsoft Online Services 才能使用域。</span><span class="sxs-lookup"><span data-stu-id="4db0f-106">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="4db0f-107">**DomainDnsRecord**实体用于提供此类 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="4db0f-107">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="4db0f-108">[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md)和[DomainDnsSrvRecord](domaindnssrvrecord.md)实体的基本实体。</span><span class="sxs-lookup"><span data-stu-id="4db0f-108">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="4db0f-109">方法</span><span class="sxs-lookup"><span data-stu-id="4db0f-109">Methods</span></span>
<span data-ttu-id="4db0f-110">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="4db0f-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="4db0f-111">有关如何查询域服务记录的信息, 请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="4db0f-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="4db0f-112">属性</span><span class="sxs-lookup"><span data-stu-id="4db0f-112">Properties</span></span>
| <span data-ttu-id="4db0f-113">属性</span><span class="sxs-lookup"><span data-stu-id="4db0f-113">Property</span></span>     | <span data-ttu-id="4db0f-114">类型</span><span class="sxs-lookup"><span data-stu-id="4db0f-114">Type</span></span>   |<span data-ttu-id="4db0f-115">说明</span><span class="sxs-lookup"><span data-stu-id="4db0f-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4db0f-116">id</span><span class="sxs-lookup"><span data-stu-id="4db0f-116">id</span></span>|<span data-ttu-id="4db0f-117">String</span><span class="sxs-lookup"><span data-stu-id="4db0f-117">String</span></span>| <span data-ttu-id="4db0f-118">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4db0f-118">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="4db0f-119">不可为 null, 只读。</span><span class="sxs-lookup"><span data-stu-id="4db0f-119">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="4db0f-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="4db0f-120">isOptional</span></span>|<span data-ttu-id="4db0f-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db0f-121">Boolean</span></span>| <span data-ttu-id="4db0f-122">如果为 false, 则客户必须在 DNS 主机上配置此记录, 才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="4db0f-122">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="4db0f-123">label</span><span class="sxs-lookup"><span data-stu-id="4db0f-123">label</span></span>|<span data-ttu-id="4db0f-124">String</span><span class="sxs-lookup"><span data-stu-id="4db0f-124">String</span></span>| <span data-ttu-id="4db0f-125">在 dns 主机上配置 dns 记录名称时使用的值。</span><span class="sxs-lookup"><span data-stu-id="4db0f-125">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="4db0f-126">recordType</span><span class="sxs-lookup"><span data-stu-id="4db0f-126">recordType</span></span>|<span data-ttu-id="4db0f-127">String</span><span class="sxs-lookup"><span data-stu-id="4db0f-127">String</span></span>| <span data-ttu-id="4db0f-128">指示此实体表示的 DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="4db0f-128">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="4db0f-129">此值可以是下列值之一: *CName*、 *Mx*、 *Srv*、 *Txt*</span><span class="sxs-lookup"><span data-stu-id="4db0f-129">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="4db0f-130">Key</span><span class="sxs-lookup"><span data-stu-id="4db0f-130">Key</span></span> |
|<span data-ttu-id="4db0f-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="4db0f-131">supportedService</span></span>|<span data-ttu-id="4db0f-132">String</span><span class="sxs-lookup"><span data-stu-id="4db0f-132">String</span></span>| <span data-ttu-id="4db0f-133">对此 DNS 记录具有依赖项的 Microsoft Online 服务或功能。</span><span class="sxs-lookup"><span data-stu-id="4db0f-133">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="4db0f-134">可以是下列值之一: **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="4db0f-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="4db0f-135">ttl</span><span class="sxs-lookup"><span data-stu-id="4db0f-135">ttl</span></span>|<span data-ttu-id="4db0f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4db0f-136">Int32</span></span>| <span data-ttu-id="4db0f-137">配置 dns 主机上的 dns 记录的生存时间 (ttl) 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="4db0f-137">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="4db0f-138">不可为 null</span><span class="sxs-lookup"><span data-stu-id="4db0f-138">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="4db0f-139">关系</span><span class="sxs-lookup"><span data-stu-id="4db0f-139">Relationships</span></span>
<span data-ttu-id="4db0f-140">无</span><span class="sxs-lookup"><span data-stu-id="4db0f-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4db0f-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4db0f-141">JSON representation</span></span>
<span data-ttu-id="4db0f-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4db0f-142">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
