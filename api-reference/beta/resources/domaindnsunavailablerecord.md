---
title: domainDnsUnavailableRecord 资源类型
description: 当您查询 Domain 实体的导航属性**serviceConfigurationRecords**时, 您可能会返回一个或多个 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord 和/或 DomainDnsTxtRecord 实体。 这些实体指示您必须添加到域的区域文件中的 DNS 记录, 在 Microsoft Online Services 可使用域之前。 如果不能生成此类实体, 则改为返回 DomainDnsUnavailableRecord 实体。 继承自 DomainDnsRecord 实体。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f641170673a1b42f8a15c268ac08bf8097a7dfcb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340668"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="0d5cd-106">domainDnsUnavailableRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d5cd-106">domainDnsUnavailableRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d5cd-107">当您查询[Domain](domain.md)实体的导航属性**serviceConfigurationRecords**时, 您可能会收到一个或多个[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md)和/或[DomainDnsTxtRecord](domaindnstxtrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="0d5cd-107">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="0d5cd-108">这些实体指示您必须添加到域的区域文件中的 DNS 记录, 在 Microsoft Online Services 可使用域之前。</span><span class="sxs-lookup"><span data-stu-id="0d5cd-108">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="0d5cd-109">如果不能生成此类实体, 则改为返回 DomainDnsUnavailableRecord 实体。</span><span class="sxs-lookup"><span data-stu-id="0d5cd-109">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="0d5cd-110">继承自[DomainDnsRecord](domaindnsrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="0d5cd-110">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="0d5cd-111">方法</span><span class="sxs-lookup"><span data-stu-id="0d5cd-111">Methods</span></span>
<span data-ttu-id="0d5cd-112">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="0d5cd-112">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="0d5cd-113">有关如何查询域服务记录的信息, 请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="0d5cd-113">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="0d5cd-114">属性</span><span class="sxs-lookup"><span data-stu-id="0d5cd-114">Properties</span></span>
| <span data-ttu-id="0d5cd-115">属性</span><span class="sxs-lookup"><span data-stu-id="0d5cd-115">Property</span></span>     | <span data-ttu-id="0d5cd-116">类型</span><span class="sxs-lookup"><span data-stu-id="0d5cd-116">Type</span></span>   |<span data-ttu-id="0d5cd-117">说明</span><span class="sxs-lookup"><span data-stu-id="0d5cd-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d5cd-118">说明</span><span class="sxs-lookup"><span data-stu-id="0d5cd-118">description</span></span>|<span data-ttu-id="0d5cd-119">String</span><span class="sxs-lookup"><span data-stu-id="0d5cd-119">String</span></span>|<span data-ttu-id="0d5cd-120">提供**DomainDnsUnavailableRecord**实体返回的原因。</span><span class="sxs-lookup"><span data-stu-id="0d5cd-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0d5cd-121">关系</span><span class="sxs-lookup"><span data-stu-id="0d5cd-121">Relationships</span></span>
<span data-ttu-id="0d5cd-122">无</span><span class="sxs-lookup"><span data-stu-id="0d5cd-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d5cd-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d5cd-123">JSON representation</span></span>
<span data-ttu-id="0d5cd-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d5cd-124">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
