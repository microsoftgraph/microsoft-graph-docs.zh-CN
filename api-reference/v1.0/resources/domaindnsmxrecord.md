---
title: domainDnsMxRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件的 MX 记录。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 017fe2ef132ce78a392a2f6fe83895b365002048
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761175"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="73de8-103">domainDnsMxRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="73de8-103">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="73de8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73de8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73de8-105">表示添加到租户中特定域的 DNS 区域文件的 MX 记录。</span><span class="sxs-lookup"><span data-stu-id="73de8-105">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="73de8-106">继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="73de8-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="73de8-107">方法</span><span class="sxs-lookup"><span data-stu-id="73de8-107">Methods</span></span>
<span data-ttu-id="73de8-108">不支持直接查询此资源。</span><span class="sxs-lookup"><span data-stu-id="73de8-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="73de8-109">请参阅 [域主题](domain.md) ，了解如何查询域服务记录。</span><span class="sxs-lookup"><span data-stu-id="73de8-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="73de8-110">属性</span><span class="sxs-lookup"><span data-stu-id="73de8-110">Properties</span></span>
| <span data-ttu-id="73de8-111">属性</span><span class="sxs-lookup"><span data-stu-id="73de8-111">Property</span></span>     | <span data-ttu-id="73de8-112">类型</span><span class="sxs-lookup"><span data-stu-id="73de8-112">Type</span></span>   |<span data-ttu-id="73de8-113">说明</span><span class="sxs-lookup"><span data-stu-id="73de8-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73de8-114">id</span><span class="sxs-lookup"><span data-stu-id="73de8-114">id</span></span>|<span data-ttu-id="73de8-115">字符串</span><span class="sxs-lookup"><span data-stu-id="73de8-115">String</span></span>| <span data-ttu-id="73de8-116">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="73de8-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="73de8-117">不可为空，只读。</span><span class="sxs-lookup"><span data-stu-id="73de8-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="73de8-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="73de8-118">isOptional</span></span>|<span data-ttu-id="73de8-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="73de8-119">Boolean</span></span>| <span data-ttu-id="73de8-120">如果为 false，则客户必须在 DNS 主机上配置 MX 记录，Microsoft Online Services该域正常运行。</span><span class="sxs-lookup"><span data-stu-id="73de8-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="73de8-121">label</span><span class="sxs-lookup"><span data-stu-id="73de8-121">label</span></span>|<span data-ttu-id="73de8-122">字符串</span><span class="sxs-lookup"><span data-stu-id="73de8-122">String</span></span>| <span data-ttu-id="73de8-123">在 DNS 主机上配置 MX 记录的 *别名/主机/* 名称属性时所使用的值。</span><span class="sxs-lookup"><span data-stu-id="73de8-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="73de8-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="73de8-124">mailExchange</span></span>|<span data-ttu-id="73de8-125">字符串</span><span class="sxs-lookup"><span data-stu-id="73de8-125">String</span></span>| <span data-ttu-id="73de8-126">在 DNS 主机上配置 MX 记录的应答 */目标/* 值时所使用的值。</span><span class="sxs-lookup"><span data-stu-id="73de8-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="73de8-127">preference</span><span class="sxs-lookup"><span data-stu-id="73de8-127">preference</span></span>|<span data-ttu-id="73de8-128">Int32</span><span class="sxs-lookup"><span data-stu-id="73de8-128">Int32</span></span>| <span data-ttu-id="73de8-129">在 DNS 主机上配置 MX 记录的 *Preference/Priority* 属性时所使用的值。</span><span class="sxs-lookup"><span data-stu-id="73de8-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="73de8-130">recordType</span><span class="sxs-lookup"><span data-stu-id="73de8-130">recordType</span></span>|<span data-ttu-id="73de8-131">字符串</span><span class="sxs-lookup"><span data-stu-id="73de8-131">String</span></span>| <span data-ttu-id="73de8-132">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="73de8-132">Type of DNS record.</span></span> <span data-ttu-id="73de8-133">该值始终为 *Mx*。</span><span class="sxs-lookup"><span data-stu-id="73de8-133">The value is always *Mx*.</span></span> <span data-ttu-id="73de8-134">键</span><span class="sxs-lookup"><span data-stu-id="73de8-134">Key</span></span> |
|<span data-ttu-id="73de8-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="73de8-135">supportedService</span></span>|<span data-ttu-id="73de8-136">字符串</span><span class="sxs-lookup"><span data-stu-id="73de8-136">String</span></span>| <span data-ttu-id="73de8-137">依赖此 MX 记录的 Microsoft Online Service 或功能。</span><span class="sxs-lookup"><span data-stu-id="73de8-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="73de8-138">可以是下列值之一：null、Email、Sharepoint、EmailInternalRelayOnly、OfficeCommunicationsOnline、SharePointDefaultDomain、FullRedelegation、SharePointPublic、OrgIdAuthentication、Yammer、Intune           </span><span class="sxs-lookup"><span data-stu-id="73de8-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="73de8-139">ttl</span><span class="sxs-lookup"><span data-stu-id="73de8-139">ttl</span></span>|<span data-ttu-id="73de8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="73de8-140">Int32</span></span>| <span data-ttu-id="73de8-141">在 DNS 主机上配置 MX 记录的 ttl (*ttl*) 时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="73de8-141">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="73de8-142">不可为 null</span><span class="sxs-lookup"><span data-stu-id="73de8-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="73de8-143">关系</span><span class="sxs-lookup"><span data-stu-id="73de8-143">Relationships</span></span>
<span data-ttu-id="73de8-144">无</span><span class="sxs-lookup"><span data-stu-id="73de8-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73de8-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73de8-145">JSON representation</span></span>
<span data-ttu-id="73de8-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73de8-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

