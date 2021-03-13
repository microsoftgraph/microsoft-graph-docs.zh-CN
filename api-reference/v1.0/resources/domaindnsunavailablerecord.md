---
title: domainDnsUnavailableRecord 资源类型
description: 指示无法生成 serviceConfigurationRecords。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6cb35152b6d31e313342f7bfea99bfc98c51635b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761372"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="5acb1-103">domainDnsUnavailableRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="5acb1-103">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="5acb1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5acb1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5acb1-105">查询 [Domain](domain.md)实体的导航属性 **serviceConfigurationRecords** 时，可以返回一个或多个 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord 和/或 [DomainDnsTxtRecord](domaindnstxtrecord.md)实体。 [](domaindnscnamerecord.md) [](domaindnsmxrecord.md) [](domaindnssrvrecord.md)</span><span class="sxs-lookup"><span data-stu-id="5acb1-105">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="5acb1-106">这些实体指示必须在域的区域文件中添加哪些 DNS 记录，然后该域才能由 Microsoft Online Services。</span><span class="sxs-lookup"><span data-stu-id="5acb1-106">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="5acb1-107">如果无法生成此类实体，则改为返回 DomainDnsUnavailableRecord Entity。</span><span class="sxs-lookup"><span data-stu-id="5acb1-107">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="5acb1-108">继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="5acb1-108">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="5acb1-109">方法</span><span class="sxs-lookup"><span data-stu-id="5acb1-109">Methods</span></span>
<span data-ttu-id="5acb1-110">不支持直接查询此资源。</span><span class="sxs-lookup"><span data-stu-id="5acb1-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="5acb1-111">请参阅 [域主题](domain.md) ，了解如何查询域服务记录。</span><span class="sxs-lookup"><span data-stu-id="5acb1-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="5acb1-112">属性</span><span class="sxs-lookup"><span data-stu-id="5acb1-112">Properties</span></span>
| <span data-ttu-id="5acb1-113">属性</span><span class="sxs-lookup"><span data-stu-id="5acb1-113">Property</span></span>     | <span data-ttu-id="5acb1-114">类型</span><span class="sxs-lookup"><span data-stu-id="5acb1-114">Type</span></span>   |<span data-ttu-id="5acb1-115">说明</span><span class="sxs-lookup"><span data-stu-id="5acb1-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5acb1-116">说明</span><span class="sxs-lookup"><span data-stu-id="5acb1-116">description</span></span>|<span data-ttu-id="5acb1-117">字符串</span><span class="sxs-lookup"><span data-stu-id="5acb1-117">String</span></span>|<span data-ttu-id="5acb1-118">提供返回 **DomainDnsUnavailableRecord** 实体的原因。</span><span class="sxs-lookup"><span data-stu-id="5acb1-118">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5acb1-119">关系</span><span class="sxs-lookup"><span data-stu-id="5acb1-119">Relationships</span></span>
<span data-ttu-id="5acb1-120">无</span><span class="sxs-lookup"><span data-stu-id="5acb1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5acb1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5acb1-121">JSON representation</span></span>
<span data-ttu-id="5acb1-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5acb1-122">Here is a JSON representation of the resource.</span></span>

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

