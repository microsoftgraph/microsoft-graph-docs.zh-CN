---
title: addContentFooterAction 资源类型
description: 表示一个操作，指定要添加到信息的内容页脚的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 20debce7dc408bd10d4f62b905efa55156d4d4ca
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962133"
---
# <a name="addcontentfooteraction-resource-type"></a><span data-ttu-id="f78a8-103">addContentFooterAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="f78a8-103">addContentFooterAction resource type</span></span>

<span data-ttu-id="f78a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f78a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f78a8-105">表示一个操作，指定要添加到信息的内容页脚的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="f78a8-105">Represents an action that specifies the details on the content footer to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="f78a8-106">属性</span><span class="sxs-lookup"><span data-stu-id="f78a8-106">Properties</span></span>

| <span data-ttu-id="f78a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="f78a8-107">Property</span></span>      | <span data-ttu-id="f78a8-108">类型</span><span class="sxs-lookup"><span data-stu-id="f78a8-108">Type</span></span>   | <span data-ttu-id="f78a8-109">说明</span><span class="sxs-lookup"><span data-stu-id="f78a8-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="f78a8-110">alignment</span><span class="sxs-lookup"><span data-stu-id="f78a8-110">alignment</span></span>     | <span data-ttu-id="f78a8-111">String</span><span class="sxs-lookup"><span data-stu-id="f78a8-111">String</span></span> | <span data-ttu-id="f78a8-112">可取值为：`left`、`right`、`center`。</span><span class="sxs-lookup"><span data-stu-id="f78a8-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="f78a8-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="f78a8-113">fontColor</span></span>     | <span data-ttu-id="f78a8-114">String</span><span class="sxs-lookup"><span data-stu-id="f78a8-114">String</span></span> | <span data-ttu-id="f78a8-115">用于页脚的字体的颜色。</span><span class="sxs-lookup"><span data-stu-id="f78a8-115">Color of the font to use for the footer.</span></span>                      |
| <span data-ttu-id="f78a8-116">fontName</span><span class="sxs-lookup"><span data-stu-id="f78a8-116">fontName</span></span>      | <span data-ttu-id="f78a8-117">String</span><span class="sxs-lookup"><span data-stu-id="f78a8-117">String</span></span> | <span data-ttu-id="f78a8-118">用于页脚的字体的名称。</span><span class="sxs-lookup"><span data-stu-id="f78a8-118">Name of the font to use for the footer.</span></span>                       |
| <span data-ttu-id="f78a8-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="f78a8-119">fontSize</span></span>      | <span data-ttu-id="f78a8-120">Int32</span><span class="sxs-lookup"><span data-stu-id="f78a8-120">Int32</span></span>  | <span data-ttu-id="f78a8-121">用于页脚的字体大小。</span><span class="sxs-lookup"><span data-stu-id="f78a8-121">Font size to use for the footer.</span></span>                              |
| <span data-ttu-id="f78a8-122">margin</span><span class="sxs-lookup"><span data-stu-id="f78a8-122">margin</span></span>        | <span data-ttu-id="f78a8-123">Int32</span><span class="sxs-lookup"><span data-stu-id="f78a8-123">Int32</span></span>  | <span data-ttu-id="f78a8-124">文档底部的页眉边距。</span><span class="sxs-lookup"><span data-stu-id="f78a8-124">The margin of the header from the bottom of the document.</span></span>     |
| <span data-ttu-id="f78a8-125">text</span><span class="sxs-lookup"><span data-stu-id="f78a8-125">text</span></span>          | <span data-ttu-id="f78a8-126">String</span><span class="sxs-lookup"><span data-stu-id="f78a8-126">String</span></span> | <span data-ttu-id="f78a8-127">页脚本身的内容。</span><span class="sxs-lookup"><span data-stu-id="f78a8-127">The contents of the footer itself.</span></span>                            |
| <span data-ttu-id="f78a8-128">uiElementName</span><span class="sxs-lookup"><span data-stu-id="f78a8-128">uiElementName</span></span> | <span data-ttu-id="f78a8-129">String</span><span class="sxs-lookup"><span data-stu-id="f78a8-129">String</span></span> | <span data-ttu-id="f78a8-130">放置页脚的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="f78a8-130">The name of the UI element where the footer should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f78a8-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f78a8-131">JSON representation</span></span>

<span data-ttu-id="f78a8-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f78a8-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentFooterAction",
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
  "description": "addContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

