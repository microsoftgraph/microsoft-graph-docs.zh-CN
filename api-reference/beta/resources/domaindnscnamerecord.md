---
title: domainDnsCnameRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件的 CNAME 记录。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ecbe5c0dd1d547a6abb116c5152a8d21f0ee3fd8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760881"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="8a18b-103">domainDnsCnameRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a18b-103">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="8a18b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a18b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a18b-105">表示添加到租户中特定域的 DNS 区域文件的 CNAME 记录。</span><span class="sxs-lookup"><span data-stu-id="8a18b-105">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="8a18b-106">继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="8a18b-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="8a18b-107">方法</span><span class="sxs-lookup"><span data-stu-id="8a18b-107">Methods</span></span>
<span data-ttu-id="8a18b-108">不支持直接查询此资源。</span><span class="sxs-lookup"><span data-stu-id="8a18b-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="8a18b-109">请参阅 [域主题](domain.md) ，了解如何查询域服务记录。</span><span class="sxs-lookup"><span data-stu-id="8a18b-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="8a18b-110">属性</span><span class="sxs-lookup"><span data-stu-id="8a18b-110">Properties</span></span>
| <span data-ttu-id="8a18b-111">属性</span><span class="sxs-lookup"><span data-stu-id="8a18b-111">Property</span></span>     | <span data-ttu-id="8a18b-112">类型</span><span class="sxs-lookup"><span data-stu-id="8a18b-112">Type</span></span>   |<span data-ttu-id="8a18b-113">说明</span><span class="sxs-lookup"><span data-stu-id="8a18b-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a18b-114">canonicalName</span><span class="sxs-lookup"><span data-stu-id="8a18b-114">canonicalName</span></span>|<span data-ttu-id="8a18b-115">String</span><span class="sxs-lookup"><span data-stu-id="8a18b-115">String</span></span>| <span data-ttu-id="8a18b-116">CNAME 记录的规范名称。</span><span class="sxs-lookup"><span data-stu-id="8a18b-116">The canonical name of the CNAME record.</span></span> <span data-ttu-id="8a18b-117">用于在 DNS 主机上配置 CNAME 记录。</span><span class="sxs-lookup"><span data-stu-id="8a18b-117">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="8a18b-118">id</span><span class="sxs-lookup"><span data-stu-id="8a18b-118">id</span></span>|<span data-ttu-id="8a18b-119">String</span><span class="sxs-lookup"><span data-stu-id="8a18b-119">String</span></span>| <span data-ttu-id="8a18b-120">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8a18b-120">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="8a18b-121">不可为空，只读</span><span class="sxs-lookup"><span data-stu-id="8a18b-121">Not nullable, Read-only</span></span>|
|<span data-ttu-id="8a18b-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="8a18b-122">isOptional</span></span>|<span data-ttu-id="8a18b-123">布尔</span><span class="sxs-lookup"><span data-stu-id="8a18b-123">Boolean</span></span>| <span data-ttu-id="8a18b-124">如果为 false，则客户必须在 DNS 主机上配置 CNAME 记录，Microsoft Online Services该域正常运行。</span><span class="sxs-lookup"><span data-stu-id="8a18b-124">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="8a18b-125">不可为 null</span><span class="sxs-lookup"><span data-stu-id="8a18b-125">Not nullable</span></span> |
|<span data-ttu-id="8a18b-126">label</span><span class="sxs-lookup"><span data-stu-id="8a18b-126">label</span></span>|<span data-ttu-id="8a18b-127">String</span><span class="sxs-lookup"><span data-stu-id="8a18b-127">String</span></span>| <span data-ttu-id="8a18b-128">在 DNS 主机上配置 CNAME 记录的 *别名/主机/* 名称时所使用的值。</span><span class="sxs-lookup"><span data-stu-id="8a18b-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="8a18b-129">recordType</span><span class="sxs-lookup"><span data-stu-id="8a18b-129">recordType</span></span>|<span data-ttu-id="8a18b-130">String</span><span class="sxs-lookup"><span data-stu-id="8a18b-130">String</span></span>| <span data-ttu-id="8a18b-131">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="8a18b-131">Type of DNS record.</span></span> <span data-ttu-id="8a18b-132">该值始终为 *CName*。</span><span class="sxs-lookup"><span data-stu-id="8a18b-132">The value is always *CName*.</span></span> <span data-ttu-id="8a18b-133">键</span><span class="sxs-lookup"><span data-stu-id="8a18b-133">Key</span></span>|
|<span data-ttu-id="8a18b-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="8a18b-134">supportedService</span></span>|<span data-ttu-id="8a18b-135">String</span><span class="sxs-lookup"><span data-stu-id="8a18b-135">String</span></span>| <span data-ttu-id="8a18b-136">依赖此 CNAME 记录的 Microsoft Online 服务或功能。</span><span class="sxs-lookup"><span data-stu-id="8a18b-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="8a18b-137">可以是下列值之一：null、Email、Sharepoint、EmailInternalRelayOnly、OfficeCommunicationsOnline、SharePointDefaultDomain、FullRedelegation、SharePointPublic、OrgIdAuthentication、Yammer、Intune           </span><span class="sxs-lookup"><span data-stu-id="8a18b-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="8a18b-138">ttl</span><span class="sxs-lookup"><span data-stu-id="8a18b-138">ttl</span></span>|<span data-ttu-id="8a18b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8a18b-139">Int32</span></span>| <span data-ttu-id="8a18b-140">在 DNS 主机上配置 CNAME 记录的 ttl (ttl) 时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8a18b-140">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="8a18b-141">不可为 null</span><span class="sxs-lookup"><span data-stu-id="8a18b-141">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="8a18b-142">关系</span><span class="sxs-lookup"><span data-stu-id="8a18b-142">Relationships</span></span>
<span data-ttu-id="8a18b-143">无</span><span class="sxs-lookup"><span data-stu-id="8a18b-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8a18b-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a18b-144">JSON representation</span></span>
<span data-ttu-id="8a18b-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a18b-145">Here is a JSON representation of the resource.</span></span>

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


