---
title: domainDnsCnameRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件中的 CNAME 记录。 继承自 DomainDnsRecord 实体。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb730cafd1689ab95563fa1e4dd6ea23962af903
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340685"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="3b29a-104">domainDnsCnameRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b29a-104">domainDnsCnameRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b29a-105">表示添加到租户中特定域的 DNS 区域文件中的 CNAME 记录。</span><span class="sxs-lookup"><span data-stu-id="3b29a-105">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="3b29a-106">继承自[DomainDnsRecord](domaindnsrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="3b29a-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="3b29a-107">方法</span><span class="sxs-lookup"><span data-stu-id="3b29a-107">Methods</span></span>
<span data-ttu-id="3b29a-108">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="3b29a-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="3b29a-109">有关如何查询域服务记录的信息, 请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="3b29a-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="3b29a-110">属性</span><span class="sxs-lookup"><span data-stu-id="3b29a-110">Properties</span></span>
| <span data-ttu-id="3b29a-111">属性</span><span class="sxs-lookup"><span data-stu-id="3b29a-111">Property</span></span>     | <span data-ttu-id="3b29a-112">类型</span><span class="sxs-lookup"><span data-stu-id="3b29a-112">Type</span></span>   |<span data-ttu-id="3b29a-113">说明</span><span class="sxs-lookup"><span data-stu-id="3b29a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b29a-114">canonicalName</span><span class="sxs-lookup"><span data-stu-id="3b29a-114">canonicalName</span></span>|<span data-ttu-id="3b29a-115">String</span><span class="sxs-lookup"><span data-stu-id="3b29a-115">String</span></span>| <span data-ttu-id="3b29a-116">CNAME 记录的规范名称。</span><span class="sxs-lookup"><span data-stu-id="3b29a-116">The canonical name of the CNAME record.</span></span> <span data-ttu-id="3b29a-117">用于配置 DNS 主机上的 CNAME 记录。</span><span class="sxs-lookup"><span data-stu-id="3b29a-117">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="3b29a-118">id</span><span class="sxs-lookup"><span data-stu-id="3b29a-118">id</span></span>|<span data-ttu-id="3b29a-119">String</span><span class="sxs-lookup"><span data-stu-id="3b29a-119">String</span></span>| <span data-ttu-id="3b29a-120">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3b29a-120">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="3b29a-121">不可为 null 的只读</span><span class="sxs-lookup"><span data-stu-id="3b29a-121">Not nullable, Read-only</span></span>|
|<span data-ttu-id="3b29a-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="3b29a-122">isOptional</span></span>|<span data-ttu-id="3b29a-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b29a-123">Boolean</span></span>| <span data-ttu-id="3b29a-124">如果为 false, 则客户必须在 DNS 主机上配置 CNAME 记录, 才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="3b29a-124">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="3b29a-125">不可为 null</span><span class="sxs-lookup"><span data-stu-id="3b29a-125">Not nullable</span></span> |
|<span data-ttu-id="3b29a-126">label</span><span class="sxs-lookup"><span data-stu-id="3b29a-126">label</span></span>|<span data-ttu-id="3b29a-127">String</span><span class="sxs-lookup"><span data-stu-id="3b29a-127">String</span></span>| <span data-ttu-id="3b29a-128">配置 DNS 主机上的 CNAME 记录的*别名/主机/名称*时使用的值。</span><span class="sxs-lookup"><span data-stu-id="3b29a-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="3b29a-129">recordType</span><span class="sxs-lookup"><span data-stu-id="3b29a-129">recordType</span></span>|<span data-ttu-id="3b29a-130">String</span><span class="sxs-lookup"><span data-stu-id="3b29a-130">String</span></span>| <span data-ttu-id="3b29a-131">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="3b29a-131">Type of DNS record.</span></span> <span data-ttu-id="3b29a-132">值始终为*CName*。</span><span class="sxs-lookup"><span data-stu-id="3b29a-132">The value is always *CName*.</span></span> <span data-ttu-id="3b29a-133">Key</span><span class="sxs-lookup"><span data-stu-id="3b29a-133">Key</span></span>|
|<span data-ttu-id="3b29a-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="3b29a-134">supportedService</span></span>|<span data-ttu-id="3b29a-135">String</span><span class="sxs-lookup"><span data-stu-id="3b29a-135">String</span></span>| <span data-ttu-id="3b29a-136">对此 CNAME 记录具有依赖关系的 Microsoft Online 服务或功能。</span><span class="sxs-lookup"><span data-stu-id="3b29a-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="3b29a-137">可以是下列值之一: **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="3b29a-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="3b29a-138">ttl</span><span class="sxs-lookup"><span data-stu-id="3b29a-138">ttl</span></span>|<span data-ttu-id="3b29a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3b29a-139">Int32</span></span>| <span data-ttu-id="3b29a-140">配置 DNS 主机上的 CNAME 记录的生存时间 (ttl) 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="3b29a-140">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="3b29a-141">不可为 null</span><span class="sxs-lookup"><span data-stu-id="3b29a-141">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="3b29a-142">关系</span><span class="sxs-lookup"><span data-stu-id="3b29a-142">Relationships</span></span>
<span data-ttu-id="3b29a-143">无</span><span class="sxs-lookup"><span data-stu-id="3b29a-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3b29a-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b29a-144">JSON representation</span></span>
<span data-ttu-id="3b29a-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b29a-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
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
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
