---
title: singleValueLegacyExtendedProperty 资源类型
description: '包含单个值的扩展属性。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 41857d57010265d7942e0d1694191ee5acf3c4d1
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849742"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="91d0e-103">singleValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="91d0e-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="91d0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91d0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="91d0e-105">包含单个值的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="91d0e-105">An extended property that contains a single value.</span></span>

<span data-ttu-id="91d0e-106">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="91d0e-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>


## <a name="methods"></a><span data-ttu-id="91d0e-107">方法</span><span class="sxs-lookup"><span data-stu-id="91d0e-107">Methods</span></span>

| <span data-ttu-id="91d0e-108">方法</span><span class="sxs-lookup"><span data-stu-id="91d0e-108">Method</span></span>           | <span data-ttu-id="91d0e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="91d0e-109">Return Type</span></span>    |<span data-ttu-id="91d0e-110">说明</span><span class="sxs-lookup"><span data-stu-id="91d0e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91d0e-111">Post</span><span class="sxs-lookup"><span data-stu-id="91d0e-111">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="91d0e-112">支持的资源实例 [：message](../resources/message.md) [、mailFolder](../resources/mailfolder.md) [、event](../resources/event.md) [、calendar](../resources/calendar.md) [、contact](../resources/contact.md) [、contactFolder](../resources/contactfolder.md) [、Outlook 任务](../resources/outlooktask.md)或 [Outlook 任务文件夹，](../resources/outlooktaskfolder.md)但不能对组帖 [子进行分组](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="91d0e-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="91d0e-113">在新建或现有的支持资源实例中创建 **singleValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="91d0e-113">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="91d0e-114">获取</span><span class="sxs-lookup"><span data-stu-id="91d0e-114">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="91d0e-115">受支持的资源实例之一 ([邮件、mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系人](../resources/contact.md)[、contactFolder](../resources/contactfolder.md) [、Outlook 任务](../resources/outlooktask.md)[、Outlook 任务](../resources/outlooktaskfolder.md)文件夹或组[帖](../resources/post.md)子) 或通过[singleValueLegacyExtendedProperty 对象扩展的一个此类](singlevaluelegacyextendedproperty.md)实例。 [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="91d0e-115">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="91d0e-116">使用 `$expand` 或 `$filter` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="91d0e-116">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="91d0e-117">属性</span><span class="sxs-lookup"><span data-stu-id="91d0e-117">Properties</span></span>
| <span data-ttu-id="91d0e-118">属性</span><span class="sxs-lookup"><span data-stu-id="91d0e-118">Property</span></span>     | <span data-ttu-id="91d0e-119">类型</span><span class="sxs-lookup"><span data-stu-id="91d0e-119">Type</span></span>   |<span data-ttu-id="91d0e-120">说明</span><span class="sxs-lookup"><span data-stu-id="91d0e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91d0e-121">id</span><span class="sxs-lookup"><span data-stu-id="91d0e-121">id</span></span>|<span data-ttu-id="91d0e-122">string</span><span class="sxs-lookup"><span data-stu-id="91d0e-122">string</span></span>|<span data-ttu-id="91d0e-p101">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="91d0e-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="91d0e-125">value</span><span class="sxs-lookup"><span data-stu-id="91d0e-125">value</span></span>|<span data-ttu-id="91d0e-126">string</span><span class="sxs-lookup"><span data-stu-id="91d0e-126">string</span></span>|<span data-ttu-id="91d0e-127">属性值。</span><span class="sxs-lookup"><span data-stu-id="91d0e-127">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91d0e-128">关系</span><span class="sxs-lookup"><span data-stu-id="91d0e-128">Relationships</span></span>
<span data-ttu-id="91d0e-129">无</span><span class="sxs-lookup"><span data-stu-id="91d0e-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="91d0e-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91d0e-130">JSON representation</span></span>

<span data-ttu-id="91d0e-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91d0e-131">Here is a JSON representation of the resource.</span></span>

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
