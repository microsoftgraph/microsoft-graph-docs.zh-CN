---
title: visualInfo 资源类型
description: 代表活动对象中的**visualElements**属性的复杂类型。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 56d3822c89de074847aeab6c8a0a742ecd7f006f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514920"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="be5ae-103">visualInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="be5ae-103">visualInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be5ae-104">代表[活动](../resources/projectrome-activity.md)对象中的**visualElements**属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="be5ae-104">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="be5ae-105">每个用户活动将在日程表中显示为自适应卡片。</span><span class="sxs-lookup"><span data-stu-id="be5ae-105">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="be5ae-106">鼓励提供用来捕获的活动的应用程序中发生的实质的自定义卡片将应用程序开发人员。</span><span class="sxs-lookup"><span data-stu-id="be5ae-106">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="be5ae-107">这是通过提供内容的属性中的自定义 JSON 卡片。</span><span class="sxs-lookup"><span data-stu-id="be5ae-107">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="be5ae-108">除了具有自适应卡片 visual 元数据，应用程序可指定内容元数据 – 为的数据用于根据用户的活动生成推断才能提供的将来重新新活动。</span><span class="sxs-lookup"><span data-stu-id="be5ae-108">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="be5ae-109">这是通过使用活动的 contentInfo 属性提供一个 JSON 对象，该利用 schema.org 属性来描述内容对象。</span><span class="sxs-lookup"><span data-stu-id="be5ae-109">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="be5ae-110">如果未提供的自定义卡片，则将生成的简单卡片使用显示文本和说明属性。</span><span class="sxs-lookup"><span data-stu-id="be5ae-110">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="be5ae-111">自定义卡建议展示从您的应用程序中的最佳内容。</span><span class="sxs-lookup"><span data-stu-id="be5ae-111">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="be5ae-112">属性</span><span class="sxs-lookup"><span data-stu-id="be5ae-112">Properties</span></span>

|<span data-ttu-id="be5ae-113">名称</span><span class="sxs-lookup"><span data-stu-id="be5ae-113">Name</span></span> | <span data-ttu-id="be5ae-114">类型</span><span class="sxs-lookup"><span data-stu-id="be5ae-114">Type</span></span> | <span data-ttu-id="be5ae-115">说明</span><span class="sxs-lookup"><span data-stu-id="be5ae-115">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="be5ae-116">显示文本</span><span class="sxs-lookup"><span data-stu-id="be5ae-116">displayText</span></span> | <span data-ttu-id="be5ae-117">String</span><span class="sxs-lookup"><span data-stu-id="be5ae-117">String</span></span> | <span data-ttu-id="be5ae-118">必需。</span><span class="sxs-lookup"><span data-stu-id="be5ae-118">Required.</span></span> <span data-ttu-id="be5ae-119">短用户的唯一活动 （例如，在其中活动是指创建文档的情况下的文档名称） 的文本的说明</span><span class="sxs-lookup"><span data-stu-id="be5ae-119">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="be5ae-120">说明</span><span class="sxs-lookup"><span data-stu-id="be5ae-120">description</span></span> | <span data-ttu-id="be5ae-121">字符串</span><span class="sxs-lookup"><span data-stu-id="be5ae-121">String</span></span> | <span data-ttu-id="be5ae-122">可选。</span><span class="sxs-lookup"><span data-stu-id="be5ae-122">Optional.</span></span> <span data-ttu-id="be5ae-123">更长时间的用户的唯一的活动的文本说明 (示例： 文档名称、 第一句和/或元数据)</span><span class="sxs-lookup"><span data-stu-id="be5ae-123">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="be5ae-124">BackgroundColor</span><span class="sxs-lookup"><span data-stu-id="be5ae-124">backgroundColor</span></span> | <span data-ttu-id="be5ae-125">字符串</span><span class="sxs-lookup"><span data-stu-id="be5ae-125">String</span></span> | <span data-ttu-id="be5ae-126">可选。</span><span class="sxs-lookup"><span data-stu-id="be5ae-126">Optional.</span></span> <span data-ttu-id="be5ae-127">用于呈现 UI 的品牌颜色活动的应用程序源中的活动的背景色。</span><span class="sxs-lookup"><span data-stu-id="be5ae-127">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="be5ae-128">必须是有效的十六进制颜色</span><span class="sxs-lookup"><span data-stu-id="be5ae-128">Must be a valid hex color</span></span>|
|<span data-ttu-id="be5ae-129">content</span><span class="sxs-lookup"><span data-stu-id="be5ae-129">content</span></span> | <span data-ttu-id="be5ae-130">类型化的 JSON 对象</span><span class="sxs-lookup"><span data-stu-id="be5ae-130">Untyped JSON object</span></span> | <span data-ttu-id="be5ae-131">可选。</span><span class="sxs-lookup"><span data-stu-id="be5ae-131">Optional.</span></span> <span data-ttu-id="be5ae-132">自定义的数据的 JSON 对象，用于提供自定义呈现 Windows 命令行管理程序用户界面中的活动内容</span><span class="sxs-lookup"><span data-stu-id="be5ae-132">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="be5ae-133">属性</span><span class="sxs-lookup"><span data-stu-id="be5ae-133">attribution</span></span> | [<span data-ttu-id="be5ae-134">imageInfo</span><span class="sxs-lookup"><span data-stu-id="be5ae-134">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="be5ae-135">可选。</span><span class="sxs-lookup"><span data-stu-id="be5ae-135">Optional.</span></span> <span data-ttu-id="be5ae-136">JSON 对象，用于表示一个表示用于生成活动的应用程序图标</span><span class="sxs-lookup"><span data-stu-id="be5ae-136">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be5ae-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be5ae-137">JSON Representation</span></span>

<span data-ttu-id="be5ae-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be5ae-138">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-visualinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
