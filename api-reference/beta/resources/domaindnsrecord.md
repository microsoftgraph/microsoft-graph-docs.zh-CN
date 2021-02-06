---
title: domainDnsRecord 资源类型
description: DomainDnsRecord 实体用于显示 DNS 记录。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e3a5152d5eb59a4a1547ee8c7fcc6dbf88c1d976
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137604"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="35c32-103">domainDnsRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="35c32-103">domainDnsRecord resource type</span></span>

<span data-ttu-id="35c32-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35c32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35c32-105">对于租户中的每个域，可能需要先将 dns 记录 () 域的 DNS 区域文件，然后域才能供 Microsoft Online Services。</span><span class="sxs-lookup"><span data-stu-id="35c32-105">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="35c32-106">**DomainDnsRecord** 实体用于显示此类 DNS 记录。</span><span class="sxs-lookup"><span data-stu-id="35c32-106">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="35c32-107">DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord 和[DomainDnsTxtRecord](domaindnstxtrecord.md)实体的基本实体。 [](domaindnscnamerecord.md) [](domaindnsmxrecord.md) [](domaindnssrvrecord.md)</span><span class="sxs-lookup"><span data-stu-id="35c32-107">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="35c32-108">方法</span><span class="sxs-lookup"><span data-stu-id="35c32-108">Methods</span></span>
<span data-ttu-id="35c32-109">不支持直接查询此资源。</span><span class="sxs-lookup"><span data-stu-id="35c32-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="35c32-110">请参阅 [域主题](domain.md) ，了解如何查询域服务记录。</span><span class="sxs-lookup"><span data-stu-id="35c32-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="35c32-111">属性</span><span class="sxs-lookup"><span data-stu-id="35c32-111">Properties</span></span>
| <span data-ttu-id="35c32-112">属性</span><span class="sxs-lookup"><span data-stu-id="35c32-112">Property</span></span>     | <span data-ttu-id="35c32-113">类型</span><span class="sxs-lookup"><span data-stu-id="35c32-113">Type</span></span>   |<span data-ttu-id="35c32-114">说明</span><span class="sxs-lookup"><span data-stu-id="35c32-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35c32-115">id</span><span class="sxs-lookup"><span data-stu-id="35c32-115">id</span></span>|<span data-ttu-id="35c32-116">字符串</span><span class="sxs-lookup"><span data-stu-id="35c32-116">String</span></span>| <span data-ttu-id="35c32-117">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="35c32-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="35c32-118">不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="35c32-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="35c32-119">isOptional</span><span class="sxs-lookup"><span data-stu-id="35c32-119">isOptional</span></span>|<span data-ttu-id="35c32-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="35c32-120">Boolean</span></span>| <span data-ttu-id="35c32-121">如果为 false，则必须由 DNS 主机的客户配置此记录，Microsoft Online Services域正常运行。</span><span class="sxs-lookup"><span data-stu-id="35c32-121">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="35c32-122">label</span><span class="sxs-lookup"><span data-stu-id="35c32-122">label</span></span>|<span data-ttu-id="35c32-123">字符串</span><span class="sxs-lookup"><span data-stu-id="35c32-123">String</span></span>| <span data-ttu-id="35c32-124">在 DNS 主机上配置 DNS 记录的名称时所使用的值。</span><span class="sxs-lookup"><span data-stu-id="35c32-124">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="35c32-125">recordType</span><span class="sxs-lookup"><span data-stu-id="35c32-125">recordType</span></span>|<span data-ttu-id="35c32-126">字符串</span><span class="sxs-lookup"><span data-stu-id="35c32-126">String</span></span>| <span data-ttu-id="35c32-127">指示此实体表示的 DNS 记录类型。</span><span class="sxs-lookup"><span data-stu-id="35c32-127">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="35c32-128">值可以是以下项之一：CName、Mx、Srv、Txt    </span><span class="sxs-lookup"><span data-stu-id="35c32-128">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="35c32-129">键</span><span class="sxs-lookup"><span data-stu-id="35c32-129">Key</span></span> |
|<span data-ttu-id="35c32-130">supportedService</span><span class="sxs-lookup"><span data-stu-id="35c32-130">supportedService</span></span>|<span data-ttu-id="35c32-131">字符串</span><span class="sxs-lookup"><span data-stu-id="35c32-131">String</span></span>| <span data-ttu-id="35c32-132">依赖此 DNS 记录的 Microsoft Online Service 或功能。</span><span class="sxs-lookup"><span data-stu-id="35c32-132">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="35c32-133">可以是下列值之一：null、Email、Sharepoint、EmailInternalRelayOnly、OfficeCommunicationsOnline、SharePointDefaultDomain、FullRedelegation、SharePointPublic、OrgIdAuthentication、Yammer、Intune           </span><span class="sxs-lookup"><span data-stu-id="35c32-133">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="35c32-134">ttl</span><span class="sxs-lookup"><span data-stu-id="35c32-134">ttl</span></span>|<span data-ttu-id="35c32-135">Int32</span><span class="sxs-lookup"><span data-stu-id="35c32-135">Int32</span></span>| <span data-ttu-id="35c32-136">在 DNS 主机上配置 DNS 记录的 (ttl) 属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="35c32-136">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="35c32-137">不可为 null</span><span class="sxs-lookup"><span data-stu-id="35c32-137">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="35c32-138">关系</span><span class="sxs-lookup"><span data-stu-id="35c32-138">Relationships</span></span>
<span data-ttu-id="35c32-139">无</span><span class="sxs-lookup"><span data-stu-id="35c32-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35c32-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35c32-140">JSON representation</span></span>
<span data-ttu-id="35c32-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35c32-141">Here is a JSON representation of the resource.</span></span>

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


