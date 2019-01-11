---
title: singleValueLegacyExtendedProperty 资源类型
description: '包含单个值的扩展属性。 '
localization_priority: Normal
ms.openlocfilehash: f865da1a8a4211ac99a70881b2851b38b8e72727
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894227"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="fd949-103">singleValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd949-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="fd949-104">包含单个值的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fd949-104">An extended property that contains a single value.</span></span> 

<span data-ttu-id="fd949-105">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="fd949-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="fd949-106">方法</span><span class="sxs-lookup"><span data-stu-id="fd949-106">Methods</span></span>

| <span data-ttu-id="fd949-107">方法</span><span class="sxs-lookup"><span data-stu-id="fd949-107">Method</span></span>           | <span data-ttu-id="fd949-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="fd949-108">Return Type</span></span>    |<span data-ttu-id="fd949-109">说明</span><span class="sxs-lookup"><span data-stu-id="fd949-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd949-110">帖子</span><span class="sxs-lookup"><span data-stu-id="fd949-110">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="fd949-111">受支持的资源实例有：[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md) 或 [contactFolder](../resources/contactfolder.md)，但没有 [post](../resources/post.md) 组。</span><span class="sxs-lookup"><span data-stu-id="fd949-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="fd949-112">在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="fd949-112">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="fd949-113">获取</span><span class="sxs-lookup"><span data-stu-id="fd949-113">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="fd949-114">一个或多个受支持的资源实例（[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md)、[contactFolder](../resources/contactfolder.md) 或[post](../resources/post.md) 组），或通过 [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 对象扩展的一个此类的实例。</span><span class="sxs-lookup"><span data-stu-id="fd949-114">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="fd949-115">使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="fd949-115">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="fd949-116">属性</span><span class="sxs-lookup"><span data-stu-id="fd949-116">Properties</span></span>
| <span data-ttu-id="fd949-117">属性</span><span class="sxs-lookup"><span data-stu-id="fd949-117">Property</span></span>     | <span data-ttu-id="fd949-118">类型</span><span class="sxs-lookup"><span data-stu-id="fd949-118">Type</span></span>   |<span data-ttu-id="fd949-119">说明</span><span class="sxs-lookup"><span data-stu-id="fd949-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd949-120">ID</span><span class="sxs-lookup"><span data-stu-id="fd949-120">id</span></span>|<span data-ttu-id="fd949-121">string</span><span class="sxs-lookup"><span data-stu-id="fd949-121">string</span></span>|<span data-ttu-id="fd949-p101">用于标识属性的属性 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="fd949-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="fd949-124">value</span><span class="sxs-lookup"><span data-stu-id="fd949-124">value</span></span>|<span data-ttu-id="fd949-125">string</span><span class="sxs-lookup"><span data-stu-id="fd949-125">string</span></span>|<span data-ttu-id="fd949-126">属性值。</span><span class="sxs-lookup"><span data-stu-id="fd949-126">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd949-127">Relationships</span><span class="sxs-lookup"><span data-stu-id="fd949-127">Relationships</span></span>
<span data-ttu-id="fd949-128">无</span><span class="sxs-lookup"><span data-stu-id="fd949-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fd949-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd949-129">JSON representation</span></span>

<span data-ttu-id="fd949-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd949-130">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
