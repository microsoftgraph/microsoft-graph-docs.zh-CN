---
title: domainDnsMxRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件中的 MX 记录。 继承自 DomainDnsRecord 实体。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b61638c2013257eebbe77f4c36a274619d6daf2b
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657110"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="29946-104">domainDnsMxRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="29946-104">domainDnsMxRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29946-105">表示添加到租户中特定域的 DNS 区域文件中的 MX 记录。</span><span class="sxs-lookup"><span data-stu-id="29946-105">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="29946-106">继承自[DomainDnsRecord](domaindnsrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="29946-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="29946-107">方法</span><span class="sxs-lookup"><span data-stu-id="29946-107">Methods</span></span>
<span data-ttu-id="29946-108">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="29946-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="29946-109">有关如何查询域服务记录的信息, 请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="29946-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="29946-110">属性</span><span class="sxs-lookup"><span data-stu-id="29946-110">Properties</span></span>
| <span data-ttu-id="29946-111">属性</span><span class="sxs-lookup"><span data-stu-id="29946-111">Property</span></span>     | <span data-ttu-id="29946-112">类型</span><span class="sxs-lookup"><span data-stu-id="29946-112">Type</span></span>   |<span data-ttu-id="29946-113">说明</span><span class="sxs-lookup"><span data-stu-id="29946-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29946-114">id</span><span class="sxs-lookup"><span data-stu-id="29946-114">id</span></span>|<span data-ttu-id="29946-115">String</span><span class="sxs-lookup"><span data-stu-id="29946-115">String</span></span>| <span data-ttu-id="29946-116">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="29946-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="29946-117">不可为 null, 只读。</span><span class="sxs-lookup"><span data-stu-id="29946-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="29946-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="29946-118">isOptional</span></span>|<span data-ttu-id="29946-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="29946-119">Boolean</span></span>| <span data-ttu-id="29946-120">如果为 false, 则客户必须在 DNS 主机上配置 MX 记录, 才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="29946-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="29946-121">label</span><span class="sxs-lookup"><span data-stu-id="29946-121">label</span></span>|<span data-ttu-id="29946-122">String</span><span class="sxs-lookup"><span data-stu-id="29946-122">String</span></span>| <span data-ttu-id="29946-123">配置 DNS 主机上的 MX 记录的*别名/主机/名称*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="29946-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="29946-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="29946-124">mailExchange</span></span>|<span data-ttu-id="29946-125">String</span><span class="sxs-lookup"><span data-stu-id="29946-125">String</span></span>| <span data-ttu-id="29946-126">配置 DNS 主机上的 MX 记录的*应答/目标/值*时使用的值。</span><span class="sxs-lookup"><span data-stu-id="29946-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="29946-127">优先权</span><span class="sxs-lookup"><span data-stu-id="29946-127">preference</span></span>|<span data-ttu-id="29946-128">Int32</span><span class="sxs-lookup"><span data-stu-id="29946-128">Int32</span></span>| <span data-ttu-id="29946-129">配置 DNS 主机上的 MX 记录的*首选项/优先级*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="29946-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="29946-130">recordType</span><span class="sxs-lookup"><span data-stu-id="29946-130">recordType</span></span>|<span data-ttu-id="29946-131">String</span><span class="sxs-lookup"><span data-stu-id="29946-131">String</span></span>| <span data-ttu-id="29946-132">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="29946-132">Type of DNS record.</span></span> <span data-ttu-id="29946-133">值始终为*Mx*。</span><span class="sxs-lookup"><span data-stu-id="29946-133">The value is always *Mx*.</span></span> <span data-ttu-id="29946-134">Key</span><span class="sxs-lookup"><span data-stu-id="29946-134">Key</span></span> |
|<span data-ttu-id="29946-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="29946-135">supportedService</span></span>|<span data-ttu-id="29946-136">String</span><span class="sxs-lookup"><span data-stu-id="29946-136">String</span></span>| <span data-ttu-id="29946-137">与此 MX 记录相关的 Microsoft Online 服务或功能。</span><span class="sxs-lookup"><span data-stu-id="29946-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="29946-138">可以是下列值之一: **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="29946-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="29946-139">ttl</span><span class="sxs-lookup"><span data-stu-id="29946-139">ttl</span></span>|<span data-ttu-id="29946-140">Int32</span><span class="sxs-lookup"><span data-stu-id="29946-140">Int32</span></span>| <span data-ttu-id="29946-141">配置 DNS 主机上的 MX 记录的*生存时间 (ttl)* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="29946-141">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="29946-142">不可为 null</span><span class="sxs-lookup"><span data-stu-id="29946-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="29946-143">关系</span><span class="sxs-lookup"><span data-stu-id="29946-143">Relationships</span></span>
<span data-ttu-id="29946-144">无</span><span class="sxs-lookup"><span data-stu-id="29946-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29946-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29946-145">JSON representation</span></span>
<span data-ttu-id="29946-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29946-146">Here is a JSON representation of the resource.</span></span>

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
