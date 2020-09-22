---
title: domainDnsUnavailableRecord 资源类型
description: 指示无法生成 serviceConfigurationRecords。
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aff0ef902a5e2c3d576be074f68078cc27a2df02
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018639"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="1a726-103">domainDnsUnavailableRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a726-103">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="1a726-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a726-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a726-105">当您查询[Domain](domain.md)实体的导航属性**serviceConfigurationRecords**时，您可能会返回一个或多个[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md)和/或[DomainDnsTxtRecord](domaindnstxtrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="1a726-105">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="1a726-106">这些实体指示您必须添加到域的区域文件中的 DNS 记录，在 Microsoft Online Services 可使用域之前。</span><span class="sxs-lookup"><span data-stu-id="1a726-106">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="1a726-107">如果不能生成此类实体，则改为返回 DomainDnsUnavailableRecord 实体。</span><span class="sxs-lookup"><span data-stu-id="1a726-107">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="1a726-108">继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="1a726-108">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="1a726-109">方法</span><span class="sxs-lookup"><span data-stu-id="1a726-109">Methods</span></span>
<span data-ttu-id="1a726-110">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="1a726-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="1a726-111">有关如何查询域服务记录的信息，请参阅 [域](domain.md) 主题。</span><span class="sxs-lookup"><span data-stu-id="1a726-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="1a726-112">属性</span><span class="sxs-lookup"><span data-stu-id="1a726-112">Properties</span></span>
| <span data-ttu-id="1a726-113">属性</span><span class="sxs-lookup"><span data-stu-id="1a726-113">Property</span></span>     | <span data-ttu-id="1a726-114">类型</span><span class="sxs-lookup"><span data-stu-id="1a726-114">Type</span></span>   |<span data-ttu-id="1a726-115">说明</span><span class="sxs-lookup"><span data-stu-id="1a726-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a726-116">说明</span><span class="sxs-lookup"><span data-stu-id="1a726-116">description</span></span>|<span data-ttu-id="1a726-117">String</span><span class="sxs-lookup"><span data-stu-id="1a726-117">String</span></span>|<span data-ttu-id="1a726-118">提供 **DomainDnsUnavailableRecord** 实体返回的原因。</span><span class="sxs-lookup"><span data-stu-id="1a726-118">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1a726-119">关系</span><span class="sxs-lookup"><span data-stu-id="1a726-119">Relationships</span></span>
<span data-ttu-id="1a726-120">无</span><span class="sxs-lookup"><span data-stu-id="1a726-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a726-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a726-121">JSON representation</span></span>
<span data-ttu-id="1a726-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a726-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
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

