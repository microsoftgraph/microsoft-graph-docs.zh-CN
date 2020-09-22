---
title: domainDnsSrvRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件中的 SRV 记录。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6854b30dec759726fefaf93e13ad23a49195e381
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010325"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="8ef9d-103">domainDnsSrvRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ef9d-103">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="8ef9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ef9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ef9d-105">表示添加到租户中特定域的 DNS 区域文件中的 SRV 记录。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-105">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="8ef9d-106">继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="8ef9d-107">方法</span><span class="sxs-lookup"><span data-stu-id="8ef9d-107">Methods</span></span>
<span data-ttu-id="8ef9d-108">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="8ef9d-109">有关如何查询域服务记录的信息，请参阅 [域](domain.md) 主题。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="8ef9d-110">属性</span><span class="sxs-lookup"><span data-stu-id="8ef9d-110">Properties</span></span>
| <span data-ttu-id="8ef9d-111">属性</span><span class="sxs-lookup"><span data-stu-id="8ef9d-111">Property</span></span>     | <span data-ttu-id="8ef9d-112">类型</span><span class="sxs-lookup"><span data-stu-id="8ef9d-112">Type</span></span>   |<span data-ttu-id="8ef9d-113">说明</span><span class="sxs-lookup"><span data-stu-id="8ef9d-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ef9d-114">id</span><span class="sxs-lookup"><span data-stu-id="8ef9d-114">id</span></span>|<span data-ttu-id="8ef9d-115">String</span><span class="sxs-lookup"><span data-stu-id="8ef9d-115">String</span></span>| <span data-ttu-id="8ef9d-116">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="8ef9d-117">不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="8ef9d-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="8ef9d-118">isOptional</span></span>|<span data-ttu-id="8ef9d-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ef9d-119">Boolean</span></span>| <span data-ttu-id="8ef9d-120">如果为 false，则客户必须在 DNS 主机上配置 SRV 记录，才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="8ef9d-121">label</span><span class="sxs-lookup"><span data-stu-id="8ef9d-121">label</span></span>|<span data-ttu-id="8ef9d-122">String</span><span class="sxs-lookup"><span data-stu-id="8ef9d-122">String</span></span>| <span data-ttu-id="8ef9d-123">配置 DNS 主机上的 SRV 记录的 *name* 属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8ef9d-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="8ef9d-124">nameTarget</span></span>|<span data-ttu-id="8ef9d-125">String</span><span class="sxs-lookup"><span data-stu-id="8ef9d-125">String</span></span>| <span data-ttu-id="8ef9d-126">配置 DNS 主机上的 SRV 记录的 *目标* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8ef9d-127">端口</span><span class="sxs-lookup"><span data-stu-id="8ef9d-127">port</span></span>|<span data-ttu-id="8ef9d-128">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef9d-128">Int32</span></span>| <span data-ttu-id="8ef9d-129">配置 DNS 主机上的 SRV 记录的 *port* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8ef9d-130">priority</span><span class="sxs-lookup"><span data-stu-id="8ef9d-130">priority</span></span>|<span data-ttu-id="8ef9d-131">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef9d-131">Int32</span></span>| <span data-ttu-id="8ef9d-132">配置 DNS 主机上的 SRV 记录的 *优先级* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8ef9d-133">协议</span><span class="sxs-lookup"><span data-stu-id="8ef9d-133">protocol</span></span>|<span data-ttu-id="8ef9d-134">String</span><span class="sxs-lookup"><span data-stu-id="8ef9d-134">String</span></span>| <span data-ttu-id="8ef9d-135">配置 DNS 主机上的 SRV 记录的 *协议* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8ef9d-136">recordType</span><span class="sxs-lookup"><span data-stu-id="8ef9d-136">recordType</span></span>|<span data-ttu-id="8ef9d-137">String</span><span class="sxs-lookup"><span data-stu-id="8ef9d-137">String</span></span>|  <span data-ttu-id="8ef9d-138">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-138">Type of DNS record.</span></span> <span data-ttu-id="8ef9d-139">该值始终为 *Srv*。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-139">The value is always *Srv*.</span></span> <span data-ttu-id="8ef9d-140">键</span><span class="sxs-lookup"><span data-stu-id="8ef9d-140">Key</span></span> |
|<span data-ttu-id="8ef9d-141">service</span><span class="sxs-lookup"><span data-stu-id="8ef9d-141">service</span></span>|<span data-ttu-id="8ef9d-142">String</span><span class="sxs-lookup"><span data-stu-id="8ef9d-142">String</span></span>| <span data-ttu-id="8ef9d-143">配置 DNS 主机上的 SRV 记录的 *服务* 属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8ef9d-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="8ef9d-144">supportedService</span></span>|<span data-ttu-id="8ef9d-145">String</span><span class="sxs-lookup"><span data-stu-id="8ef9d-145">String</span></span>| <span data-ttu-id="8ef9d-146">依赖于此 SRV 记录的 Microsoft Online 服务或功能。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="8ef9d-147">可以是下列值之一： **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="8ef9d-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="8ef9d-148">ttl</span><span class="sxs-lookup"><span data-stu-id="8ef9d-148">ttl</span></span>|<span data-ttu-id="8ef9d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef9d-149">Int32</span></span>| <span data-ttu-id="8ef9d-150">配置 DNS 主机上的 SRV 记录的 \*生存时间 (ttl) \* 属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-150">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="8ef9d-151">不可为 null</span><span class="sxs-lookup"><span data-stu-id="8ef9d-151">Not nullable</span></span> |
|<span data-ttu-id="8ef9d-152">weight</span><span class="sxs-lookup"><span data-stu-id="8ef9d-152">weight</span></span>|<span data-ttu-id="8ef9d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8ef9d-153">Int32</span></span>| <span data-ttu-id="8ef9d-154">配置 DNS 主机上的 SRV 记录的 *权重* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8ef9d-155">关系</span><span class="sxs-lookup"><span data-stu-id="8ef9d-155">Relationships</span></span>
<span data-ttu-id="8ef9d-156">无</span><span class="sxs-lookup"><span data-stu-id="8ef9d-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8ef9d-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ef9d-157">JSON representation</span></span>
<span data-ttu-id="8ef9d-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ef9d-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


