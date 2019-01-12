---
title: domainDnsUnavailableRecord 资源类型
description: 当您的域实体的导航属性**serviceConfigurationRecords**查询时，可能会返回一个或多个 DomainDnsCnameRecord、 DomainDnsMxRecord、 DomainDnsSrvRecord，和/或 DomainDnsTxtRecord 实体。 这些实体指示您必须先将添加到区域文件域的域可由 Microsoft Online Services 何种 DNS 记录。 当不可能生成此类实体时，而被返回 DomainDnsUnavailableRecord 实体。 继承自 DomainDnsRecord 实体。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99da0448d75375b84bb37c05102c1f702c222a25
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982790"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="2cb04-106">domainDnsUnavailableRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="2cb04-106">domainDnsUnavailableRecord resource type</span></span>

> <span data-ttu-id="2cb04-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2cb04-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cb04-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2cb04-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2cb04-p103">查询[域](domain.md)实体的导航属性 **serviceConfigurationRecords** 时，可能会返回一个或多个 [DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) 和/或 [DomainDnsTxtRecord](domaindnstxtrecord.md) 实体。这些实体指示 Microsoft Online Services 可以使用域前必须要添加到域的区域文件的 DNS 记录。无法生成这些实体时，将返回 DomainDnsUnavailableRecord 实体。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="2cb04-p103">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="2cb04-113">方法</span><span class="sxs-lookup"><span data-stu-id="2cb04-113">Methods</span></span>
<span data-ttu-id="2cb04-p104">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="2cb04-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="2cb04-116">属性</span><span class="sxs-lookup"><span data-stu-id="2cb04-116">Properties</span></span>
| <span data-ttu-id="2cb04-117">属性</span><span class="sxs-lookup"><span data-stu-id="2cb04-117">Property</span></span>     | <span data-ttu-id="2cb04-118">类型</span><span class="sxs-lookup"><span data-stu-id="2cb04-118">Type</span></span>   |<span data-ttu-id="2cb04-119">说明</span><span class="sxs-lookup"><span data-stu-id="2cb04-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2cb04-120">说明</span><span class="sxs-lookup"><span data-stu-id="2cb04-120">description</span></span>|<span data-ttu-id="2cb04-121">String</span><span class="sxs-lookup"><span data-stu-id="2cb04-121">String</span></span>|<span data-ttu-id="2cb04-122">提供返回 **DomainDnsUnavailableRecord** 实体的原因。</span><span class="sxs-lookup"><span data-stu-id="2cb04-122">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2cb04-123">关系</span><span class="sxs-lookup"><span data-stu-id="2cb04-123">Relationships</span></span>
<span data-ttu-id="2cb04-124">无</span><span class="sxs-lookup"><span data-stu-id="2cb04-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cb04-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cb04-125">JSON representation</span></span>
<span data-ttu-id="2cb04-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cb04-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
