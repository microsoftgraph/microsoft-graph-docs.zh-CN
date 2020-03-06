---
title: domainDnsTxtRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件中的 TXT 记录。 继承自 DomainDnsRecord 实体。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a2899081dcc171feb2ae937ae1a742093c5133f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531589"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="489df-104">domainDnsTxtRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="489df-104">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="489df-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="489df-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="489df-106">表示添加到租户中特定域的 DNS 区域文件中的 TXT 记录。</span><span class="sxs-lookup"><span data-stu-id="489df-106">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="489df-107">继承自[DomainDnsRecord](domaindnsrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="489df-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="489df-108">Methods</span><span class="sxs-lookup"><span data-stu-id="489df-108">Methods</span></span>
<span data-ttu-id="489df-109">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="489df-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="489df-110">有关如何查询域服务记录的信息，请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="489df-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="489df-111">属性</span><span class="sxs-lookup"><span data-stu-id="489df-111">Properties</span></span>
| <span data-ttu-id="489df-112">属性</span><span class="sxs-lookup"><span data-stu-id="489df-112">Property</span></span>     | <span data-ttu-id="489df-113">类型</span><span class="sxs-lookup"><span data-stu-id="489df-113">Type</span></span>   |<span data-ttu-id="489df-114">说明</span><span class="sxs-lookup"><span data-stu-id="489df-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="489df-115">id</span><span class="sxs-lookup"><span data-stu-id="489df-115">id</span></span>|<span data-ttu-id="489df-116">字符串</span><span class="sxs-lookup"><span data-stu-id="489df-116">String</span></span>| <span data-ttu-id="489df-117">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="489df-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="489df-118">不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="489df-118">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="489df-119">isOptional</span><span class="sxs-lookup"><span data-stu-id="489df-119">isOptional</span></span>|<span data-ttu-id="489df-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="489df-120">Boolean</span></span>| <span data-ttu-id="489df-121">如果为 false，则客户必须在 DNS 主机上配置 TXT 记录才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="489df-121">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="489df-122">label</span><span class="sxs-lookup"><span data-stu-id="489df-122">label</span></span>|<span data-ttu-id="489df-123">字符串</span><span class="sxs-lookup"><span data-stu-id="489df-123">String</span></span>| <span data-ttu-id="489df-124">配置 DNS 主机上的 TXT 记录的*name*属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="489df-124">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="489df-125">recordType</span><span class="sxs-lookup"><span data-stu-id="489df-125">recordType</span></span>|<span data-ttu-id="489df-126">字符串</span><span class="sxs-lookup"><span data-stu-id="489df-126">String</span></span>| <span data-ttu-id="489df-127">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="489df-127">Type of DNS record.</span></span> <span data-ttu-id="489df-128">值始终为*Txt*。</span><span class="sxs-lookup"><span data-stu-id="489df-128">The value is always *Txt*.</span></span> <span data-ttu-id="489df-129">键</span><span class="sxs-lookup"><span data-stu-id="489df-129">Key</span></span> |
|<span data-ttu-id="489df-130">supportedService</span><span class="sxs-lookup"><span data-stu-id="489df-130">supportedService</span></span>|<span data-ttu-id="489df-131">字符串</span><span class="sxs-lookup"><span data-stu-id="489df-131">String</span></span>| <span data-ttu-id="489df-132">Microsoft Online Service 或与此 TXT 记录有依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="489df-132">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="489df-133">可以是下列值之一： **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="489df-133">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="489df-134">text</span><span class="sxs-lookup"><span data-stu-id="489df-134">text</span></span>|<span data-ttu-id="489df-135">字符串</span><span class="sxs-lookup"><span data-stu-id="489df-135">String</span></span>| <span data-ttu-id="489df-136">配置 DNS 主机上的*文本*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="489df-136">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="489df-137">ttl</span><span class="sxs-lookup"><span data-stu-id="489df-137">ttl</span></span>|<span data-ttu-id="489df-138">Int32</span><span class="sxs-lookup"><span data-stu-id="489df-138">Int32</span></span>| <span data-ttu-id="489df-139">配置 DNS 主机上的 MX 记录的*生存时间（ttl）* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="489df-139">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="489df-140">不可为 null</span><span class="sxs-lookup"><span data-stu-id="489df-140">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="489df-141">关系</span><span class="sxs-lookup"><span data-stu-id="489df-141">Relationships</span></span>
<span data-ttu-id="489df-142">无</span><span class="sxs-lookup"><span data-stu-id="489df-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="489df-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="489df-143">JSON representation</span></span>
<span data-ttu-id="489df-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="489df-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
