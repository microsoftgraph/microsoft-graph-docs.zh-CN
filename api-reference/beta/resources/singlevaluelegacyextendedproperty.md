---
title: singleValueLegacyExtendedProperty 资源类型
description: '包含单个值的扩展属性。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 411cf91d2da986f1b669fe172f30a99c0298840b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520560"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="0b949-103">singleValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b949-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="0b949-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0b949-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b949-105">包含单个值的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="0b949-105">An extended property that contains a single value.</span></span> 

<span data-ttu-id="0b949-106">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="0b949-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="0b949-107">方法</span><span class="sxs-lookup"><span data-stu-id="0b949-107">Methods</span></span>

| <span data-ttu-id="0b949-108">方法</span><span class="sxs-lookup"><span data-stu-id="0b949-108">Method</span></span>           | <span data-ttu-id="0b949-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b949-109">Return Type</span></span>    |<span data-ttu-id="0b949-110">说明</span><span class="sxs-lookup"><span data-stu-id="0b949-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b949-111">Post</span><span class="sxs-lookup"><span data-stu-id="0b949-111">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="0b949-112">受支持的资源实例[： message](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [outlook 任务](../resources/outlooktask.md)或[Outlook 任务文件夹](../resources/outlooktaskfolder.md)，但不能进行组[帖子](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="0b949-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="0b949-113">在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="0b949-113">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="0b949-114">获取</span><span class="sxs-lookup"><span data-stu-id="0b949-114">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="0b949-115">一个或一组受支持的资源实例[（message](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook 任务](../resources/outlooktask.md)、 [outlook 任务文件夹](../resources/outlooktaskfolder.md)或组[post](../resources/post.md)），或使用[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)对象扩展的一个此类实例。</span><span class="sxs-lookup"><span data-stu-id="0b949-115">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="0b949-116">使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="0b949-116">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b949-117">属性</span><span class="sxs-lookup"><span data-stu-id="0b949-117">Properties</span></span>
| <span data-ttu-id="0b949-118">属性</span><span class="sxs-lookup"><span data-stu-id="0b949-118">Property</span></span>     | <span data-ttu-id="0b949-119">类型</span><span class="sxs-lookup"><span data-stu-id="0b949-119">Type</span></span>   |<span data-ttu-id="0b949-120">说明</span><span class="sxs-lookup"><span data-stu-id="0b949-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b949-121">id</span><span class="sxs-lookup"><span data-stu-id="0b949-121">id</span></span>|<span data-ttu-id="0b949-122">string</span><span class="sxs-lookup"><span data-stu-id="0b949-122">string</span></span>|<span data-ttu-id="0b949-p101">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="0b949-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="0b949-125">value</span><span class="sxs-lookup"><span data-stu-id="0b949-125">value</span></span>|<span data-ttu-id="0b949-126">string</span><span class="sxs-lookup"><span data-stu-id="0b949-126">string</span></span>|<span data-ttu-id="0b949-127">属性值。</span><span class="sxs-lookup"><span data-stu-id="0b949-127">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b949-128">关系</span><span class="sxs-lookup"><span data-stu-id="0b949-128">Relationships</span></span>
<span data-ttu-id="0b949-129">无</span><span class="sxs-lookup"><span data-stu-id="0b949-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0b949-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b949-130">JSON representation</span></span>

<span data-ttu-id="0b949-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b949-131">Here is a JSON representation of the resource.</span></span>

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
