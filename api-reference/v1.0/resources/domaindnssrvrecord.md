---
title: domainDnsSrvRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件中的 SRV 记录。 继承自 DomainDnsRecord 实体。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 32a9461cb28bc51489ddca6f3b569871bcc584d0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531596"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="8a140-104">domainDnsSrvRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a140-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="8a140-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a140-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a140-106">表示添加到租户中特定域的 DNS 区域文件中的 SRV 记录。</span><span class="sxs-lookup"><span data-stu-id="8a140-106">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="8a140-107">继承自[DomainDnsRecord](domaindnsrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="8a140-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="8a140-108">Methods</span><span class="sxs-lookup"><span data-stu-id="8a140-108">Methods</span></span>
<span data-ttu-id="8a140-109">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="8a140-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="8a140-110">有关如何查询域服务记录的信息，请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="8a140-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="8a140-111">属性</span><span class="sxs-lookup"><span data-stu-id="8a140-111">Properties</span></span>
| <span data-ttu-id="8a140-112">属性</span><span class="sxs-lookup"><span data-stu-id="8a140-112">Property</span></span>     | <span data-ttu-id="8a140-113">类型</span><span class="sxs-lookup"><span data-stu-id="8a140-113">Type</span></span>   |<span data-ttu-id="8a140-114">说明</span><span class="sxs-lookup"><span data-stu-id="8a140-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a140-115">id</span><span class="sxs-lookup"><span data-stu-id="8a140-115">id</span></span>|<span data-ttu-id="8a140-116">字符串</span><span class="sxs-lookup"><span data-stu-id="8a140-116">String</span></span>| <span data-ttu-id="8a140-117">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8a140-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="8a140-118">不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="8a140-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="8a140-119">isOptional</span><span class="sxs-lookup"><span data-stu-id="8a140-119">isOptional</span></span>|<span data-ttu-id="8a140-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a140-120">Boolean</span></span>| <span data-ttu-id="8a140-121">如果为 false，则客户必须在 DNS 主机上配置 SRV 记录，才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="8a140-121">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="8a140-122">label</span><span class="sxs-lookup"><span data-stu-id="8a140-122">label</span></span>|<span data-ttu-id="8a140-123">字符串</span><span class="sxs-lookup"><span data-stu-id="8a140-123">String</span></span>| <span data-ttu-id="8a140-124">配置 DNS 主机上的 SRV 记录的*name*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="8a140-124">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8a140-125">nameTarget</span><span class="sxs-lookup"><span data-stu-id="8a140-125">nameTarget</span></span>|<span data-ttu-id="8a140-126">字符串</span><span class="sxs-lookup"><span data-stu-id="8a140-126">String</span></span>| <span data-ttu-id="8a140-127">配置 DNS 主机上的 SRV 记录的*目标*属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8a140-127">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8a140-128">端口</span><span class="sxs-lookup"><span data-stu-id="8a140-128">port</span></span>|<span data-ttu-id="8a140-129">Int32</span><span class="sxs-lookup"><span data-stu-id="8a140-129">Int32</span></span>| <span data-ttu-id="8a140-130">配置 DNS 主机上的 SRV 记录的*port*属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8a140-130">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8a140-131">priority</span><span class="sxs-lookup"><span data-stu-id="8a140-131">priority</span></span>|<span data-ttu-id="8a140-132">Int32</span><span class="sxs-lookup"><span data-stu-id="8a140-132">Int32</span></span>| <span data-ttu-id="8a140-133">配置 DNS 主机上的 SRV 记录的*优先级*属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8a140-133">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8a140-134">协议</span><span class="sxs-lookup"><span data-stu-id="8a140-134">protocol</span></span>|<span data-ttu-id="8a140-135">字符串</span><span class="sxs-lookup"><span data-stu-id="8a140-135">String</span></span>| <span data-ttu-id="8a140-136">配置 DNS 主机上的 SRV 记录的*协议*属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8a140-136">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8a140-137">recordType</span><span class="sxs-lookup"><span data-stu-id="8a140-137">recordType</span></span>|<span data-ttu-id="8a140-138">字符串</span><span class="sxs-lookup"><span data-stu-id="8a140-138">String</span></span>|  <span data-ttu-id="8a140-139">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="8a140-139">Type of DNS record.</span></span> <span data-ttu-id="8a140-140">该值始终为*Srv*。</span><span class="sxs-lookup"><span data-stu-id="8a140-140">The value is always *Srv*.</span></span> <span data-ttu-id="8a140-141">键</span><span class="sxs-lookup"><span data-stu-id="8a140-141">Key</span></span> |
|<span data-ttu-id="8a140-142">service</span><span class="sxs-lookup"><span data-stu-id="8a140-142">service</span></span>|<span data-ttu-id="8a140-143">String</span><span class="sxs-lookup"><span data-stu-id="8a140-143">String</span></span>| <span data-ttu-id="8a140-144">配置 DNS 主机上的 SRV 记录的*服务*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="8a140-144">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="8a140-145">supportedService</span><span class="sxs-lookup"><span data-stu-id="8a140-145">supportedService</span></span>|<span data-ttu-id="8a140-146">字符串</span><span class="sxs-lookup"><span data-stu-id="8a140-146">String</span></span>| <span data-ttu-id="8a140-147">依赖于此 SRV 记录的 Microsoft Online 服务或功能。</span><span class="sxs-lookup"><span data-stu-id="8a140-147">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="8a140-148">可以是下列值之一： **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="8a140-148">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="8a140-149">ttl</span><span class="sxs-lookup"><span data-stu-id="8a140-149">ttl</span></span>|<span data-ttu-id="8a140-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8a140-150">Int32</span></span>| <span data-ttu-id="8a140-151">配置 DNS 主机上的 SRV 记录的*生存时间（ttl）* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8a140-151">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="8a140-152">不可为 null</span><span class="sxs-lookup"><span data-stu-id="8a140-152">Not nullable</span></span> |
|<span data-ttu-id="8a140-153">weight</span><span class="sxs-lookup"><span data-stu-id="8a140-153">weight</span></span>|<span data-ttu-id="8a140-154">Int32</span><span class="sxs-lookup"><span data-stu-id="8a140-154">Int32</span></span>| <span data-ttu-id="8a140-155">配置 DNS 主机上的 SRV 记录的*权重*属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8a140-155">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8a140-156">关系</span><span class="sxs-lookup"><span data-stu-id="8a140-156">Relationships</span></span>
<span data-ttu-id="8a140-157">无</span><span class="sxs-lookup"><span data-stu-id="8a140-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8a140-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a140-158">JSON representation</span></span>
<span data-ttu-id="8a140-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a140-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
