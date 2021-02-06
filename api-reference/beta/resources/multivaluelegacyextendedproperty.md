---
title: multiValueLegacyExtendedProperty 资源类型
description: 包含值集合的扩展属性。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: a8752fa866478eff57124f486e958388fa7603a1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131927"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="122e7-103">multiValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="122e7-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="122e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="122e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="122e7-105">包含值集合的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="122e7-105">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="122e7-106">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="122e7-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="122e7-107">方法</span><span class="sxs-lookup"><span data-stu-id="122e7-107">Methods</span></span>

| <span data-ttu-id="122e7-108">方法</span><span class="sxs-lookup"><span data-stu-id="122e7-108">Method</span></span>           | <span data-ttu-id="122e7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="122e7-109">Return Type</span></span>    |<span data-ttu-id="122e7-110">说明</span><span class="sxs-lookup"><span data-stu-id="122e7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="122e7-111">Post</span><span class="sxs-lookup"><span data-stu-id="122e7-111">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="122e7-112">受支持的资源实例：[邮件](../resources/message.md)[、mailFolder、](../resources/mailfolder.md)[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系人](../resources/contact.md)[、contactFolder、Outlook](../resources/contactfolder.md)[任务](../resources/outlooktask.md)或[Outlook 任务文件夹](../resources/outlooktaskfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="122e7-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="122e7-113">请注意，不支持 [post](../resources/post.md) 组。</span><span class="sxs-lookup"><span data-stu-id="122e7-113">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="122e7-114">在新建或现有的支持资源实例中创建 **multiValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="122e7-114">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="122e7-115">获取</span><span class="sxs-lookup"><span data-stu-id="122e7-115">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="122e7-116">受支持的资源实例 ([邮件](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、 日历[、](../resources/calendar.md)[联系人](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook 任务](../resources/outlooktask.md)、 [Outlook](../resources/outlooktaskfolder.md)任务文件夹或组帖子[) ](../resources/post.md)使用[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)对象扩展。</span><span class="sxs-lookup"><span data-stu-id="122e7-116">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="122e7-117">使用 `$expand` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="122e7-117">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="122e7-118">属性</span><span class="sxs-lookup"><span data-stu-id="122e7-118">Properties</span></span>
| <span data-ttu-id="122e7-119">属性</span><span class="sxs-lookup"><span data-stu-id="122e7-119">Property</span></span>     | <span data-ttu-id="122e7-120">类型</span><span class="sxs-lookup"><span data-stu-id="122e7-120">Type</span></span>   |<span data-ttu-id="122e7-121">说明</span><span class="sxs-lookup"><span data-stu-id="122e7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="122e7-122">id</span><span class="sxs-lookup"><span data-stu-id="122e7-122">id</span></span>|<span data-ttu-id="122e7-123">string</span><span class="sxs-lookup"><span data-stu-id="122e7-123">string</span></span>|<span data-ttu-id="122e7-p102">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="122e7-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="122e7-126">value</span><span class="sxs-lookup"><span data-stu-id="122e7-126">value</span></span>|<span data-ttu-id="122e7-127">string collection</span><span class="sxs-lookup"><span data-stu-id="122e7-127">string collection</span></span>|<span data-ttu-id="122e7-128">属性值的集合。</span><span class="sxs-lookup"><span data-stu-id="122e7-128">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="122e7-129">关系</span><span class="sxs-lookup"><span data-stu-id="122e7-129">Relationships</span></span>
<span data-ttu-id="122e7-130">无</span><span class="sxs-lookup"><span data-stu-id="122e7-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="122e7-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="122e7-131">JSON representation</span></span>

<span data-ttu-id="122e7-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="122e7-132">Here is a JSON representation of the resource.</span></span>

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


