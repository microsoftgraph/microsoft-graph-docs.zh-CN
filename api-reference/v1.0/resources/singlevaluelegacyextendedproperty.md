---
title: singleValueLegacyExtendedProperty 资源类型
description: '包含单个值的扩展属性。 '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 030893ab3a5eaefad4637cfd50321f1653b41070
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334428"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="aaa46-103">singleValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="aaa46-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="aaa46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaa46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aaa46-105">包含单个值的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aaa46-105">An extended property that contains a single value.</span></span>

<span data-ttu-id="aaa46-106">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="aaa46-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>


## <a name="methods"></a><span data-ttu-id="aaa46-107">方法</span><span class="sxs-lookup"><span data-stu-id="aaa46-107">Methods</span></span>

| <span data-ttu-id="aaa46-108">方法</span><span class="sxs-lookup"><span data-stu-id="aaa46-108">Method</span></span>           | <span data-ttu-id="aaa46-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="aaa46-109">Return Type</span></span>    |<span data-ttu-id="aaa46-110">说明</span><span class="sxs-lookup"><span data-stu-id="aaa46-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aaa46-111">Post</span><span class="sxs-lookup"><span data-stu-id="aaa46-111">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="aaa46-112">受支持的资源实例有：[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md) 或 [contactFolder](../resources/contactfolder.md)，但没有 [post](../resources/post.md) 组。</span><span class="sxs-lookup"><span data-stu-id="aaa46-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="aaa46-113">在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="aaa46-113">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="aaa46-114">获取</span><span class="sxs-lookup"><span data-stu-id="aaa46-114">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="aaa46-115">一个或多个受支持的资源实例（[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md)、[contactFolder](../resources/contactfolder.md) 或[post](../resources/post.md) 组），或通过 [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 对象扩展的一个此类的实例。</span><span class="sxs-lookup"><span data-stu-id="aaa46-115">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="aaa46-116">使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="aaa46-116">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="aaa46-117">属性</span><span class="sxs-lookup"><span data-stu-id="aaa46-117">Properties</span></span>
| <span data-ttu-id="aaa46-118">属性</span><span class="sxs-lookup"><span data-stu-id="aaa46-118">Property</span></span>     | <span data-ttu-id="aaa46-119">类型</span><span class="sxs-lookup"><span data-stu-id="aaa46-119">Type</span></span>   |<span data-ttu-id="aaa46-120">说明</span><span class="sxs-lookup"><span data-stu-id="aaa46-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aaa46-121">id</span><span class="sxs-lookup"><span data-stu-id="aaa46-121">id</span></span>|<span data-ttu-id="aaa46-122">string</span><span class="sxs-lookup"><span data-stu-id="aaa46-122">string</span></span>|<span data-ttu-id="aaa46-p101">用于标识属性的属性 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="aaa46-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="aaa46-125">value</span><span class="sxs-lookup"><span data-stu-id="aaa46-125">value</span></span>|<span data-ttu-id="aaa46-126">string</span><span class="sxs-lookup"><span data-stu-id="aaa46-126">string</span></span>|<span data-ttu-id="aaa46-127">属性值。</span><span class="sxs-lookup"><span data-stu-id="aaa46-127">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaa46-128">关系</span><span class="sxs-lookup"><span data-stu-id="aaa46-128">Relationships</span></span>
<span data-ttu-id="aaa46-129">无</span><span class="sxs-lookup"><span data-stu-id="aaa46-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="aaa46-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aaa46-130">JSON representation</span></span>

<span data-ttu-id="aaa46-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aaa46-131">Here is a JSON representation of the resource.</span></span>

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

