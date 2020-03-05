---
title: addContentHeaderAction 资源类型
description: 表示一个操作，该操作指定要添加到信息中的内容标头的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d426252b6ab83557c3d3085ac4ffa7a530aae271
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508406"
---
# <a name="addcontentheaderaction-resource-type"></a><span data-ttu-id="adb41-103">addContentHeaderAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="adb41-103">addContentHeaderAction resource type</span></span>

<span data-ttu-id="adb41-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="adb41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adb41-105">表示一个操作，该操作指定要添加到信息中的内容标头的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="adb41-105">Represents an action that specifies the details on the content header to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="adb41-106">属性</span><span class="sxs-lookup"><span data-stu-id="adb41-106">Properties</span></span>

| <span data-ttu-id="adb41-107">属性</span><span class="sxs-lookup"><span data-stu-id="adb41-107">Property</span></span>      | <span data-ttu-id="adb41-108">类型</span><span class="sxs-lookup"><span data-stu-id="adb41-108">Type</span></span>   | <span data-ttu-id="adb41-109">说明</span><span class="sxs-lookup"><span data-stu-id="adb41-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="adb41-110">alignment</span><span class="sxs-lookup"><span data-stu-id="adb41-110">alignment</span></span>     | <span data-ttu-id="adb41-111">String</span><span class="sxs-lookup"><span data-stu-id="adb41-111">String</span></span> | <span data-ttu-id="adb41-112">可取值为：`left`、`right`、`center`。</span><span class="sxs-lookup"><span data-stu-id="adb41-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="adb41-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="adb41-113">fontColor</span></span>     | <span data-ttu-id="adb41-114">String</span><span class="sxs-lookup"><span data-stu-id="adb41-114">String</span></span> | <span data-ttu-id="adb41-115">标头使用的字体颜色。</span><span class="sxs-lookup"><span data-stu-id="adb41-115">Color of the font to use for the header.</span></span>                      |
| <span data-ttu-id="adb41-116">fontName</span><span class="sxs-lookup"><span data-stu-id="adb41-116">fontName</span></span>      | <span data-ttu-id="adb41-117">String</span><span class="sxs-lookup"><span data-stu-id="adb41-117">String</span></span> | <span data-ttu-id="adb41-118">要用于标头的字体的名称。</span><span class="sxs-lookup"><span data-stu-id="adb41-118">Name of the font to use for the header.</span></span>                       |
| <span data-ttu-id="adb41-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="adb41-119">fontSize</span></span>      | <span data-ttu-id="adb41-120">Int32</span><span class="sxs-lookup"><span data-stu-id="adb41-120">Int32</span></span>  | <span data-ttu-id="adb41-121">标头使用的字号。</span><span class="sxs-lookup"><span data-stu-id="adb41-121">Font size to use for the header.</span></span>                              |
| <span data-ttu-id="adb41-122">页脚</span><span class="sxs-lookup"><span data-stu-id="adb41-122">margin</span></span>        | <span data-ttu-id="adb41-123">Int32</span><span class="sxs-lookup"><span data-stu-id="adb41-123">Int32</span></span>  | <span data-ttu-id="adb41-124">文档顶部的页眉的边距。</span><span class="sxs-lookup"><span data-stu-id="adb41-124">The margin of the header from the top of the document.</span></span>        |
| <span data-ttu-id="adb41-125">text</span><span class="sxs-lookup"><span data-stu-id="adb41-125">text</span></span>          | <span data-ttu-id="adb41-126">String</span><span class="sxs-lookup"><span data-stu-id="adb41-126">String</span></span> | <span data-ttu-id="adb41-127">标头本身的内容。</span><span class="sxs-lookup"><span data-stu-id="adb41-127">The contents of the header itself.</span></span>                            |
| <span data-ttu-id="adb41-128">uiElementName</span><span class="sxs-lookup"><span data-stu-id="adb41-128">uiElementName</span></span> | <span data-ttu-id="adb41-129">String</span><span class="sxs-lookup"><span data-stu-id="adb41-129">String</span></span> | <span data-ttu-id="adb41-130">应在其中放置标头的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="adb41-130">The name of the UI element where the header should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="adb41-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="adb41-131">JSON representation</span></span>

<span data-ttu-id="adb41-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adb41-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentHeaderAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "alignment": "String",
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "margin": 1024,
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->