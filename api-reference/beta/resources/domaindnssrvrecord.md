---
title: domainDnsSrvRecord 资源类型
description: 表示已添加到租户中特定域的 DNS 区域文件的 SRV 记录。继承自 DomainDnsRecord 实体。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bdbc2246340d5cd15529dd05101567bc04d1e607
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524476"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="35d67-104">domainDnsSrvRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="35d67-104">domainDnsSrvRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35d67-p102">表示已添加到租户中特定域的 DNS 区域文件的 SRV 记录。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="35d67-p102">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="35d67-107">方法</span><span class="sxs-lookup"><span data-stu-id="35d67-107">Methods</span></span>
<span data-ttu-id="35d67-p103">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="35d67-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="35d67-110">属性</span><span class="sxs-lookup"><span data-stu-id="35d67-110">Properties</span></span>
| <span data-ttu-id="35d67-111">属性</span><span class="sxs-lookup"><span data-stu-id="35d67-111">Property</span></span>     | <span data-ttu-id="35d67-112">类型</span><span class="sxs-lookup"><span data-stu-id="35d67-112">Type</span></span>   |<span data-ttu-id="35d67-113">说明</span><span class="sxs-lookup"><span data-stu-id="35d67-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35d67-114">id</span><span class="sxs-lookup"><span data-stu-id="35d67-114">id</span></span>|<span data-ttu-id="35d67-115">字符串</span><span class="sxs-lookup"><span data-stu-id="35d67-115">String</span></span>| <span data-ttu-id="35d67-p104">分配给此实体的唯一标识符。不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="35d67-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="35d67-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="35d67-118">isOptional</span></span>|<span data-ttu-id="35d67-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="35d67-119">Boolean</span></span>| <span data-ttu-id="35d67-120">如果为 false，则客户必须在 DNS 主机上配置 SRV 记录才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="35d67-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="35d67-121">label</span><span class="sxs-lookup"><span data-stu-id="35d67-121">label</span></span>|<span data-ttu-id="35d67-122">字符串</span><span class="sxs-lookup"><span data-stu-id="35d67-122">String</span></span>| <span data-ttu-id="35d67-123">配置 DNS 主机上的 SRV 记录的*名称*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="35d67-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="35d67-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="35d67-124">nameTarget</span></span>|<span data-ttu-id="35d67-125">String</span><span class="sxs-lookup"><span data-stu-id="35d67-125">String</span></span>| <span data-ttu-id="35d67-126">配置 DNS 主机上的 SRV 记录的*目标*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="35d67-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="35d67-127">port</span><span class="sxs-lookup"><span data-stu-id="35d67-127">port</span></span>|<span data-ttu-id="35d67-128">Int32</span><span class="sxs-lookup"><span data-stu-id="35d67-128">Int32</span></span>| <span data-ttu-id="35d67-129">配置 DNS 主机上的 SRV 记录的*端口*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="35d67-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="35d67-130">priority</span><span class="sxs-lookup"><span data-stu-id="35d67-130">priority</span></span>|<span data-ttu-id="35d67-131">Int32</span><span class="sxs-lookup"><span data-stu-id="35d67-131">Int32</span></span>| <span data-ttu-id="35d67-132">配置 DNS 主机上的 SRV 记录的*优先级*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="35d67-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="35d67-133">protocol</span><span class="sxs-lookup"><span data-stu-id="35d67-133">protocol</span></span>|<span data-ttu-id="35d67-134">String</span><span class="sxs-lookup"><span data-stu-id="35d67-134">String</span></span>| <span data-ttu-id="35d67-135">配置 DNS 主机上的 SRV 记录的*协议*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="35d67-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="35d67-136">recordType</span><span class="sxs-lookup"><span data-stu-id="35d67-136">recordType</span></span>|<span data-ttu-id="35d67-137">String</span><span class="sxs-lookup"><span data-stu-id="35d67-137">String</span></span>|  <span data-ttu-id="35d67-p105">DNS 记录类型。此值始终是 *Srv*。Key</span><span class="sxs-lookup"><span data-stu-id="35d67-p105">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="35d67-141">service</span><span class="sxs-lookup"><span data-stu-id="35d67-141">service</span></span>|<span data-ttu-id="35d67-142">String</span><span class="sxs-lookup"><span data-stu-id="35d67-142">String</span></span>| <span data-ttu-id="35d67-143">配置 DNS 主机上的 SRV 记录的*服务*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="35d67-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="35d67-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="35d67-144">supportedService</span></span>|<span data-ttu-id="35d67-145">String</span><span class="sxs-lookup"><span data-stu-id="35d67-145">String</span></span>| <span data-ttu-id="35d67-146">Microsoft Online Service 或与该 SRV 记录存在依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="35d67-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="35d67-147">可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="35d67-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="35d67-148">ttl</span><span class="sxs-lookup"><span data-stu-id="35d67-148">ttl</span></span>|<span data-ttu-id="35d67-149">Int32</span><span class="sxs-lookup"><span data-stu-id="35d67-149">Int32</span></span>| <span data-ttu-id="35d67-p106">配置 DNS 主机上的 SRV 记录的*生存时间 (ttl)* 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="35d67-p106">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="35d67-152">weight</span><span class="sxs-lookup"><span data-stu-id="35d67-152">weight</span></span>|<span data-ttu-id="35d67-153">Int32</span><span class="sxs-lookup"><span data-stu-id="35d67-153">Int32</span></span>| <span data-ttu-id="35d67-154">配置 DNS 主机上的 SRV 记录的*权重*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="35d67-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="35d67-155">关系</span><span class="sxs-lookup"><span data-stu-id="35d67-155">Relationships</span></span>
<span data-ttu-id="35d67-156">无</span><span class="sxs-lookup"><span data-stu-id="35d67-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="35d67-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35d67-157">JSON representation</span></span>
<span data-ttu-id="35d67-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35d67-158">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnssrvrecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
