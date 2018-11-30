---
title: multiValueLegacyExtendedProperty 资源类型
description: 包含值集合的扩展属性。
ms.openlocfilehash: efb871594028b5c2d54b1c081f901717b754c8ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045358"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="1a7d7-103">multiValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a7d7-103">multiValueLegacyExtendedProperty resource type</span></span>

> <span data-ttu-id="1a7d7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a7d7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a7d7-106">包含值集合的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-106">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="1a7d7-107">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-107">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="1a7d7-108">方法</span><span class="sxs-lookup"><span data-stu-id="1a7d7-108">Methods</span></span>

| <span data-ttu-id="1a7d7-109">方法</span><span class="sxs-lookup"><span data-stu-id="1a7d7-109">Method</span></span>           | <span data-ttu-id="1a7d7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1a7d7-110">Return Type</span></span>    |<span data-ttu-id="1a7d7-111">说明</span><span class="sxs-lookup"><span data-stu-id="1a7d7-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a7d7-112">Post</span><span class="sxs-lookup"><span data-stu-id="1a7d7-112">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="1a7d7-113">支持的资源实例：[消息](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系人](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook 任务](../resources/outlooktask.md)或[Outlook 任务文件夹](../resources/outlooktaskfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-113">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="1a7d7-114">请注意，不支持[发布](../resources/post.md)的组。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-114">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="1a7d7-115">在新建或现有的支持资源实例中创建 **multiValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-115">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="1a7d7-116">Get</span><span class="sxs-lookup"><span data-stu-id="1a7d7-116">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="1a7d7-117">展开[为支持的资源实例 （[消息](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系人](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook 任务](../resources/outlooktask.md)、 [Outlook 任务文件夹](../resources/outlooktaskfolder.md)或组[发布](../resources/post.md)）multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-117">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="1a7d7-118">使用 `$expand` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-118">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a7d7-119">属性</span><span class="sxs-lookup"><span data-stu-id="1a7d7-119">Properties</span></span>
| <span data-ttu-id="1a7d7-120">属性</span><span class="sxs-lookup"><span data-stu-id="1a7d7-120">Property</span></span>     | <span data-ttu-id="1a7d7-121">类型</span><span class="sxs-lookup"><span data-stu-id="1a7d7-121">Type</span></span>   |<span data-ttu-id="1a7d7-122">说明</span><span class="sxs-lookup"><span data-stu-id="1a7d7-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a7d7-123">ID</span><span class="sxs-lookup"><span data-stu-id="1a7d7-123">id</span></span>|<span data-ttu-id="1a7d7-124">string</span><span class="sxs-lookup"><span data-stu-id="1a7d7-124">string</span></span>|<span data-ttu-id="1a7d7-p103">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-p103">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="1a7d7-127">value</span><span class="sxs-lookup"><span data-stu-id="1a7d7-127">value</span></span>|<span data-ttu-id="1a7d7-128">string collection</span><span class="sxs-lookup"><span data-stu-id="1a7d7-128">string collection</span></span>|<span data-ttu-id="1a7d7-129">属性值的集合。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-129">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a7d7-130">Relationships</span><span class="sxs-lookup"><span data-stu-id="1a7d7-130">Relationships</span></span>
<span data-ttu-id="1a7d7-131">无</span><span class="sxs-lookup"><span data-stu-id="1a7d7-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1a7d7-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a7d7-132">JSON representation</span></span>

<span data-ttu-id="1a7d7-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a7d7-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.multivaluelegacyextendedproperty"
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