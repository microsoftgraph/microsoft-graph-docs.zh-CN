---
title: multiValueLegacyExtendedProperty 资源类型
description: 包含值集合的扩展属性。
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4d6139259616c6d347387b515f16e4b9ef5e4ddf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131521"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="084e7-103">multiValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="084e7-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="084e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="084e7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="084e7-105">包含值集合的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="084e7-105">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="084e7-106">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="084e7-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="084e7-107">Methods</span><span class="sxs-lookup"><span data-stu-id="084e7-107">Methods</span></span>

| <span data-ttu-id="084e7-108">方法</span><span class="sxs-lookup"><span data-stu-id="084e7-108">Method</span></span>           | <span data-ttu-id="084e7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="084e7-109">Return Type</span></span>    |<span data-ttu-id="084e7-110">说明</span><span class="sxs-lookup"><span data-stu-id="084e7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="084e7-111">Post</span><span class="sxs-lookup"><span data-stu-id="084e7-111">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="084e7-p101">受支持的资源实例有：[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md) 或 [contactFolder](../resources/contactfolder.md)。请注意，不支持 [post](../resources/post.md) 组。</span><span class="sxs-lookup"><span data-stu-id="084e7-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="084e7-114">在新建或现有的支持资源实例中创建 **multiValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="084e7-114">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="084e7-115">获取</span><span class="sxs-lookup"><span data-stu-id="084e7-115">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="084e7-116">通过 [multiValueLegacyExtendedProperty](../resources/message.md) 对象扩展的受支持的资源实例（[message](../resources/mailfolder.md)、[mailFolder](../resources/event.md)、[event](../resources/calendar.md)、[calendar](../resources/contact.md)、[contact](../resources/contactfolder.md)、[contactFolder](../resources/post.md) 或 [post](multivaluelegacyextendedproperty.md) 组）。</span><span class="sxs-lookup"><span data-stu-id="084e7-116">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="084e7-117">使用 `$expand` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="084e7-117">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="084e7-118">属性</span><span class="sxs-lookup"><span data-stu-id="084e7-118">Properties</span></span>
| <span data-ttu-id="084e7-119">属性</span><span class="sxs-lookup"><span data-stu-id="084e7-119">Property</span></span>     | <span data-ttu-id="084e7-120">类型</span><span class="sxs-lookup"><span data-stu-id="084e7-120">Type</span></span>   |<span data-ttu-id="084e7-121">说明</span><span class="sxs-lookup"><span data-stu-id="084e7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="084e7-122">id</span><span class="sxs-lookup"><span data-stu-id="084e7-122">id</span></span>|<span data-ttu-id="084e7-123">string</span><span class="sxs-lookup"><span data-stu-id="084e7-123">string</span></span>|<span data-ttu-id="084e7-p102">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="084e7-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="084e7-126">value</span><span class="sxs-lookup"><span data-stu-id="084e7-126">value</span></span>|<span data-ttu-id="084e7-127">string collection</span><span class="sxs-lookup"><span data-stu-id="084e7-127">string collection</span></span>|<span data-ttu-id="084e7-128">属性值的集合。</span><span class="sxs-lookup"><span data-stu-id="084e7-128">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="084e7-129">关系</span><span class="sxs-lookup"><span data-stu-id="084e7-129">Relationships</span></span>
<span data-ttu-id="084e7-130">无</span><span class="sxs-lookup"><span data-stu-id="084e7-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="084e7-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="084e7-131">JSON representation</span></span>

<span data-ttu-id="084e7-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="084e7-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

