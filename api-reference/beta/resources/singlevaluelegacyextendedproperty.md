---
title: singleValueLegacyExtendedProperty 资源类型
description: '包含单个值的扩展属性。 '
localization_priority: Normal
ms.openlocfilehash: 51a42661ea3a19ea8e82ba78115bfa5290d99d15
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857412"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="91a84-103">singleValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="91a84-103">singleValueLegacyExtendedProperty resource type</span></span>

> <span data-ttu-id="91a84-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="91a84-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91a84-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="91a84-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91a84-106">包含单个值的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="91a84-106">An extended property that contains a single value.</span></span> 

<span data-ttu-id="91a84-107">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="91a84-107">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="91a84-108">方法</span><span class="sxs-lookup"><span data-stu-id="91a84-108">Methods</span></span>

| <span data-ttu-id="91a84-109">方法</span><span class="sxs-lookup"><span data-stu-id="91a84-109">Method</span></span>           | <span data-ttu-id="91a84-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="91a84-110">Return Type</span></span>    |<span data-ttu-id="91a84-111">说明</span><span class="sxs-lookup"><span data-stu-id="91a84-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91a84-112">Post</span><span class="sxs-lookup"><span data-stu-id="91a84-112">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="91a84-113">支持的资源实例：[消息](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系人](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook 任务](../resources/outlooktask.md)中，或[Outlook 任务文件夹](../resources/outlooktaskfolder.md)，但不是组[发布](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="91a84-113">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="91a84-114">在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="91a84-114">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="91a84-115">获取</span><span class="sxs-lookup"><span data-stu-id="91a84-115">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="91a84-116">一项或者 （[消息](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系人](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook 任务](../resources/outlooktask.md)、 [Outlook 任务文件夹](../resources/outlooktaskfolder.md)或组[发布](../resources/post.md)），支持的资源实例的集合或展开[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)对象为一个此类的实例。</span><span class="sxs-lookup"><span data-stu-id="91a84-116">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="91a84-117">使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="91a84-117">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="91a84-118">属性</span><span class="sxs-lookup"><span data-stu-id="91a84-118">Properties</span></span>
| <span data-ttu-id="91a84-119">属性</span><span class="sxs-lookup"><span data-stu-id="91a84-119">Property</span></span>     | <span data-ttu-id="91a84-120">类型</span><span class="sxs-lookup"><span data-stu-id="91a84-120">Type</span></span>   |<span data-ttu-id="91a84-121">说明</span><span class="sxs-lookup"><span data-stu-id="91a84-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91a84-122">ID</span><span class="sxs-lookup"><span data-stu-id="91a84-122">id</span></span>|<span data-ttu-id="91a84-123">string</span><span class="sxs-lookup"><span data-stu-id="91a84-123">string</span></span>|<span data-ttu-id="91a84-p102">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="91a84-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="91a84-126">value</span><span class="sxs-lookup"><span data-stu-id="91a84-126">value</span></span>|<span data-ttu-id="91a84-127">string</span><span class="sxs-lookup"><span data-stu-id="91a84-127">string</span></span>|<span data-ttu-id="91a84-128">属性值。</span><span class="sxs-lookup"><span data-stu-id="91a84-128">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91a84-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="91a84-129">Relationships</span></span>
<span data-ttu-id="91a84-130">无</span><span class="sxs-lookup"><span data-stu-id="91a84-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="91a84-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91a84-131">JSON representation</span></span>

<span data-ttu-id="91a84-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91a84-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
