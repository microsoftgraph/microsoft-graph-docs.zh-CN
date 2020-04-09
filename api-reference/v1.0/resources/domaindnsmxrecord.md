---
title: domainDnsMxRecord 资源类型
description: 表示添加到租户中特定域的 DNS 区域文件中的 MX 记录。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: af95edfde834e04449398b1a9b306fe29529a15d
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181649"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="8fd9e-103">domainDnsMxRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fd9e-103">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="8fd9e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fd9e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8fd9e-105">表示添加到租户中特定域的 DNS 区域文件中的 MX 记录。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-105">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="8fd9e-106">继承自[DomainDnsRecord](domaindnsrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="8fd9e-107">方法</span><span class="sxs-lookup"><span data-stu-id="8fd9e-107">Methods</span></span>
<span data-ttu-id="8fd9e-108">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="8fd9e-109">有关如何查询域服务记录的信息，请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="8fd9e-110">属性</span><span class="sxs-lookup"><span data-stu-id="8fd9e-110">Properties</span></span>
| <span data-ttu-id="8fd9e-111">属性</span><span class="sxs-lookup"><span data-stu-id="8fd9e-111">Property</span></span>     | <span data-ttu-id="8fd9e-112">类型</span><span class="sxs-lookup"><span data-stu-id="8fd9e-112">Type</span></span>   |<span data-ttu-id="8fd9e-113">说明</span><span class="sxs-lookup"><span data-stu-id="8fd9e-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fd9e-114">id</span><span class="sxs-lookup"><span data-stu-id="8fd9e-114">id</span></span>|<span data-ttu-id="8fd9e-115">字符串</span><span class="sxs-lookup"><span data-stu-id="8fd9e-115">String</span></span>| <span data-ttu-id="8fd9e-116">分配给此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="8fd9e-117">不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="8fd9e-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="8fd9e-118">isOptional</span></span>|<span data-ttu-id="8fd9e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fd9e-119">Boolean</span></span>| <span data-ttu-id="8fd9e-120">如果为 false，则客户必须在 DNS 主机上配置 MX 记录，才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="8fd9e-121">label</span><span class="sxs-lookup"><span data-stu-id="8fd9e-121">label</span></span>|<span data-ttu-id="8fd9e-122">字符串</span><span class="sxs-lookup"><span data-stu-id="8fd9e-122">String</span></span>| <span data-ttu-id="8fd9e-123">配置 DNS 主机上的 MX 记录的*别名/主机/名称*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="8fd9e-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="8fd9e-124">mailExchange</span></span>|<span data-ttu-id="8fd9e-125">字符串</span><span class="sxs-lookup"><span data-stu-id="8fd9e-125">String</span></span>| <span data-ttu-id="8fd9e-126">配置 DNS 主机上的 MX 记录的*应答/目标/值*时使用的值。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="8fd9e-127">优先权</span><span class="sxs-lookup"><span data-stu-id="8fd9e-127">preference</span></span>|<span data-ttu-id="8fd9e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="8fd9e-128">Int32</span></span>| <span data-ttu-id="8fd9e-129">配置 DNS 主机上的 MX 记录的*首选项/优先级*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="8fd9e-130">recordType</span><span class="sxs-lookup"><span data-stu-id="8fd9e-130">recordType</span></span>|<span data-ttu-id="8fd9e-131">字符串</span><span class="sxs-lookup"><span data-stu-id="8fd9e-131">String</span></span>| <span data-ttu-id="8fd9e-132">DNS 记录的类型。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-132">Type of DNS record.</span></span> <span data-ttu-id="8fd9e-133">值始终为*Mx*。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-133">The value is always *Mx*.</span></span> <span data-ttu-id="8fd9e-134">键</span><span class="sxs-lookup"><span data-stu-id="8fd9e-134">Key</span></span> |
|<span data-ttu-id="8fd9e-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="8fd9e-135">supportedService</span></span>|<span data-ttu-id="8fd9e-136">字符串</span><span class="sxs-lookup"><span data-stu-id="8fd9e-136">String</span></span>| <span data-ttu-id="8fd9e-137">与此 MX 记录相关的 Microsoft Online 服务或功能。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="8fd9e-138">可以是下列值之一： **null**、 *Email*、 *Sharepoint*、 *EmailInternalRelayOnly*、 *OfficeCommunicationsOnline*、 *SharePointDefaultDomain*、 *FullRedelegation*、 *SharePointPublic*、 *OrgIdAuthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="8fd9e-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="8fd9e-139">ttl</span><span class="sxs-lookup"><span data-stu-id="8fd9e-139">ttl</span></span>|<span data-ttu-id="8fd9e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8fd9e-140">Int32</span></span>| <span data-ttu-id="8fd9e-141">配置 DNS 主机上的 MX 记录的*生存时间（ttl）* 属性时要使用的值。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-141">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="8fd9e-142">不可为 null</span><span class="sxs-lookup"><span data-stu-id="8fd9e-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="8fd9e-143">关系</span><span class="sxs-lookup"><span data-stu-id="8fd9e-143">Relationships</span></span>
<span data-ttu-id="8fd9e-144">无</span><span class="sxs-lookup"><span data-stu-id="8fd9e-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fd9e-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fd9e-145">JSON representation</span></span>
<span data-ttu-id="8fd9e-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-146">Here is a JSON representation of the resource.</span></span>

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
