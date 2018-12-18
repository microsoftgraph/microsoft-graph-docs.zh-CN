---
title: domainDnsCnameRecord 资源类型
description: 表示已添加到租户中特定域的 DNS 区域文件的 CNAME 记录。继承自 DomainDnsRecord 实体。
author: lleonard-msft
ms.openlocfilehash: 0ce5a748d9a1b558b4ac49e104eb9498efe674aa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315839"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="81801-104">domainDnsCnameRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="81801-104">domainDnsCnameRecord resource type</span></span>

> <span data-ttu-id="81801-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="81801-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81801-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="81801-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81801-p103">表示已添加到租户中特定域的 DNS 区域文件的 CNAME 记录。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="81801-p103">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="81801-109">方法</span><span class="sxs-lookup"><span data-stu-id="81801-109">Methods</span></span>
<span data-ttu-id="81801-p104">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="81801-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="81801-112">属性</span><span class="sxs-lookup"><span data-stu-id="81801-112">Properties</span></span>
| <span data-ttu-id="81801-113">属性</span><span class="sxs-lookup"><span data-stu-id="81801-113">Property</span></span>     | <span data-ttu-id="81801-114">类型</span><span class="sxs-lookup"><span data-stu-id="81801-114">Type</span></span>   |<span data-ttu-id="81801-115">说明</span><span class="sxs-lookup"><span data-stu-id="81801-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81801-116">canonicalName</span><span class="sxs-lookup"><span data-stu-id="81801-116">canonicalName</span></span>|<span data-ttu-id="81801-117">字符串</span><span class="sxs-lookup"><span data-stu-id="81801-117">String</span></span>| <span data-ttu-id="81801-p105">CNAME 记录的规范名称。用于配置 DNS 主机上的 CNAME 记录。</span><span class="sxs-lookup"><span data-stu-id="81801-p105">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="81801-120">id</span><span class="sxs-lookup"><span data-stu-id="81801-120">id</span></span>|<span data-ttu-id="81801-121">字符串</span><span class="sxs-lookup"><span data-stu-id="81801-121">String</span></span>| <span data-ttu-id="81801-p106">分配给该实体的唯一标识符。不可为 NULL，只读</span><span class="sxs-lookup"><span data-stu-id="81801-p106">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="81801-124">isOptional</span><span class="sxs-lookup"><span data-stu-id="81801-124">isOptional</span></span>|<span data-ttu-id="81801-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="81801-125">Boolean</span></span>| <span data-ttu-id="81801-p107">如果为 false，则客户必须在 DNS 主机上配置 CNAME 记录才能使 Microsoft Online Services 在域中正常运行。不可为 null</span><span class="sxs-lookup"><span data-stu-id="81801-p107">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="81801-128">标签</span><span class="sxs-lookup"><span data-stu-id="81801-128">label</span></span>|<span data-ttu-id="81801-129">String</span><span class="sxs-lookup"><span data-stu-id="81801-129">String</span></span>| <span data-ttu-id="81801-130">配置 DNS 主机上的 CNAME 记录的*别名/主机/名称*时使用的值。</span><span class="sxs-lookup"><span data-stu-id="81801-130">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="81801-131">recordType</span><span class="sxs-lookup"><span data-stu-id="81801-131">recordType</span></span>|<span data-ttu-id="81801-132">String</span><span class="sxs-lookup"><span data-stu-id="81801-132">String</span></span>| <span data-ttu-id="81801-p108">DNS 记录类型。此值始终是 *CName*。键</span><span class="sxs-lookup"><span data-stu-id="81801-p108">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="81801-136">supportedService</span><span class="sxs-lookup"><span data-stu-id="81801-136">supportedService</span></span>|<span data-ttu-id="81801-137">String</span><span class="sxs-lookup"><span data-stu-id="81801-137">String</span></span>| <span data-ttu-id="81801-138">Microsoft Online Service 或与该 CNAME 记录存在依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="81801-138">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="81801-139">可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="81801-139">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="81801-140">ttl</span><span class="sxs-lookup"><span data-stu-id="81801-140">ttl</span></span>|<span data-ttu-id="81801-141">Int32</span><span class="sxs-lookup"><span data-stu-id="81801-141">Int32</span></span>| <span data-ttu-id="81801-p109">配置 DNS 主机上的 CNAME 记录的生存时间 (ttl) 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="81801-p109">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="81801-144">关系</span><span class="sxs-lookup"><span data-stu-id="81801-144">Relationships</span></span>
<span data-ttu-id="81801-145">无</span><span class="sxs-lookup"><span data-stu-id="81801-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="81801-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81801-146">JSON representation</span></span>
<span data-ttu-id="81801-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81801-147">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->