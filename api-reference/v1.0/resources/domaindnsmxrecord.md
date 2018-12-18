---
title: domainDnsMxRecord 资源类型
description: 表示已添加到租户中特定域的 DNS 区域文件的 MX 记录。继承自 DomainDnsRecord 实体。
author: lleonard-msft
ms.openlocfilehash: e06b3c405f4ad5e2e561e57876ef010bddb1068d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345834"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="878dd-104">domainDnsMxRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="878dd-104">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="878dd-p102">表示已添加到租户中特定域的 DNS 区域文件的 MX 记录。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="878dd-p102">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="878dd-107">方法</span><span class="sxs-lookup"><span data-stu-id="878dd-107">Methods</span></span>
<span data-ttu-id="878dd-p103">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="878dd-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="878dd-110">属性</span><span class="sxs-lookup"><span data-stu-id="878dd-110">Properties</span></span>
| <span data-ttu-id="878dd-111">属性</span><span class="sxs-lookup"><span data-stu-id="878dd-111">Property</span></span>     | <span data-ttu-id="878dd-112">类型</span><span class="sxs-lookup"><span data-stu-id="878dd-112">Type</span></span>   |<span data-ttu-id="878dd-113">说明</span><span class="sxs-lookup"><span data-stu-id="878dd-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="878dd-114">id</span><span class="sxs-lookup"><span data-stu-id="878dd-114">id</span></span>|<span data-ttu-id="878dd-115">字符串</span><span class="sxs-lookup"><span data-stu-id="878dd-115">String</span></span>| <span data-ttu-id="878dd-p104">分配给此实体的唯一标识符。不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="878dd-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="878dd-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="878dd-118">isOptional</span></span>|<span data-ttu-id="878dd-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="878dd-119">Boolean</span></span>| <span data-ttu-id="878dd-120">如果为 false，则客户必须在 DNS 主机上配置 MX 记录才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="878dd-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="878dd-121">label</span><span class="sxs-lookup"><span data-stu-id="878dd-121">label</span></span>|<span data-ttu-id="878dd-122">String</span><span class="sxs-lookup"><span data-stu-id="878dd-122">String</span></span>| <span data-ttu-id="878dd-123">配置 DNS 主机上的 MX 记录的*别名/主机/名称*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="878dd-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="878dd-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="878dd-124">mailExchange</span></span>|<span data-ttu-id="878dd-125">String</span><span class="sxs-lookup"><span data-stu-id="878dd-125">String</span></span>| <span data-ttu-id="878dd-126">配置 DNS 主机上的 MX 记录的*答复/目标/值*时使用的值。</span><span class="sxs-lookup"><span data-stu-id="878dd-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="878dd-127">preference</span><span class="sxs-lookup"><span data-stu-id="878dd-127">preference</span></span>|<span data-ttu-id="878dd-128">Int32</span><span class="sxs-lookup"><span data-stu-id="878dd-128">Int32</span></span>| <span data-ttu-id="878dd-129">配置 DNS 主机上的 MX 记录的*首选项/优先级*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="878dd-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="878dd-130">recordType</span><span class="sxs-lookup"><span data-stu-id="878dd-130">recordType</span></span>|<span data-ttu-id="878dd-131">String</span><span class="sxs-lookup"><span data-stu-id="878dd-131">String</span></span>| <span data-ttu-id="878dd-p105">DNS 记录类型。此值始终是 *Mx*。Key</span><span class="sxs-lookup"><span data-stu-id="878dd-p105">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="878dd-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="878dd-135">supportedService</span></span>|<span data-ttu-id="878dd-136">String</span><span class="sxs-lookup"><span data-stu-id="878dd-136">String</span></span>| <span data-ttu-id="878dd-137">Microsoft Online Service 或与该 Mx 记录存在依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="878dd-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="878dd-138">可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="878dd-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="878dd-139">ttl</span><span class="sxs-lookup"><span data-stu-id="878dd-139">ttl</span></span>|<span data-ttu-id="878dd-140">Int32</span><span class="sxs-lookup"><span data-stu-id="878dd-140">Int32</span></span>| <span data-ttu-id="878dd-p106">配置 DNS 主机上的 MX 记录的*生存时间 (ttl)* 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="878dd-p106">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="878dd-143">关系</span><span class="sxs-lookup"><span data-stu-id="878dd-143">Relationships</span></span>
<span data-ttu-id="878dd-144">无</span><span class="sxs-lookup"><span data-stu-id="878dd-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="878dd-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="878dd-145">JSON representation</span></span>
<span data-ttu-id="878dd-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="878dd-146">Here is a JSON representation of the resource.</span></span>

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