---
title: domainDnsMxRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件中的 MX 记录。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 72e260fc4ba3401d94aec2e32096b167f8297234
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010344"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="f41ec-103">domainDnsMxRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="f41ec-103">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="f41ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f41ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f41ec-105">表示添加到租户中特定域的 DNS 区域文件中的 MX 记录。</span><span class="sxs-lookup"><span data-stu-id="f41ec-105">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="f41ec-106">继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="f41ec-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="f41ec-107">方法</span><span class="sxs-lookup"><span data-stu-id="f41ec-107">Methods</span></span>
<span data-ttu-id="f41ec-108">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="f41ec-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="f41ec-109">有关如何查询域服务记录的信息，请参阅 [域](domain.md) 主题。</span><span class="sxs-lookup"><span data-stu-id="f41ec-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="f41ec-110">属性</span><span class="sxs-lookup"><span data-stu-id="f41ec-110">Properties</span></span>
| <span data-ttu-id="f41ec-111">属性</span><span class="sxs-lookup"><span data-stu-id="f41ec-111">Property</span></span>     | <span data-ttu-id="f41ec-112">类型</span><span class="sxs-lookup"><span data-stu-id="f41ec-112">Type</span></span>   |<span data-ttu-id="f41ec-113">说明</span><span class="sxs-lookup"><span data-stu-id="f41ec-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f41ec-114">id</span><span class="sxs-lookup"><span data-stu-id="f41ec-114">id</span></span>|<span data-ttu-id="f41ec-115">String</span><span class="sxs-lookup"><span data-stu-id="f41ec-115">String</span></span>| <span data-ttu-id="f41ec-116">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f41ec-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="f41ec-117">不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="f41ec-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="f41ec-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="f41ec-118">isOptional</span></span>|<span data-ttu-id="f41ec-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="f41ec-119">Boolean</span></span>| <span data-ttu-id="f41ec-120">如果为 false，则客户必须在 DNS 主机上配置 MX 记录，才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="f41ec-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="f41ec-121">label</span><span class="sxs-lookup"><span data-stu-id="f41ec-121">label</span></span>|<span data-ttu-id="f41ec-122">String</span><span class="sxs-lookup"><span data-stu-id="f41ec-122">String</span></span>| <span data-ttu-id="f41ec-123">配置 DNS 主机上的 MX 记录的 *别名/主机/名称* 属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="f41ec-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="f41ec-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="f41ec-124">mailExchange</span></span>|<span data-ttu-id="f41ec-125">String</span><span class="sxs-lookup"><span data-stu-id="f41ec-125">String</span></span>| <span data-ttu-id="f41ec-126">配置 DNS 主机上的 MX 记录的 *应答/目标/值* 时使用的值。</span><span class="sxs-lookup"><span data-stu-id="f41ec-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="f41ec-127">优先权</span><span class="sxs-lookup"><span data-stu-id="f41ec-127">preference</span></span>|<span data-ttu-id="f41ec-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f41ec-128">Int32</span></span>| <span data-ttu-id="f41ec-129">配置 DNS 主机上的 MX 记录的 *首选项/优先级* 属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="f41ec-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="f41ec-130">recordType</span><span class="sxs-lookup"><span data-stu-id="f41ec-130">recordType</span></span>|<span data-ttu-id="f41ec-131">String</span><span class="sxs-lookup"><span data-stu-id="f41ec-131">String</span></span>| <span data-ttu-id="f41ec-132">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="f41ec-132">Type of DNS record.</span></span> <span data-ttu-id="f41ec-133">值始终为 *Mx*。</span><span class="sxs-lookup"><span data-stu-id="f41ec-133">The value is always *Mx*.</span></span> <span data-ttu-id="f41ec-134">键</span><span class="sxs-lookup"><span data-stu-id="f41ec-134">Key</span></span> |
|<span data-ttu-id="f41ec-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="f41ec-135">supportedService</span></span>|<span data-ttu-id="f41ec-136">String</span><span class="sxs-lookup"><span data-stu-id="f41ec-136">String</span></span>| <span data-ttu-id="f41ec-137">与此 MX 记录相关的 Microsoft Online 服务或功能。</span><span class="sxs-lookup"><span data-stu-id="f41ec-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="f41ec-138">可以是下列值之一： **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="f41ec-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="f41ec-139">ttl</span><span class="sxs-lookup"><span data-stu-id="f41ec-139">ttl</span></span>|<span data-ttu-id="f41ec-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f41ec-140">Int32</span></span>| <span data-ttu-id="f41ec-141">在 DNS 主机上配置 MX 记录的 \*生存时间 (ttl) \* 属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="f41ec-141">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="f41ec-142">不可为 null</span><span class="sxs-lookup"><span data-stu-id="f41ec-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="f41ec-143">关系</span><span class="sxs-lookup"><span data-stu-id="f41ec-143">Relationships</span></span>
<span data-ttu-id="f41ec-144">无</span><span class="sxs-lookup"><span data-stu-id="f41ec-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f41ec-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f41ec-145">JSON representation</span></span>
<span data-ttu-id="f41ec-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f41ec-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


