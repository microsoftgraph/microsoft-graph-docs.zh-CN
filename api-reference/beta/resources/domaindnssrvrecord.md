---
title: domainDnsSrvRecord 资源类型
description: 表示已添加到租户中特定域的 DNS 区域文件的 SRV 记录。继承自 DomainDnsRecord 实体。
author: lleonard-msft
ms.openlocfilehash: 73eec36406844ef26b0f0349711258ddcd13f200
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322048"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="da736-104">domainDnsSrvRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="da736-104">domainDnsSrvRecord resource type</span></span>

> <span data-ttu-id="da736-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="da736-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da736-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="da736-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da736-p103">表示已添加到租户中特定域的 DNS 区域文件的 SRV 记录。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="da736-p103">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="da736-109">方法</span><span class="sxs-lookup"><span data-stu-id="da736-109">Methods</span></span>
<span data-ttu-id="da736-p104">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="da736-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="da736-112">属性</span><span class="sxs-lookup"><span data-stu-id="da736-112">Properties</span></span>
| <span data-ttu-id="da736-113">属性</span><span class="sxs-lookup"><span data-stu-id="da736-113">Property</span></span>     | <span data-ttu-id="da736-114">类型</span><span class="sxs-lookup"><span data-stu-id="da736-114">Type</span></span>   |<span data-ttu-id="da736-115">说明</span><span class="sxs-lookup"><span data-stu-id="da736-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da736-116">id</span><span class="sxs-lookup"><span data-stu-id="da736-116">id</span></span>|<span data-ttu-id="da736-117">字符串</span><span class="sxs-lookup"><span data-stu-id="da736-117">String</span></span>| <span data-ttu-id="da736-p105">分配给此实体的唯一标识符。不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="da736-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="da736-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="da736-120">isOptional</span></span>|<span data-ttu-id="da736-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="da736-121">Boolean</span></span>| <span data-ttu-id="da736-122">如果为 false，则客户必须在 DNS 主机上配置 SRV 记录才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="da736-122">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="da736-123">label</span><span class="sxs-lookup"><span data-stu-id="da736-123">label</span></span>|<span data-ttu-id="da736-124">String</span><span class="sxs-lookup"><span data-stu-id="da736-124">String</span></span>| <span data-ttu-id="da736-125">配置 DNS 主机上的 SRV 记录的*名称*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="da736-125">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="da736-126">nameTarget</span><span class="sxs-lookup"><span data-stu-id="da736-126">nameTarget</span></span>|<span data-ttu-id="da736-127">String</span><span class="sxs-lookup"><span data-stu-id="da736-127">String</span></span>| <span data-ttu-id="da736-128">配置 DNS 主机上的 SRV 记录的*目标*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="da736-128">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="da736-129">port</span><span class="sxs-lookup"><span data-stu-id="da736-129">port</span></span>|<span data-ttu-id="da736-130">Int32</span><span class="sxs-lookup"><span data-stu-id="da736-130">Int32</span></span>| <span data-ttu-id="da736-131">配置 DNS 主机上的 SRV 记录的*端口*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="da736-131">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="da736-132">priority</span><span class="sxs-lookup"><span data-stu-id="da736-132">priority</span></span>|<span data-ttu-id="da736-133">Int32</span><span class="sxs-lookup"><span data-stu-id="da736-133">Int32</span></span>| <span data-ttu-id="da736-134">配置 DNS 主机上的 SRV 记录的*优先级*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="da736-134">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="da736-135">protocol</span><span class="sxs-lookup"><span data-stu-id="da736-135">protocol</span></span>|<span data-ttu-id="da736-136">String</span><span class="sxs-lookup"><span data-stu-id="da736-136">String</span></span>| <span data-ttu-id="da736-137">配置 DNS 主机上的 SRV 记录的*协议*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="da736-137">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="da736-138">recordType</span><span class="sxs-lookup"><span data-stu-id="da736-138">recordType</span></span>|<span data-ttu-id="da736-139">String</span><span class="sxs-lookup"><span data-stu-id="da736-139">String</span></span>|  <span data-ttu-id="da736-p106">DNS 记录类型。此值始终是 *Srv*。Key</span><span class="sxs-lookup"><span data-stu-id="da736-p106">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="da736-143">service</span><span class="sxs-lookup"><span data-stu-id="da736-143">service</span></span>|<span data-ttu-id="da736-144">String</span><span class="sxs-lookup"><span data-stu-id="da736-144">String</span></span>| <span data-ttu-id="da736-145">配置 DNS 主机上的 SRV 记录的*服务*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="da736-145">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="da736-146">supportedService</span><span class="sxs-lookup"><span data-stu-id="da736-146">supportedService</span></span>|<span data-ttu-id="da736-147">String</span><span class="sxs-lookup"><span data-stu-id="da736-147">String</span></span>| <span data-ttu-id="da736-148">Microsoft Online Service 或与该 SRV 记录存在依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="da736-148">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="da736-149">可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="da736-149">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="da736-150">ttl</span><span class="sxs-lookup"><span data-stu-id="da736-150">ttl</span></span>|<span data-ttu-id="da736-151">Int32</span><span class="sxs-lookup"><span data-stu-id="da736-151">Int32</span></span>| <span data-ttu-id="da736-p107">配置 DNS 主机上的 SRV 记录的*生存时间 (ttl)* 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="da736-p107">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="da736-154">weight</span><span class="sxs-lookup"><span data-stu-id="da736-154">weight</span></span>|<span data-ttu-id="da736-155">Int32</span><span class="sxs-lookup"><span data-stu-id="da736-155">Int32</span></span>| <span data-ttu-id="da736-156">配置 DNS 主机上的 SRV 记录的*权重*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="da736-156">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="da736-157">关系</span><span class="sxs-lookup"><span data-stu-id="da736-157">Relationships</span></span>
<span data-ttu-id="da736-158">无</span><span class="sxs-lookup"><span data-stu-id="da736-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="da736-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da736-159">JSON representation</span></span>
<span data-ttu-id="da736-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da736-160">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->