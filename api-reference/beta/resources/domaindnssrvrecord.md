---
title: domainDnsSrvRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件的 SRV 记录。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5b3355115f11937584879725073cd4a4c279c62d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761672"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="c70dc-103">domainDnsSrvRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="c70dc-103">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="c70dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c70dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c70dc-105">表示添加到租户中特定域的 DNS 区域文件的 SRV 记录。</span><span class="sxs-lookup"><span data-stu-id="c70dc-105">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="c70dc-106">继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="c70dc-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="c70dc-107">方法</span><span class="sxs-lookup"><span data-stu-id="c70dc-107">Methods</span></span>
<span data-ttu-id="c70dc-108">不支持直接查询此资源。</span><span class="sxs-lookup"><span data-stu-id="c70dc-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="c70dc-109">请参阅 [域主题](domain.md) ，了解如何查询域服务记录。</span><span class="sxs-lookup"><span data-stu-id="c70dc-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="c70dc-110">属性</span><span class="sxs-lookup"><span data-stu-id="c70dc-110">Properties</span></span>
| <span data-ttu-id="c70dc-111">属性</span><span class="sxs-lookup"><span data-stu-id="c70dc-111">Property</span></span>     | <span data-ttu-id="c70dc-112">类型</span><span class="sxs-lookup"><span data-stu-id="c70dc-112">Type</span></span>   |<span data-ttu-id="c70dc-113">说明</span><span class="sxs-lookup"><span data-stu-id="c70dc-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c70dc-114">id</span><span class="sxs-lookup"><span data-stu-id="c70dc-114">id</span></span>|<span data-ttu-id="c70dc-115">String</span><span class="sxs-lookup"><span data-stu-id="c70dc-115">String</span></span>| <span data-ttu-id="c70dc-116">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c70dc-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="c70dc-117">不可为空，只读。</span><span class="sxs-lookup"><span data-stu-id="c70dc-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="c70dc-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="c70dc-118">isOptional</span></span>|<span data-ttu-id="c70dc-119">布尔</span><span class="sxs-lookup"><span data-stu-id="c70dc-119">Boolean</span></span>| <span data-ttu-id="c70dc-120">如果为 false，则客户必须在 DNS 主机上配置 SRV 记录，Microsoft Online Services该域正常运行。</span><span class="sxs-lookup"><span data-stu-id="c70dc-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="c70dc-121">label</span><span class="sxs-lookup"><span data-stu-id="c70dc-121">label</span></span>|<span data-ttu-id="c70dc-122">String</span><span class="sxs-lookup"><span data-stu-id="c70dc-122">String</span></span>| <span data-ttu-id="c70dc-123">在 DNS 主机上配置 SRV 记录的名称属性时所使用的值。</span><span class="sxs-lookup"><span data-stu-id="c70dc-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c70dc-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="c70dc-124">nameTarget</span></span>|<span data-ttu-id="c70dc-125">String</span><span class="sxs-lookup"><span data-stu-id="c70dc-125">String</span></span>| <span data-ttu-id="c70dc-126">在 DNS 主机上配置 SRV 记录的 *Target* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="c70dc-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c70dc-127">端口</span><span class="sxs-lookup"><span data-stu-id="c70dc-127">port</span></span>|<span data-ttu-id="c70dc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c70dc-128">Int32</span></span>| <span data-ttu-id="c70dc-129">在 DNS 主机上配置 SRV 记录的 *端口* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="c70dc-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c70dc-130">priority</span><span class="sxs-lookup"><span data-stu-id="c70dc-130">priority</span></span>|<span data-ttu-id="c70dc-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c70dc-131">Int32</span></span>| <span data-ttu-id="c70dc-132">在 DNS 主机上配置SRV 记录的优先级属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="c70dc-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c70dc-133">协议</span><span class="sxs-lookup"><span data-stu-id="c70dc-133">protocol</span></span>|<span data-ttu-id="c70dc-134">String</span><span class="sxs-lookup"><span data-stu-id="c70dc-134">String</span></span>| <span data-ttu-id="c70dc-135">在 DNS 主机上配置SRV 记录的协议属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="c70dc-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c70dc-136">recordType</span><span class="sxs-lookup"><span data-stu-id="c70dc-136">recordType</span></span>|<span data-ttu-id="c70dc-137">String</span><span class="sxs-lookup"><span data-stu-id="c70dc-137">String</span></span>|  <span data-ttu-id="c70dc-138">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="c70dc-138">Type of DNS record.</span></span> <span data-ttu-id="c70dc-139">该值始终为 *Srv*。</span><span class="sxs-lookup"><span data-stu-id="c70dc-139">The value is always *Srv*.</span></span> <span data-ttu-id="c70dc-140">键</span><span class="sxs-lookup"><span data-stu-id="c70dc-140">Key</span></span> |
|<span data-ttu-id="c70dc-141">service</span><span class="sxs-lookup"><span data-stu-id="c70dc-141">service</span></span>|<span data-ttu-id="c70dc-142">String</span><span class="sxs-lookup"><span data-stu-id="c70dc-142">String</span></span>| <span data-ttu-id="c70dc-143">在 DNS 主机上配置SRV 记录的服务属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="c70dc-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c70dc-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="c70dc-144">supportedService</span></span>|<span data-ttu-id="c70dc-145">String</span><span class="sxs-lookup"><span data-stu-id="c70dc-145">String</span></span>| <span data-ttu-id="c70dc-146">依赖此 SRV 记录的 Microsoft Online Service 或功能。</span><span class="sxs-lookup"><span data-stu-id="c70dc-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="c70dc-147">可以是下列值之一：null、Email、Sharepoint、EmailInternalRelayOnly、OfficeCommunicationsOnline、SharePointDefaultDomain、FullRedelegation、SharePointPublic、OrgIdAuthentication、Yammer、Intune           </span><span class="sxs-lookup"><span data-stu-id="c70dc-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="c70dc-148">ttl</span><span class="sxs-lookup"><span data-stu-id="c70dc-148">ttl</span></span>|<span data-ttu-id="c70dc-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c70dc-149">Int32</span></span>| <span data-ttu-id="c70dc-150">在 DNS 主机上配置 SRV 记录 *(ttl*) 时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="c70dc-150">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="c70dc-151">不可为 null</span><span class="sxs-lookup"><span data-stu-id="c70dc-151">Not nullable</span></span> |
|<span data-ttu-id="c70dc-152">weight</span><span class="sxs-lookup"><span data-stu-id="c70dc-152">weight</span></span>|<span data-ttu-id="c70dc-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c70dc-153">Int32</span></span>| <span data-ttu-id="c70dc-154">在 DNS 主机上配置 SRV 记录的 *weight* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="c70dc-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c70dc-155">关系</span><span class="sxs-lookup"><span data-stu-id="c70dc-155">Relationships</span></span>
<span data-ttu-id="c70dc-156">无</span><span class="sxs-lookup"><span data-stu-id="c70dc-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c70dc-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c70dc-157">JSON representation</span></span>
<span data-ttu-id="c70dc-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c70dc-158">Here is a JSON representation of the resource.</span></span>

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


