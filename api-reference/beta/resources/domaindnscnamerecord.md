---
title: domainDnsCnameRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件中的 CNAME 记录。 继承自 DomainDnsRecord 实体。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9b3a957197821bfb010aed5de071ec1e89192828
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506363"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="ab1c5-104">domainDnsCnameRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab1c5-104">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="ab1c5-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ab1c5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab1c5-106">表示添加到租户中特定域的 DNS 区域文件中的 CNAME 记录。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-106">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="ab1c5-107">继承自[DomainDnsRecord](domaindnsrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="ab1c5-108">方法</span><span class="sxs-lookup"><span data-stu-id="ab1c5-108">Methods</span></span>
<span data-ttu-id="ab1c5-109">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="ab1c5-110">有关如何查询域服务记录的信息，请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="ab1c5-111">属性</span><span class="sxs-lookup"><span data-stu-id="ab1c5-111">Properties</span></span>
| <span data-ttu-id="ab1c5-112">属性</span><span class="sxs-lookup"><span data-stu-id="ab1c5-112">Property</span></span>     | <span data-ttu-id="ab1c5-113">类型</span><span class="sxs-lookup"><span data-stu-id="ab1c5-113">Type</span></span>   |<span data-ttu-id="ab1c5-114">说明</span><span class="sxs-lookup"><span data-stu-id="ab1c5-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab1c5-115">canonicalName</span><span class="sxs-lookup"><span data-stu-id="ab1c5-115">canonicalName</span></span>|<span data-ttu-id="ab1c5-116">String</span><span class="sxs-lookup"><span data-stu-id="ab1c5-116">String</span></span>| <span data-ttu-id="ab1c5-117">CNAME 记录的规范名称。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-117">The canonical name of the CNAME record.</span></span> <span data-ttu-id="ab1c5-118">用于配置 DNS 主机上的 CNAME 记录。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-118">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="ab1c5-119">id</span><span class="sxs-lookup"><span data-stu-id="ab1c5-119">id</span></span>|<span data-ttu-id="ab1c5-120">String</span><span class="sxs-lookup"><span data-stu-id="ab1c5-120">String</span></span>| <span data-ttu-id="ab1c5-121">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-121">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="ab1c5-122">不可为 null 的只读</span><span class="sxs-lookup"><span data-stu-id="ab1c5-122">Not nullable, Read-only</span></span>|
|<span data-ttu-id="ab1c5-123">isOptional</span><span class="sxs-lookup"><span data-stu-id="ab1c5-123">isOptional</span></span>|<span data-ttu-id="ab1c5-124">布尔</span><span class="sxs-lookup"><span data-stu-id="ab1c5-124">Boolean</span></span>| <span data-ttu-id="ab1c5-125">如果为 false，则客户必须在 DNS 主机上配置 CNAME 记录，才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-125">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="ab1c5-126">不可为 null</span><span class="sxs-lookup"><span data-stu-id="ab1c5-126">Not nullable</span></span> |
|<span data-ttu-id="ab1c5-127">label</span><span class="sxs-lookup"><span data-stu-id="ab1c5-127">label</span></span>|<span data-ttu-id="ab1c5-128">String</span><span class="sxs-lookup"><span data-stu-id="ab1c5-128">String</span></span>| <span data-ttu-id="ab1c5-129">配置 DNS 主机上的 CNAME 记录的*别名/主机/名称*时使用的值。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-129">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="ab1c5-130">recordType</span><span class="sxs-lookup"><span data-stu-id="ab1c5-130">recordType</span></span>|<span data-ttu-id="ab1c5-131">String</span><span class="sxs-lookup"><span data-stu-id="ab1c5-131">String</span></span>| <span data-ttu-id="ab1c5-132">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-132">Type of DNS record.</span></span> <span data-ttu-id="ab1c5-133">值始终为*CName*。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-133">The value is always *CName*.</span></span> <span data-ttu-id="ab1c5-134">键</span><span class="sxs-lookup"><span data-stu-id="ab1c5-134">Key</span></span>|
|<span data-ttu-id="ab1c5-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="ab1c5-135">supportedService</span></span>|<span data-ttu-id="ab1c5-136">String</span><span class="sxs-lookup"><span data-stu-id="ab1c5-136">String</span></span>| <span data-ttu-id="ab1c5-137">对此 CNAME 记录具有依赖关系的 Microsoft Online 服务或功能。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-137">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="ab1c5-138">可以是下列值之一： **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="ab1c5-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="ab1c5-139">ttl</span><span class="sxs-lookup"><span data-stu-id="ab1c5-139">ttl</span></span>|<span data-ttu-id="ab1c5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ab1c5-140">Int32</span></span>| <span data-ttu-id="ab1c5-141">配置 DNS 主机上的 CNAME 记录的生存时间（ttl）属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-141">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="ab1c5-142">不可为 null</span><span class="sxs-lookup"><span data-stu-id="ab1c5-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="ab1c5-143">关系</span><span class="sxs-lookup"><span data-stu-id="ab1c5-143">Relationships</span></span>
<span data-ttu-id="ab1c5-144">无</span><span class="sxs-lookup"><span data-stu-id="ab1c5-144">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ab1c5-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab1c5-145">JSON representation</span></span>
<span data-ttu-id="ab1c5-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab1c5-146">Here is a JSON representation of the resource.</span></span>

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
