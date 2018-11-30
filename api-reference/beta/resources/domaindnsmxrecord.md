---
title: domainDnsMxRecord 资源类型
description: 表示已添加到租户中特定域的 DNS 区域文件的 MX 记录。继承自 DomainDnsRecord 实体。
ms.openlocfilehash: 51a99efbb9929064809bbd00364c72ffe2ed8651
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041492"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="2a499-104">domainDnsMxRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a499-104">domainDnsMxRecord resource type</span></span>

> <span data-ttu-id="2a499-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2a499-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a499-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2a499-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2a499-p103">表示已添加到租户中特定域的 DNS 区域文件的 MX 记录。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="2a499-p103">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="2a499-109">方法</span><span class="sxs-lookup"><span data-stu-id="2a499-109">Methods</span></span>
<span data-ttu-id="2a499-p104">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="2a499-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="2a499-112">属性</span><span class="sxs-lookup"><span data-stu-id="2a499-112">Properties</span></span>
| <span data-ttu-id="2a499-113">属性</span><span class="sxs-lookup"><span data-stu-id="2a499-113">Property</span></span>     | <span data-ttu-id="2a499-114">类型</span><span class="sxs-lookup"><span data-stu-id="2a499-114">Type</span></span>   |<span data-ttu-id="2a499-115">说明</span><span class="sxs-lookup"><span data-stu-id="2a499-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a499-116">id</span><span class="sxs-lookup"><span data-stu-id="2a499-116">id</span></span>|<span data-ttu-id="2a499-117">字符串</span><span class="sxs-lookup"><span data-stu-id="2a499-117">String</span></span>| <span data-ttu-id="2a499-p105">分配给此实体的唯一标识符。不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="2a499-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="2a499-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="2a499-120">isOptional</span></span>|<span data-ttu-id="2a499-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a499-121">Boolean</span></span>| <span data-ttu-id="2a499-122">如果为 false，则客户必须在 DNS 主机上配置 MX 记录才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="2a499-122">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="2a499-123">label</span><span class="sxs-lookup"><span data-stu-id="2a499-123">label</span></span>|<span data-ttu-id="2a499-124">String</span><span class="sxs-lookup"><span data-stu-id="2a499-124">String</span></span>| <span data-ttu-id="2a499-125">配置 DNS 主机上的 MX 记录的*别名/主机/名称*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="2a499-125">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="2a499-126">mailExchange</span><span class="sxs-lookup"><span data-stu-id="2a499-126">mailExchange</span></span>|<span data-ttu-id="2a499-127">String</span><span class="sxs-lookup"><span data-stu-id="2a499-127">String</span></span>| <span data-ttu-id="2a499-128">配置 DNS 主机上的 MX 记录的*答复/目标/值*时使用的值。</span><span class="sxs-lookup"><span data-stu-id="2a499-128">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="2a499-129">preference</span><span class="sxs-lookup"><span data-stu-id="2a499-129">preference</span></span>|<span data-ttu-id="2a499-130">Int32</span><span class="sxs-lookup"><span data-stu-id="2a499-130">Int32</span></span>| <span data-ttu-id="2a499-131">配置 DNS 主机上的 MX 记录的*首选项/优先级*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="2a499-131">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="2a499-132">recordType</span><span class="sxs-lookup"><span data-stu-id="2a499-132">recordType</span></span>|<span data-ttu-id="2a499-133">String</span><span class="sxs-lookup"><span data-stu-id="2a499-133">String</span></span>| <span data-ttu-id="2a499-p106">DNS 记录类型。此值始终是 *Mx*。Key</span><span class="sxs-lookup"><span data-stu-id="2a499-p106">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="2a499-137">supportedService</span><span class="sxs-lookup"><span data-stu-id="2a499-137">supportedService</span></span>|<span data-ttu-id="2a499-138">String</span><span class="sxs-lookup"><span data-stu-id="2a499-138">String</span></span>| <span data-ttu-id="2a499-139">Microsoft Online Service 或与该 Mx 记录存在依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="2a499-139">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="2a499-140">可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="2a499-140">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="2a499-141">ttl</span><span class="sxs-lookup"><span data-stu-id="2a499-141">ttl</span></span>|<span data-ttu-id="2a499-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2a499-142">Int32</span></span>| <span data-ttu-id="2a499-p107">配置 DNS 主机上的 MX 记录的*生存时间 (ttl)* 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="2a499-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="2a499-145">关系</span><span class="sxs-lookup"><span data-stu-id="2a499-145">Relationships</span></span>
<span data-ttu-id="2a499-146">无</span><span class="sxs-lookup"><span data-stu-id="2a499-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a499-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a499-147">JSON representation</span></span>
<span data-ttu-id="2a499-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a499-148">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->