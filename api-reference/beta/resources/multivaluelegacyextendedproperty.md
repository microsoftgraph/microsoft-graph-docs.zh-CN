---
title: multiValueLegacyExtendedProperty 资源类型
description: 包含值集合的扩展属性。
localization_priority: Normal
ms.openlocfilehash: 4a30f8cf2a77e43db028c069fc36dc5cd8f360a3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342182"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="f3273-103">multiValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3273-103">multiValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3273-104">包含值集合的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f3273-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="f3273-105">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="f3273-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="f3273-106">方法</span><span class="sxs-lookup"><span data-stu-id="f3273-106">Methods</span></span>

| <span data-ttu-id="f3273-107">方法</span><span class="sxs-lookup"><span data-stu-id="f3273-107">Method</span></span>           | <span data-ttu-id="f3273-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f3273-108">Return Type</span></span>    |<span data-ttu-id="f3273-109">说明</span><span class="sxs-lookup"><span data-stu-id="f3273-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f3273-110">Post</span><span class="sxs-lookup"><span data-stu-id="f3273-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="f3273-111">受支持的资源实例[: message](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [outlook task](../resources/outlooktask.md)或[Outlook 任务文件夹](../resources/outlooktaskfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="f3273-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="f3273-112">请注意，不支持 [post](../resources/post.md) 组。</span><span class="sxs-lookup"><span data-stu-id="f3273-112">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="f3273-113">在新建或现有的支持资源实例中创建 **multiValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="f3273-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="f3273-114">获取</span><span class="sxs-lookup"><span data-stu-id="f3273-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="f3273-115">扩展[](../resources/mailfolder.md) [](../resources/event.md)[](../resources/message.md) [](../resources/contactfolder.md) [](../resources/post.md) [](../resources/calendar.md) [](../resources/contact.md) [](../resources/outlooktask.md) [](../resources/outlooktaskfolder.md)了受支持的资源实例 (message、mailFolder、event、calendar、contact、contactFolder、outlook task、outlook task 文件夹或 group post) [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f3273-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="f3273-116">使用 `$expand` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="f3273-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3273-117">属性</span><span class="sxs-lookup"><span data-stu-id="f3273-117">Properties</span></span>
| <span data-ttu-id="f3273-118">属性</span><span class="sxs-lookup"><span data-stu-id="f3273-118">Property</span></span>     | <span data-ttu-id="f3273-119">类型</span><span class="sxs-lookup"><span data-stu-id="f3273-119">Type</span></span>   |<span data-ttu-id="f3273-120">说明</span><span class="sxs-lookup"><span data-stu-id="f3273-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3273-121">id</span><span class="sxs-lookup"><span data-stu-id="f3273-121">id</span></span>|<span data-ttu-id="f3273-122">string</span><span class="sxs-lookup"><span data-stu-id="f3273-122">string</span></span>|<span data-ttu-id="f3273-p102">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="f3273-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="f3273-125">value</span><span class="sxs-lookup"><span data-stu-id="f3273-125">value</span></span>|<span data-ttu-id="f3273-126">string collection</span><span class="sxs-lookup"><span data-stu-id="f3273-126">string collection</span></span>|<span data-ttu-id="f3273-127">属性值的集合。</span><span class="sxs-lookup"><span data-stu-id="f3273-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3273-128">关系</span><span class="sxs-lookup"><span data-stu-id="f3273-128">Relationships</span></span>
<span data-ttu-id="f3273-129">无</span><span class="sxs-lookup"><span data-stu-id="f3273-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f3273-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3273-130">JSON representation</span></span>

<span data-ttu-id="f3273-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3273-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
