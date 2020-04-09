---
title: domainDnsTxtRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件中的 TXT 记录。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c45845d984220997123f12e7558bf8ab300e679e
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181628"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="22e2b-103">domainDnsTxtRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="22e2b-103">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="22e2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22e2b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22e2b-105">表示添加到租户中特定域的 DNS 区域文件中的 TXT 记录。</span><span class="sxs-lookup"><span data-stu-id="22e2b-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="22e2b-106">继承自[DomainDnsRecord](domaindnsrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="22e2b-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="22e2b-107">方法</span><span class="sxs-lookup"><span data-stu-id="22e2b-107">Methods</span></span>
<span data-ttu-id="22e2b-108">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="22e2b-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="22e2b-109">有关如何查询域服务记录的信息，请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="22e2b-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="22e2b-110">属性</span><span class="sxs-lookup"><span data-stu-id="22e2b-110">Properties</span></span>
| <span data-ttu-id="22e2b-111">属性</span><span class="sxs-lookup"><span data-stu-id="22e2b-111">Property</span></span>     | <span data-ttu-id="22e2b-112">类型</span><span class="sxs-lookup"><span data-stu-id="22e2b-112">Type</span></span>   |<span data-ttu-id="22e2b-113">说明</span><span class="sxs-lookup"><span data-stu-id="22e2b-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22e2b-114">id</span><span class="sxs-lookup"><span data-stu-id="22e2b-114">id</span></span>|<span data-ttu-id="22e2b-115">字符串</span><span class="sxs-lookup"><span data-stu-id="22e2b-115">String</span></span>| <span data-ttu-id="22e2b-116">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="22e2b-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="22e2b-117">不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="22e2b-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="22e2b-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="22e2b-118">isOptional</span></span>|<span data-ttu-id="22e2b-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="22e2b-119">Boolean</span></span>| <span data-ttu-id="22e2b-120">如果为 false，则客户必须在 DNS 主机上配置 TXT 记录才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="22e2b-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="22e2b-121">label</span><span class="sxs-lookup"><span data-stu-id="22e2b-121">label</span></span>|<span data-ttu-id="22e2b-122">字符串</span><span class="sxs-lookup"><span data-stu-id="22e2b-122">String</span></span>| <span data-ttu-id="22e2b-123">配置 DNS 主机上的 TXT 记录的*name*属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="22e2b-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="22e2b-124">recordType</span><span class="sxs-lookup"><span data-stu-id="22e2b-124">recordType</span></span>|<span data-ttu-id="22e2b-125">字符串</span><span class="sxs-lookup"><span data-stu-id="22e2b-125">String</span></span>| <span data-ttu-id="22e2b-126">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="22e2b-126">Type of DNS record.</span></span> <span data-ttu-id="22e2b-127">值始终为*Txt*。</span><span class="sxs-lookup"><span data-stu-id="22e2b-127">The value is always *Txt*.</span></span> <span data-ttu-id="22e2b-128">键</span><span class="sxs-lookup"><span data-stu-id="22e2b-128">Key</span></span> |
|<span data-ttu-id="22e2b-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="22e2b-129">supportedService</span></span>|<span data-ttu-id="22e2b-130">字符串</span><span class="sxs-lookup"><span data-stu-id="22e2b-130">String</span></span>| <span data-ttu-id="22e2b-131">Microsoft Online Service 或与此 TXT 记录有依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="22e2b-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="22e2b-132">可以是下列值之一： **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="22e2b-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="22e2b-133">text</span><span class="sxs-lookup"><span data-stu-id="22e2b-133">text</span></span>|<span data-ttu-id="22e2b-134">字符串</span><span class="sxs-lookup"><span data-stu-id="22e2b-134">String</span></span>| <span data-ttu-id="22e2b-135">配置 DNS 主机上的*文本*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="22e2b-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="22e2b-136">ttl</span><span class="sxs-lookup"><span data-stu-id="22e2b-136">ttl</span></span>|<span data-ttu-id="22e2b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="22e2b-137">Int32</span></span>| <span data-ttu-id="22e2b-138">配置 DNS 主机上的 MX 记录的*生存时间（ttl）* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="22e2b-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="22e2b-139">不可为 null</span><span class="sxs-lookup"><span data-stu-id="22e2b-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="22e2b-140">关系</span><span class="sxs-lookup"><span data-stu-id="22e2b-140">Relationships</span></span>
<span data-ttu-id="22e2b-141">无</span><span class="sxs-lookup"><span data-stu-id="22e2b-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="22e2b-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22e2b-142">JSON representation</span></span>
<span data-ttu-id="22e2b-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22e2b-143">Here is a JSON representation of the resource.</span></span>

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
