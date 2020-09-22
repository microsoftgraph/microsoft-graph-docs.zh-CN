---
title: visualInfo 资源类型
description: 一个代表 activity 对象中的 **visualElements** 属性的复杂类型。
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ailae
ms.openlocfilehash: e6bc7bb02ccfc077f9461e5c2a4f15aac4ddf22d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078219"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="79848-103">visualInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="79848-103">visualInfo resource type</span></span>

<span data-ttu-id="79848-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79848-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79848-105">一个代表[activity](../resources/projectrome-activity.md)对象中的**visualElements**属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="79848-105">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="79848-106">每个用户活动将在时间轴中显示为一个自适应卡片。</span><span class="sxs-lookup"><span data-stu-id="79848-106">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="79848-107">鼓励应用程序开发人员提供自定义卡片，以捕获应用程序中发生的活动的实质。</span><span class="sxs-lookup"><span data-stu-id="79848-107">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="79848-108">可通过在 content 属性中提供自定义 JSON 卡片来实现这一点。</span><span class="sxs-lookup"><span data-stu-id="79848-108">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="79848-109">除了具有自适应卡片的可视元数据之外，应用还可以指定内容元数据–用于在用户活动上建立推断的数据，以便为将来的重新约定提供新活动。</span><span class="sxs-lookup"><span data-stu-id="79848-109">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="79848-110">为此，可以使用活动的 contentInfo 属性提供一个 JSON 对象，该对象利用 schema.org 属性来描述内容。</span><span class="sxs-lookup"><span data-stu-id="79848-110">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="79848-111">如果未提供自定义卡片，将使用 "文本" 和 "说明" 属性生成一个简单的卡片。</span><span class="sxs-lookup"><span data-stu-id="79848-111">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="79848-112">建议使用自定义卡片展示应用程序中的最佳内容。</span><span class="sxs-lookup"><span data-stu-id="79848-112">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="79848-113">属性</span><span class="sxs-lookup"><span data-stu-id="79848-113">Properties</span></span>

|<span data-ttu-id="79848-114">名称</span><span class="sxs-lookup"><span data-stu-id="79848-114">Name</span></span> | <span data-ttu-id="79848-115">类型</span><span class="sxs-lookup"><span data-stu-id="79848-115">Type</span></span> | <span data-ttu-id="79848-116">说明</span><span class="sxs-lookup"><span data-stu-id="79848-116">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="79848-117">displayText</span><span class="sxs-lookup"><span data-stu-id="79848-117">displayText</span></span> | <span data-ttu-id="79848-118">String</span><span class="sxs-lookup"><span data-stu-id="79848-118">String</span></span> | <span data-ttu-id="79848-119">必需。</span><span class="sxs-lookup"><span data-stu-id="79848-119">Required.</span></span> <span data-ttu-id="79848-120">用户独特活动的简短文本说明 (例如，当活动引用文档创建时的文档名称) </span><span class="sxs-lookup"><span data-stu-id="79848-120">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="79848-121">说明</span><span class="sxs-lookup"><span data-stu-id="79848-121">description</span></span> | <span data-ttu-id="79848-122">String</span><span class="sxs-lookup"><span data-stu-id="79848-122">String</span></span> | <span data-ttu-id="79848-123">可选。</span><span class="sxs-lookup"><span data-stu-id="79848-123">Optional.</span></span> <span data-ttu-id="79848-124">用户独特活动的更长文本说明 (示例：文档名称、第一句和/或元数据) </span><span class="sxs-lookup"><span data-stu-id="79848-124">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="79848-125">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="79848-125">backgroundColor</span></span> | <span data-ttu-id="79848-126">String</span><span class="sxs-lookup"><span data-stu-id="79848-126">String</span></span> | <span data-ttu-id="79848-127">可选。</span><span class="sxs-lookup"><span data-stu-id="79848-127">Optional.</span></span> <span data-ttu-id="79848-128">用于呈现活动的应用程序源的 UI 品牌颜色中的活动的背景色。</span><span class="sxs-lookup"><span data-stu-id="79848-128">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="79848-129">必须是有效的十六进制颜色</span><span class="sxs-lookup"><span data-stu-id="79848-129">Must be a valid hex color</span></span>|
|<span data-ttu-id="79848-130">content</span><span class="sxs-lookup"><span data-stu-id="79848-130">content</span></span> | <span data-ttu-id="79848-131">非类型化 JSON 对象</span><span class="sxs-lookup"><span data-stu-id="79848-131">Untyped JSON object</span></span> | <span data-ttu-id="79848-132">可选。</span><span class="sxs-lookup"><span data-stu-id="79848-132">Optional.</span></span> <span data-ttu-id="79848-133">用于提供自定义内容以在 Windows Shell UI 中呈现活动的自定义数据 JSON 对象块</span><span class="sxs-lookup"><span data-stu-id="79848-133">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="79848-134">attribution</span><span class="sxs-lookup"><span data-stu-id="79848-134">attribution</span></span> | [<span data-ttu-id="79848-135">imageInfo</span><span class="sxs-lookup"><span data-stu-id="79848-135">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="79848-136">可选。</span><span class="sxs-lookup"><span data-stu-id="79848-136">Optional.</span></span> <span data-ttu-id="79848-137">JSON 对象，用于表示表示用于生成活动的应用程序的图标</span><span class="sxs-lookup"><span data-stu-id="79848-137">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79848-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79848-138">JSON Representation</span></span>

<span data-ttu-id="79848-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79848-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@data.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@data.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


