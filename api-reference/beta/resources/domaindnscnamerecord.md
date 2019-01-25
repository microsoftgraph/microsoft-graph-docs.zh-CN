---
title: domainDnsCnameRecord 资源类型
description: 表示已添加到租户中特定域的 DNS 区域文件的 CNAME 记录。继承自 DomainDnsRecord 实体。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f270075556843625d1ec408f06be8ed4a065c831
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516733"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="0506d-104">domainDnsCnameRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="0506d-104">domainDnsCnameRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0506d-p102">表示已添加到租户中特定域的 DNS 区域文件的 CNAME 记录。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="0506d-p102">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="0506d-107">方法</span><span class="sxs-lookup"><span data-stu-id="0506d-107">Methods</span></span>
<span data-ttu-id="0506d-p103">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="0506d-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="0506d-110">属性</span><span class="sxs-lookup"><span data-stu-id="0506d-110">Properties</span></span>
| <span data-ttu-id="0506d-111">属性</span><span class="sxs-lookup"><span data-stu-id="0506d-111">Property</span></span>     | <span data-ttu-id="0506d-112">类型</span><span class="sxs-lookup"><span data-stu-id="0506d-112">Type</span></span>   |<span data-ttu-id="0506d-113">说明</span><span class="sxs-lookup"><span data-stu-id="0506d-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0506d-114">canonicalName</span><span class="sxs-lookup"><span data-stu-id="0506d-114">canonicalName</span></span>|<span data-ttu-id="0506d-115">String</span><span class="sxs-lookup"><span data-stu-id="0506d-115">String</span></span>| <span data-ttu-id="0506d-p104">CNAME 记录的规范名称。用于配置 DNS 主机上的 CNAME 记录。</span><span class="sxs-lookup"><span data-stu-id="0506d-p104">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="0506d-118">id</span><span class="sxs-lookup"><span data-stu-id="0506d-118">id</span></span>|<span data-ttu-id="0506d-119">String</span><span class="sxs-lookup"><span data-stu-id="0506d-119">String</span></span>| <span data-ttu-id="0506d-p105">分配给该实体的唯一标识符。不可为 NULL，只读</span><span class="sxs-lookup"><span data-stu-id="0506d-p105">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="0506d-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="0506d-122">isOptional</span></span>|<span data-ttu-id="0506d-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0506d-123">Boolean</span></span>| <span data-ttu-id="0506d-p106">如果为 false，则客户必须在 DNS 主机上配置 CNAME 记录才能使 Microsoft Online Services 在域中正常运行。不可为 null</span><span class="sxs-lookup"><span data-stu-id="0506d-p106">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="0506d-126">标签</span><span class="sxs-lookup"><span data-stu-id="0506d-126">label</span></span>|<span data-ttu-id="0506d-127">字符串</span><span class="sxs-lookup"><span data-stu-id="0506d-127">String</span></span>| <span data-ttu-id="0506d-128">配置 DNS 主机上的 CNAME 记录的*别名/主机/名称*时使用的值。</span><span class="sxs-lookup"><span data-stu-id="0506d-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="0506d-129">recordType</span><span class="sxs-lookup"><span data-stu-id="0506d-129">recordType</span></span>|<span data-ttu-id="0506d-130">String</span><span class="sxs-lookup"><span data-stu-id="0506d-130">String</span></span>| <span data-ttu-id="0506d-p107">DNS 记录类型。此值始终是 *CName*。键</span><span class="sxs-lookup"><span data-stu-id="0506d-p107">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="0506d-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="0506d-134">supportedService</span></span>|<span data-ttu-id="0506d-135">String</span><span class="sxs-lookup"><span data-stu-id="0506d-135">String</span></span>| <span data-ttu-id="0506d-136">Microsoft Online Service 或与该 CNAME 记录存在依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="0506d-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="0506d-137">可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="0506d-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="0506d-138">ttl</span><span class="sxs-lookup"><span data-stu-id="0506d-138">ttl</span></span>|<span data-ttu-id="0506d-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0506d-139">Int32</span></span>| <span data-ttu-id="0506d-p108">配置 DNS 主机上的 CNAME 记录的生存时间 (ttl) 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="0506d-p108">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="0506d-142">关系</span><span class="sxs-lookup"><span data-stu-id="0506d-142">Relationships</span></span>
<span data-ttu-id="0506d-143">无</span><span class="sxs-lookup"><span data-stu-id="0506d-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0506d-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0506d-144">JSON representation</span></span>
<span data-ttu-id="0506d-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0506d-145">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnscnamerecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
