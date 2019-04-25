---
title: multiValueLegacyExtendedProperty 资源类型
description: 包含值集合的扩展属性。
localization_priority: Normal
ms.openlocfilehash: 87823559bad3e149ef3c4d4d6f21f43cf66c41fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580266"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="d2f7d-103">multiValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2f7d-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="d2f7d-104">包含值集合的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d2f7d-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="d2f7d-105">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="d2f7d-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="d2f7d-106">方法</span><span class="sxs-lookup"><span data-stu-id="d2f7d-106">Methods</span></span>

| <span data-ttu-id="d2f7d-107">方法</span><span class="sxs-lookup"><span data-stu-id="d2f7d-107">Method</span></span>           | <span data-ttu-id="d2f7d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2f7d-108">Return Type</span></span>    |<span data-ttu-id="d2f7d-109">说明</span><span class="sxs-lookup"><span data-stu-id="d2f7d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2f7d-110">帖子</span><span class="sxs-lookup"><span data-stu-id="d2f7d-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="d2f7d-p101">受支持的资源实例有：[message](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[event](../resources/event.md)、[calendar](../resources/calendar.md)、[contact](../resources/contact.md) 或 [contactFolder](../resources/contactfolder.md)。请注意，不支持 [post](../resources/post.md) 组。</span><span class="sxs-lookup"><span data-stu-id="d2f7d-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="d2f7d-113">在新建或现有的支持资源实例中创建 **multiValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="d2f7d-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="d2f7d-114">获取</span><span class="sxs-lookup"><span data-stu-id="d2f7d-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="d2f7d-115">通过 [multiValueLegacyExtendedProperty](../resources/message.md) 对象扩展的受支持的资源实例（[message](../resources/mailfolder.md)、[mailFolder](../resources/event.md)、[event](../resources/calendar.md)、[calendar](../resources/contact.md)、[contact](../resources/contactfolder.md)、[contactFolder](../resources/post.md) 或 [post](multivaluelegacyextendedproperty.md) 组）。</span><span class="sxs-lookup"><span data-stu-id="d2f7d-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="d2f7d-116">使用 `$expand` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="d2f7d-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2f7d-117">属性</span><span class="sxs-lookup"><span data-stu-id="d2f7d-117">Properties</span></span>
| <span data-ttu-id="d2f7d-118">属性</span><span class="sxs-lookup"><span data-stu-id="d2f7d-118">Property</span></span>     | <span data-ttu-id="d2f7d-119">类型</span><span class="sxs-lookup"><span data-stu-id="d2f7d-119">Type</span></span>   |<span data-ttu-id="d2f7d-120">说明</span><span class="sxs-lookup"><span data-stu-id="d2f7d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2f7d-121">id</span><span class="sxs-lookup"><span data-stu-id="d2f7d-121">id</span></span>|<span data-ttu-id="d2f7d-122">string</span><span class="sxs-lookup"><span data-stu-id="d2f7d-122">string</span></span>|<span data-ttu-id="d2f7d-p102">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d2f7d-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="d2f7d-125">value</span><span class="sxs-lookup"><span data-stu-id="d2f7d-125">value</span></span>|<span data-ttu-id="d2f7d-126">string collection</span><span class="sxs-lookup"><span data-stu-id="d2f7d-126">string collection</span></span>|<span data-ttu-id="d2f7d-127">属性值的集合。</span><span class="sxs-lookup"><span data-stu-id="d2f7d-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2f7d-128">关系</span><span class="sxs-lookup"><span data-stu-id="d2f7d-128">Relationships</span></span>
<span data-ttu-id="d2f7d-129">无</span><span class="sxs-lookup"><span data-stu-id="d2f7d-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d2f7d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2f7d-130">JSON representation</span></span>

<span data-ttu-id="d2f7d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2f7d-131">Here is a JSON representation of the resource.</span></span>

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
