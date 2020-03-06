---
title: domainDnsUnavailableRecord 资源类型
description: 当您查询 Domain 实体的导航属性**serviceConfigurationRecords**时，您可能会返回一个或多个 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord 和/或 DomainDnsTxtRecord 实体。 这些实体指示您必须添加到域的区域文件中的 DNS 记录，在 Microsoft Online Services 可使用域之前。 如果不能生成此类实体，则改为返回 DomainDnsUnavailableRecord 实体。 继承自 DomainDnsRecord 实体。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 50616237d446f2feb22dd394e018a9a23bfe850b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531582"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="c3c52-106">domainDnsUnavailableRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3c52-106">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="c3c52-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3c52-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3c52-108">当您查询[Domain](domain.md)实体的导航属性**serviceConfigurationRecords**时，您可能会返回一个或多个[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md)和/或[DomainDnsTxtRecord](domaindnstxtrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="c3c52-108">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="c3c52-109">这些实体指示您必须添加到域的区域文件中的 DNS 记录，在 Microsoft Online Services 可使用域之前。</span><span class="sxs-lookup"><span data-stu-id="c3c52-109">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="c3c52-110">如果不能生成此类实体，则改为返回 DomainDnsUnavailableRecord 实体。</span><span class="sxs-lookup"><span data-stu-id="c3c52-110">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="c3c52-111">继承自[DomainDnsRecord](domaindnsrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="c3c52-111">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="c3c52-112">Methods</span><span class="sxs-lookup"><span data-stu-id="c3c52-112">Methods</span></span>
<span data-ttu-id="c3c52-113">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="c3c52-113">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="c3c52-114">有关如何查询域服务记录的信息，请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="c3c52-114">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="c3c52-115">属性</span><span class="sxs-lookup"><span data-stu-id="c3c52-115">Properties</span></span>
| <span data-ttu-id="c3c52-116">属性</span><span class="sxs-lookup"><span data-stu-id="c3c52-116">Property</span></span>     | <span data-ttu-id="c3c52-117">类型</span><span class="sxs-lookup"><span data-stu-id="c3c52-117">Type</span></span>   |<span data-ttu-id="c3c52-118">说明</span><span class="sxs-lookup"><span data-stu-id="c3c52-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3c52-119">说明</span><span class="sxs-lookup"><span data-stu-id="c3c52-119">description</span></span>|<span data-ttu-id="c3c52-120">字符串</span><span class="sxs-lookup"><span data-stu-id="c3c52-120">String</span></span>|<span data-ttu-id="c3c52-121">提供**DomainDnsUnavailableRecord**实体返回的原因。</span><span class="sxs-lookup"><span data-stu-id="c3c52-121">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c3c52-122">关系</span><span class="sxs-lookup"><span data-stu-id="c3c52-122">Relationships</span></span>
<span data-ttu-id="c3c52-123">无</span><span class="sxs-lookup"><span data-stu-id="c3c52-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3c52-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3c52-124">JSON representation</span></span>
<span data-ttu-id="c3c52-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3c52-125">Here is a JSON representation of the resource.</span></span>

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
