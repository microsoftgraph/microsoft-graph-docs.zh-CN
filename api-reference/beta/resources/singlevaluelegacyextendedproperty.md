---
title: singleValueLegacyExtendedProperty 资源类型
description: '包含单个值的扩展属性。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 578b2792a815dd0c7cd5dad4fc77d9c96319045a
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334582"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="919bc-103">singleValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="919bc-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="919bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="919bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="919bc-105">包含单个值的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="919bc-105">An extended property that contains a single value.</span></span>

<span data-ttu-id="919bc-106">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="919bc-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>


## <a name="methods"></a><span data-ttu-id="919bc-107">方法</span><span class="sxs-lookup"><span data-stu-id="919bc-107">Methods</span></span>

| <span data-ttu-id="919bc-108">方法</span><span class="sxs-lookup"><span data-stu-id="919bc-108">Method</span></span>           | <span data-ttu-id="919bc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="919bc-109">Return Type</span></span>    |<span data-ttu-id="919bc-110">说明</span><span class="sxs-lookup"><span data-stu-id="919bc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="919bc-111">Post</span><span class="sxs-lookup"><span data-stu-id="919bc-111">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="919bc-112">[](../resources/post.md)受支持的资源实例：message、mailFolder、event、calendar、contact、contactFolder、Outlook [](../resources/event.md) [](../resources/mailfolder.md) [task](../resources/outlooktask.md)或 Outlook [task folder](../resources/outlooktaskfolder.md)，但不是组 post 。 [](../resources/message.md) [](../resources/calendar.md) [](../resources/contact.md) [](../resources/contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="919bc-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="919bc-113">在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="919bc-113">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="919bc-114">获取</span><span class="sxs-lookup"><span data-stu-id="919bc-114">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="919bc-115">支持的资源实例 ([](../resources/message.md)message、mailFolder、event、calendar、contact、contactFolder、Outlook [](../resources/contactfolder.md) [](../resources/contact.md) [](../resources/mailfolder.md) [](../resources/event.md) [task、Outlook](../resources/outlooktask.md) [task folder](../resources/outlooktaskfolder.md)或 group [post](../resources/post.md)) 或一个此类实例（使用[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)对象扩展）的一个或一个集合。 [](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="919bc-115">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="919bc-116">使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="919bc-116">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="919bc-117">属性</span><span class="sxs-lookup"><span data-stu-id="919bc-117">Properties</span></span>
| <span data-ttu-id="919bc-118">属性</span><span class="sxs-lookup"><span data-stu-id="919bc-118">Property</span></span>     | <span data-ttu-id="919bc-119">类型</span><span class="sxs-lookup"><span data-stu-id="919bc-119">Type</span></span>   |<span data-ttu-id="919bc-120">说明</span><span class="sxs-lookup"><span data-stu-id="919bc-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="919bc-121">id</span><span class="sxs-lookup"><span data-stu-id="919bc-121">id</span></span>|<span data-ttu-id="919bc-122">string</span><span class="sxs-lookup"><span data-stu-id="919bc-122">string</span></span>|<span data-ttu-id="919bc-p101">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="919bc-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="919bc-125">value</span><span class="sxs-lookup"><span data-stu-id="919bc-125">value</span></span>|<span data-ttu-id="919bc-126">string</span><span class="sxs-lookup"><span data-stu-id="919bc-126">string</span></span>|<span data-ttu-id="919bc-127">属性值。</span><span class="sxs-lookup"><span data-stu-id="919bc-127">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="919bc-128">关系</span><span class="sxs-lookup"><span data-stu-id="919bc-128">Relationships</span></span>
<span data-ttu-id="919bc-129">无</span><span class="sxs-lookup"><span data-stu-id="919bc-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="919bc-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="919bc-130">JSON representation</span></span>

<span data-ttu-id="919bc-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="919bc-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


