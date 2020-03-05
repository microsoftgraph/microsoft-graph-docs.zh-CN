---
title: domainDnsUnavailableRecord 资源类型
description: 当您查询 Domain 实体的导航属性**serviceConfigurationRecords**时，您可能会返回一个或多个 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord 和/或 DomainDnsTxtRecord 实体。 这些实体指示您必须添加到域的区域文件中的 DNS 记录，在 Microsoft Online Services 可使用域之前。 如果不能生成此类实体，则改为返回 DomainDnsUnavailableRecord 实体。 继承自 DomainDnsRecord 实体。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9743d1f9a4db1018f1b704b45b8236aeda6d5cd9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505810"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="5336c-106">domainDnsUnavailableRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="5336c-106">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="5336c-107">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5336c-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5336c-108">当您查询[Domain](domain.md)实体的导航属性**serviceConfigurationRecords**时，您可能会返回一个或多个[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md)和/或[DomainDnsTxtRecord](domaindnstxtrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="5336c-108">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="5336c-109">这些实体指示您必须添加到域的区域文件中的 DNS 记录，在 Microsoft Online Services 可使用域之前。</span><span class="sxs-lookup"><span data-stu-id="5336c-109">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="5336c-110">如果不能生成此类实体，则改为返回 DomainDnsUnavailableRecord 实体。</span><span class="sxs-lookup"><span data-stu-id="5336c-110">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="5336c-111">继承自[DomainDnsRecord](domaindnsrecord.md)实体。</span><span class="sxs-lookup"><span data-stu-id="5336c-111">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="5336c-112">方法</span><span class="sxs-lookup"><span data-stu-id="5336c-112">Methods</span></span>
<span data-ttu-id="5336c-113">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="5336c-113">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="5336c-114">有关如何查询域服务记录的信息，请参阅[域](domain.md)主题。</span><span class="sxs-lookup"><span data-stu-id="5336c-114">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="5336c-115">属性</span><span class="sxs-lookup"><span data-stu-id="5336c-115">Properties</span></span>
| <span data-ttu-id="5336c-116">属性</span><span class="sxs-lookup"><span data-stu-id="5336c-116">Property</span></span>     | <span data-ttu-id="5336c-117">类型</span><span class="sxs-lookup"><span data-stu-id="5336c-117">Type</span></span>   |<span data-ttu-id="5336c-118">说明</span><span class="sxs-lookup"><span data-stu-id="5336c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5336c-119">说明</span><span class="sxs-lookup"><span data-stu-id="5336c-119">description</span></span>|<span data-ttu-id="5336c-120">String</span><span class="sxs-lookup"><span data-stu-id="5336c-120">String</span></span>|<span data-ttu-id="5336c-121">提供**DomainDnsUnavailableRecord**实体返回的原因。</span><span class="sxs-lookup"><span data-stu-id="5336c-121">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5336c-122">关系</span><span class="sxs-lookup"><span data-stu-id="5336c-122">Relationships</span></span>
<span data-ttu-id="5336c-123">无</span><span class="sxs-lookup"><span data-stu-id="5336c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5336c-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5336c-124">JSON representation</span></span>
<span data-ttu-id="5336c-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5336c-125">Here is a JSON representation of the resource.</span></span>

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
