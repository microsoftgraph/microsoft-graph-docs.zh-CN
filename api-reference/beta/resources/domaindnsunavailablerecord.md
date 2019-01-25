---
title: domainDnsUnavailableRecord 资源类型
description: 查询域实体的导航属性 serviceConfigurationRecords 时，可能会返回一个或多个 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord 和/或 DomainDnsTxtRecord 实体。这些实体指示 Microsoft Online Services 可以使用域前必须要添加到域的区域文件的 DNS 记录。无法生成这些实体时，将返回 DomainDnsUnavailableRecord 实体。继承自 DomainDnsRecord 实体。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fe3c1eeae7ae3ddb634a3c120332dd8d8996f41c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527869"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="f6dc6-106">domainDnsUnavailableRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6dc6-106">domainDnsUnavailableRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6dc6-p102">查询[域](domain.md)实体的导航属性 **serviceConfigurationRecords** 时，可能会返回一个或多个 [DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) 和/或 [DomainDnsTxtRecord](domaindnstxtrecord.md) 实体。这些实体指示 Microsoft Online Services 可以使用域前必须要添加到域的区域文件的 DNS 记录。无法生成这些实体时，将返回 DomainDnsUnavailableRecord 实体。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="f6dc6-p102">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="f6dc6-111">方法</span><span class="sxs-lookup"><span data-stu-id="f6dc6-111">Methods</span></span>
<span data-ttu-id="f6dc6-p103">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="f6dc6-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="f6dc6-114">属性</span><span class="sxs-lookup"><span data-stu-id="f6dc6-114">Properties</span></span>
| <span data-ttu-id="f6dc6-115">属性</span><span class="sxs-lookup"><span data-stu-id="f6dc6-115">Property</span></span>     | <span data-ttu-id="f6dc6-116">类型</span><span class="sxs-lookup"><span data-stu-id="f6dc6-116">Type</span></span>   |<span data-ttu-id="f6dc6-117">说明</span><span class="sxs-lookup"><span data-stu-id="f6dc6-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6dc6-118">说明</span><span class="sxs-lookup"><span data-stu-id="f6dc6-118">description</span></span>|<span data-ttu-id="f6dc6-119">String</span><span class="sxs-lookup"><span data-stu-id="f6dc6-119">String</span></span>|<span data-ttu-id="f6dc6-120">提供返回 **DomainDnsUnavailableRecord** 实体的原因。</span><span class="sxs-lookup"><span data-stu-id="f6dc6-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f6dc6-121">关系</span><span class="sxs-lookup"><span data-stu-id="f6dc6-121">Relationships</span></span>
<span data-ttu-id="f6dc6-122">无</span><span class="sxs-lookup"><span data-stu-id="f6dc6-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6dc6-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6dc6-123">JSON representation</span></span>
<span data-ttu-id="f6dc6-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6dc6-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnsunavailablerecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
