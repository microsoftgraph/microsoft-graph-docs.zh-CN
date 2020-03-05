---
title: domainDnsRecord 资源类型
description: 对于租户中的每个域，您可能需要将 DNS 记录添加到域的 DNS 区域文件中，然后 Microsoft Online Services 才能使用域。 **DomainDnsRecord**实体用于提供此类 DNS 记录。 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord 和 DomainDnsTxtRecord 实体的基本实体。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4eb36c4d57826dab8e2da83eeab2bfaf577008c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506293"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="002b0-105">domainDnsRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="002b0-105">domainDnsRecord resource type</span></span>

<span data-ttu-id="002b0-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="002b0-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="002b0-107">对于租户中的每个域，您可能需要将 DNS 记录添加到域的 DNS 区域文件中，然后 Microsoft Online Services 才能使用域。</span><span class="sxs-lookup"><span data-stu-id="002b0-107">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="002b0-108">**DomainDnsRecord**实体用于提供此类 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="002b0-108">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="002b0-109">[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md)和[DomainDnsTxtRecord](domaindnstxtrecord.md)实体的基本实体。</span><span class="sxs-lookup"><span data-stu-id="002b0-109">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="002b0-110">方法</span><span class="sxs-lookup"><span data-stu-id="002b0-110">Methods</span></span>
<span data-ttu-id="002b0-111">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="002b0-111">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="002b0-112">有关如何查询域服务记录的信息，请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="002b0-112">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="002b0-113">属性</span><span class="sxs-lookup"><span data-stu-id="002b0-113">Properties</span></span>
| <span data-ttu-id="002b0-114">属性</span><span class="sxs-lookup"><span data-stu-id="002b0-114">Property</span></span>     | <span data-ttu-id="002b0-115">类型</span><span class="sxs-lookup"><span data-stu-id="002b0-115">Type</span></span>   |<span data-ttu-id="002b0-116">说明</span><span class="sxs-lookup"><span data-stu-id="002b0-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="002b0-117">id</span><span class="sxs-lookup"><span data-stu-id="002b0-117">id</span></span>|<span data-ttu-id="002b0-118">String</span><span class="sxs-lookup"><span data-stu-id="002b0-118">String</span></span>| <span data-ttu-id="002b0-119">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="002b0-119">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="002b0-120">不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="002b0-120">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="002b0-121">isOptional</span><span class="sxs-lookup"><span data-stu-id="002b0-121">isOptional</span></span>|<span data-ttu-id="002b0-122">布尔</span><span class="sxs-lookup"><span data-stu-id="002b0-122">Boolean</span></span>| <span data-ttu-id="002b0-123">如果为 false，则客户必须在 DNS 主机上配置此记录，才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="002b0-123">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="002b0-124">label</span><span class="sxs-lookup"><span data-stu-id="002b0-124">label</span></span>|<span data-ttu-id="002b0-125">String</span><span class="sxs-lookup"><span data-stu-id="002b0-125">String</span></span>| <span data-ttu-id="002b0-126">在 DNS 主机上配置 DNS 记录名称时使用的值。</span><span class="sxs-lookup"><span data-stu-id="002b0-126">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="002b0-127">recordType</span><span class="sxs-lookup"><span data-stu-id="002b0-127">recordType</span></span>|<span data-ttu-id="002b0-128">String</span><span class="sxs-lookup"><span data-stu-id="002b0-128">String</span></span>| <span data-ttu-id="002b0-129">指示此实体表示的 DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="002b0-129">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="002b0-130">此值可以是下列值之一： *CName*、 *Mx*、 *Srv*、 *Txt*</span><span class="sxs-lookup"><span data-stu-id="002b0-130">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="002b0-131">键</span><span class="sxs-lookup"><span data-stu-id="002b0-131">Key</span></span> |
|<span data-ttu-id="002b0-132">supportedService</span><span class="sxs-lookup"><span data-stu-id="002b0-132">supportedService</span></span>|<span data-ttu-id="002b0-133">String</span><span class="sxs-lookup"><span data-stu-id="002b0-133">String</span></span>| <span data-ttu-id="002b0-134">对此 DNS 记录具有依赖项的 Microsoft Online 服务或功能。</span><span class="sxs-lookup"><span data-stu-id="002b0-134">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="002b0-135">可以是下列值之一： **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="002b0-135">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="002b0-136">ttl</span><span class="sxs-lookup"><span data-stu-id="002b0-136">ttl</span></span>|<span data-ttu-id="002b0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="002b0-137">Int32</span></span>| <span data-ttu-id="002b0-138">配置 DNS 主机上的 DNS 记录的生存时间（ttl）属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="002b0-138">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="002b0-139">不可为 null</span><span class="sxs-lookup"><span data-stu-id="002b0-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="002b0-140">关系</span><span class="sxs-lookup"><span data-stu-id="002b0-140">Relationships</span></span>
<span data-ttu-id="002b0-141">无</span><span class="sxs-lookup"><span data-stu-id="002b0-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="002b0-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="002b0-142">JSON representation</span></span>
<span data-ttu-id="002b0-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="002b0-143">Here is a JSON representation of the resource.</span></span>

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
