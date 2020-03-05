---
title: domainDnsMxRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件中的 MX 记录。 继承自 DomainDnsRecord 实体。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1af4ca26a3456dd3e926b81045845675002c04a1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506356"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="33200-104">domainDnsMxRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="33200-104">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="33200-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="33200-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33200-106">表示添加到租户中特定域的 DNS 区域文件中的 MX 记录。</span><span class="sxs-lookup"><span data-stu-id="33200-106">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="33200-107">继承自[DomainDnsRecord](domaindnsrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="33200-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="33200-108">方法</span><span class="sxs-lookup"><span data-stu-id="33200-108">Methods</span></span>
<span data-ttu-id="33200-109">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="33200-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="33200-110">有关如何查询域服务记录的信息，请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="33200-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="33200-111">属性</span><span class="sxs-lookup"><span data-stu-id="33200-111">Properties</span></span>
| <span data-ttu-id="33200-112">属性</span><span class="sxs-lookup"><span data-stu-id="33200-112">Property</span></span>     | <span data-ttu-id="33200-113">类型</span><span class="sxs-lookup"><span data-stu-id="33200-113">Type</span></span>   |<span data-ttu-id="33200-114">说明</span><span class="sxs-lookup"><span data-stu-id="33200-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33200-115">id</span><span class="sxs-lookup"><span data-stu-id="33200-115">id</span></span>|<span data-ttu-id="33200-116">String</span><span class="sxs-lookup"><span data-stu-id="33200-116">String</span></span>| <span data-ttu-id="33200-117">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="33200-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="33200-118">不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="33200-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="33200-119">isOptional</span><span class="sxs-lookup"><span data-stu-id="33200-119">isOptional</span></span>|<span data-ttu-id="33200-120">布尔</span><span class="sxs-lookup"><span data-stu-id="33200-120">Boolean</span></span>| <span data-ttu-id="33200-121">如果为 false，则客户必须在 DNS 主机上配置 MX 记录，才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="33200-121">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="33200-122">label</span><span class="sxs-lookup"><span data-stu-id="33200-122">label</span></span>|<span data-ttu-id="33200-123">String</span><span class="sxs-lookup"><span data-stu-id="33200-123">String</span></span>| <span data-ttu-id="33200-124">配置 DNS 主机上的 MX 记录的*别名/主机/名称*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="33200-124">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="33200-125">mailExchange</span><span class="sxs-lookup"><span data-stu-id="33200-125">mailExchange</span></span>|<span data-ttu-id="33200-126">String</span><span class="sxs-lookup"><span data-stu-id="33200-126">String</span></span>| <span data-ttu-id="33200-127">配置 DNS 主机上的 MX 记录的*应答/目标/值*时使用的值。</span><span class="sxs-lookup"><span data-stu-id="33200-127">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="33200-128">优先权</span><span class="sxs-lookup"><span data-stu-id="33200-128">preference</span></span>|<span data-ttu-id="33200-129">Int32</span><span class="sxs-lookup"><span data-stu-id="33200-129">Int32</span></span>| <span data-ttu-id="33200-130">配置 DNS 主机上的 MX 记录的*首选项/优先级*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="33200-130">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="33200-131">recordType</span><span class="sxs-lookup"><span data-stu-id="33200-131">recordType</span></span>|<span data-ttu-id="33200-132">String</span><span class="sxs-lookup"><span data-stu-id="33200-132">String</span></span>| <span data-ttu-id="33200-133">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="33200-133">Type of DNS record.</span></span> <span data-ttu-id="33200-134">值始终为*Mx*。</span><span class="sxs-lookup"><span data-stu-id="33200-134">The value is always *Mx*.</span></span> <span data-ttu-id="33200-135">键</span><span class="sxs-lookup"><span data-stu-id="33200-135">Key</span></span> |
|<span data-ttu-id="33200-136">supportedService</span><span class="sxs-lookup"><span data-stu-id="33200-136">supportedService</span></span>|<span data-ttu-id="33200-137">String</span><span class="sxs-lookup"><span data-stu-id="33200-137">String</span></span>| <span data-ttu-id="33200-138">与此 MX 记录相关的 Microsoft Online 服务或功能。</span><span class="sxs-lookup"><span data-stu-id="33200-138">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="33200-139">可以是下列值之一： **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="33200-139">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="33200-140">ttl</span><span class="sxs-lookup"><span data-stu-id="33200-140">ttl</span></span>|<span data-ttu-id="33200-141">Int32</span><span class="sxs-lookup"><span data-stu-id="33200-141">Int32</span></span>| <span data-ttu-id="33200-142">配置 DNS 主机上的 MX 记录的*生存时间（ttl）* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="33200-142">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="33200-143">不可为 null</span><span class="sxs-lookup"><span data-stu-id="33200-143">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="33200-144">关系</span><span class="sxs-lookup"><span data-stu-id="33200-144">Relationships</span></span>
<span data-ttu-id="33200-145">无</span><span class="sxs-lookup"><span data-stu-id="33200-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33200-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33200-146">JSON representation</span></span>
<span data-ttu-id="33200-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33200-147">Here is a JSON representation of the resource.</span></span>

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
