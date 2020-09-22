---
title: addContentFooterAction 资源类型
description: 表示一个操作，该操作指定要添加到信息中的内容页脚的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b4e9edf4007d7bc5d4028e4f9202e09647ca863
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024513"
---
# <a name="addcontentfooteraction-resource-type"></a><span data-ttu-id="6ebe4-103">addContentFooterAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ebe4-103">addContentFooterAction resource type</span></span>

<span data-ttu-id="6ebe4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ebe4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ebe4-105">表示一个操作，该操作指定要添加到信息中的内容页脚的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="6ebe4-105">Represents an action that specifies the details on the content footer to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="6ebe4-106">属性</span><span class="sxs-lookup"><span data-stu-id="6ebe4-106">Properties</span></span>

| <span data-ttu-id="6ebe4-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ebe4-107">Property</span></span>      | <span data-ttu-id="6ebe4-108">类型</span><span class="sxs-lookup"><span data-stu-id="6ebe4-108">Type</span></span>   | <span data-ttu-id="6ebe4-109">说明</span><span class="sxs-lookup"><span data-stu-id="6ebe4-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="6ebe4-110">alignment</span><span class="sxs-lookup"><span data-stu-id="6ebe4-110">alignment</span></span>     | <span data-ttu-id="6ebe4-111">String</span><span class="sxs-lookup"><span data-stu-id="6ebe4-111">String</span></span> | <span data-ttu-id="6ebe4-112">可取值为：`left`、`right`、`center`。</span><span class="sxs-lookup"><span data-stu-id="6ebe4-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="6ebe4-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="6ebe4-113">fontColor</span></span>     | <span data-ttu-id="6ebe4-114">String</span><span class="sxs-lookup"><span data-stu-id="6ebe4-114">String</span></span> | <span data-ttu-id="6ebe4-115">用于页脚的字体颜色。</span><span class="sxs-lookup"><span data-stu-id="6ebe4-115">Color of the font to use for the footer.</span></span>                      |
| <span data-ttu-id="6ebe4-116">fontName</span><span class="sxs-lookup"><span data-stu-id="6ebe4-116">fontName</span></span>      | <span data-ttu-id="6ebe4-117">String</span><span class="sxs-lookup"><span data-stu-id="6ebe4-117">String</span></span> | <span data-ttu-id="6ebe4-118">要用于页脚的字体的名称。</span><span class="sxs-lookup"><span data-stu-id="6ebe4-118">Name of the font to use for the footer.</span></span>                       |
| <span data-ttu-id="6ebe4-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="6ebe4-119">fontSize</span></span>      | <span data-ttu-id="6ebe4-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6ebe4-120">Int32</span></span>  | <span data-ttu-id="6ebe4-121">用于页脚的字号。</span><span class="sxs-lookup"><span data-stu-id="6ebe4-121">Font size to use for the footer.</span></span>                              |
| <span data-ttu-id="6ebe4-122">margin</span><span class="sxs-lookup"><span data-stu-id="6ebe4-122">margin</span></span>        | <span data-ttu-id="6ebe4-123">Int32</span><span class="sxs-lookup"><span data-stu-id="6ebe4-123">Int32</span></span>  | <span data-ttu-id="6ebe4-124">文档底部的页眉的边距。</span><span class="sxs-lookup"><span data-stu-id="6ebe4-124">The margin of the header from the bottom of the document.</span></span>     |
| <span data-ttu-id="6ebe4-125">text</span><span class="sxs-lookup"><span data-stu-id="6ebe4-125">text</span></span>          | <span data-ttu-id="6ebe4-126">String</span><span class="sxs-lookup"><span data-stu-id="6ebe4-126">String</span></span> | <span data-ttu-id="6ebe4-127">页脚本身的内容。</span><span class="sxs-lookup"><span data-stu-id="6ebe4-127">The contents of the footer itself.</span></span>                            |
| <span data-ttu-id="6ebe4-128">uiElementName</span><span class="sxs-lookup"><span data-stu-id="6ebe4-128">uiElementName</span></span> | <span data-ttu-id="6ebe4-129">String</span><span class="sxs-lookup"><span data-stu-id="6ebe4-129">String</span></span> | <span data-ttu-id="6ebe4-130">应在其中放置页脚的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="6ebe4-130">The name of the UI element where the footer should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6ebe4-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ebe4-131">JSON representation</span></span>

<span data-ttu-id="6ebe4-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ebe4-132">The following is a JSON representation of the resource.</span></span>

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

