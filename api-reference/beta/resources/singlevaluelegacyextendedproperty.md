---
title: singleValueLegacyExtendedProperty 资源类型
description: '包含单个值的扩展属性。 '
localization_priority: Normal
ms.openlocfilehash: e57091e9ccf525fc10754dab7de464f2ebf7662c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343046"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="2615f-103">singleValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="2615f-103">singleValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2615f-104">包含单个值的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="2615f-104">An extended property that contains a single value.</span></span> 

<span data-ttu-id="2615f-105">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="2615f-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="2615f-106">方法</span><span class="sxs-lookup"><span data-stu-id="2615f-106">Methods</span></span>

| <span data-ttu-id="2615f-107">方法</span><span class="sxs-lookup"><span data-stu-id="2615f-107">Method</span></span>           | <span data-ttu-id="2615f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2615f-108">Return Type</span></span>    |<span data-ttu-id="2615f-109">说明</span><span class="sxs-lookup"><span data-stu-id="2615f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2615f-110">Post</span><span class="sxs-lookup"><span data-stu-id="2615f-110">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="2615f-111">受支持的资源实例[: message](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [outlook 任务](../resources/outlooktask.md)或[Outlook 任务文件夹](../resources/outlooktaskfolder.md), 但不能进行组[帖子](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="2615f-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="2615f-112">在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="2615f-112">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="2615f-113">获取</span><span class="sxs-lookup"><span data-stu-id="2615f-113">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="2615f-114">一个或一组受支持的资源实例[(message](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [outlook task](../resources/outlooktask.md)、 [outlook task folder](../resources/outlooktaskfolder.md)或 group [post](../resources/post.md))或使用[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)对象扩展的一个此类实例。</span><span class="sxs-lookup"><span data-stu-id="2615f-114">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="2615f-115">使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="2615f-115">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="2615f-116">属性</span><span class="sxs-lookup"><span data-stu-id="2615f-116">Properties</span></span>
| <span data-ttu-id="2615f-117">属性</span><span class="sxs-lookup"><span data-stu-id="2615f-117">Property</span></span>     | <span data-ttu-id="2615f-118">类型</span><span class="sxs-lookup"><span data-stu-id="2615f-118">Type</span></span>   |<span data-ttu-id="2615f-119">说明</span><span class="sxs-lookup"><span data-stu-id="2615f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2615f-120">id</span><span class="sxs-lookup"><span data-stu-id="2615f-120">id</span></span>|<span data-ttu-id="2615f-121">string</span><span class="sxs-lookup"><span data-stu-id="2615f-121">string</span></span>|<span data-ttu-id="2615f-p101">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="2615f-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="2615f-124">value</span><span class="sxs-lookup"><span data-stu-id="2615f-124">value</span></span>|<span data-ttu-id="2615f-125">string</span><span class="sxs-lookup"><span data-stu-id="2615f-125">string</span></span>|<span data-ttu-id="2615f-126">属性值。</span><span class="sxs-lookup"><span data-stu-id="2615f-126">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2615f-127">关系</span><span class="sxs-lookup"><span data-stu-id="2615f-127">Relationships</span></span>
<span data-ttu-id="2615f-128">无</span><span class="sxs-lookup"><span data-stu-id="2615f-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2615f-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2615f-129">JSON representation</span></span>

<span data-ttu-id="2615f-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2615f-130">Here is a JSON representation of the resource.</span></span>

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
