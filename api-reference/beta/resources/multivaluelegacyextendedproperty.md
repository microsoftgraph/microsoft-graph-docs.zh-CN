---
title: multiValueLegacyExtendedProperty 资源类型
description: 包含值集合的扩展属性。
localization_priority: Normal
ms.openlocfilehash: de77f94076fe6bb2f0aa3ded3b1839b8d25ce752
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575889"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="a6117-103">multiValueLegacyExtendedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6117-103">multiValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6117-104">包含值集合的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="a6117-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="a6117-105">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="a6117-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="a6117-106">方法</span><span class="sxs-lookup"><span data-stu-id="a6117-106">Methods</span></span>

| <span data-ttu-id="a6117-107">方法</span><span class="sxs-lookup"><span data-stu-id="a6117-107">Method</span></span>           | <span data-ttu-id="a6117-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a6117-108">Return Type</span></span>    |<span data-ttu-id="a6117-109">说明</span><span class="sxs-lookup"><span data-stu-id="a6117-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6117-110">Post</span><span class="sxs-lookup"><span data-stu-id="a6117-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="a6117-111">支持的资源实例：[消息](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系人](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook 任务](../resources/outlooktask.md)或[Outlook 任务文件夹](../resources/outlooktaskfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="a6117-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="a6117-112">请注意，不支持[发布](../resources/post.md)的组。</span><span class="sxs-lookup"><span data-stu-id="a6117-112">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="a6117-113">在新建或现有的支持资源实例中创建 **multiValueLegacyExtendedProperty**。</span><span class="sxs-lookup"><span data-stu-id="a6117-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="a6117-114">Get</span><span class="sxs-lookup"><span data-stu-id="a6117-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="a6117-115">展开[为支持的资源实例 （[消息](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[事件](../resources/event.md)、[日历](../resources/calendar.md)、[联系人](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook 任务](../resources/outlooktask.md)、 [Outlook 任务文件夹](../resources/outlooktaskfolder.md)或组[发布](../resources/post.md)）multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a6117-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="a6117-116">使用 `$expand` 获取具有扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="a6117-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6117-117">属性</span><span class="sxs-lookup"><span data-stu-id="a6117-117">Properties</span></span>
| <span data-ttu-id="a6117-118">属性</span><span class="sxs-lookup"><span data-stu-id="a6117-118">Property</span></span>     | <span data-ttu-id="a6117-119">类型</span><span class="sxs-lookup"><span data-stu-id="a6117-119">Type</span></span>   |<span data-ttu-id="a6117-120">说明</span><span class="sxs-lookup"><span data-stu-id="a6117-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6117-121">id</span><span class="sxs-lookup"><span data-stu-id="a6117-121">id</span></span>|<span data-ttu-id="a6117-122">string</span><span class="sxs-lookup"><span data-stu-id="a6117-122">string</span></span>|<span data-ttu-id="a6117-p102">属性标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="a6117-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="a6117-125">value</span><span class="sxs-lookup"><span data-stu-id="a6117-125">value</span></span>|<span data-ttu-id="a6117-126">字符串集合</span><span class="sxs-lookup"><span data-stu-id="a6117-126">string collection</span></span>|<span data-ttu-id="a6117-127">属性值的集合。</span><span class="sxs-lookup"><span data-stu-id="a6117-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6117-128">关系</span><span class="sxs-lookup"><span data-stu-id="a6117-128">Relationships</span></span>
<span data-ttu-id="a6117-129">无</span><span class="sxs-lookup"><span data-stu-id="a6117-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a6117-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6117-130">JSON representation</span></span>

<span data-ttu-id="a6117-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6117-131">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/multivaluelegacyextendedproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
