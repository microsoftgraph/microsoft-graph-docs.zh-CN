---
title: addWatermarkAction 资源类型
description: 表示一个操作，该操作指定要添加到信息中的内容水印的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 884553ce1181fd3d79fe0e953fe7703b386698b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024432"
---
# <a name="addwatermarkaction-resource-type"></a><span data-ttu-id="cbe0d-103">addWatermarkAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="cbe0d-103">addWatermarkAction resource type</span></span>

<span data-ttu-id="cbe0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbe0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbe0d-105">表示一个操作，该操作指定要添加到信息中的内容水印的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="cbe0d-105">Represents an action that specifies the details on the content watermark to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="cbe0d-106">属性</span><span class="sxs-lookup"><span data-stu-id="cbe0d-106">Properties</span></span>

| <span data-ttu-id="cbe0d-107">属性</span><span class="sxs-lookup"><span data-stu-id="cbe0d-107">Property</span></span>      | <span data-ttu-id="cbe0d-108">类型</span><span class="sxs-lookup"><span data-stu-id="cbe0d-108">Type</span></span>   | <span data-ttu-id="cbe0d-109">说明</span><span class="sxs-lookup"><span data-stu-id="cbe0d-109">Description</span></span>                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| <span data-ttu-id="cbe0d-110">fontColor</span><span class="sxs-lookup"><span data-stu-id="cbe0d-110">fontColor</span></span>     | <span data-ttu-id="cbe0d-111">String</span><span class="sxs-lookup"><span data-stu-id="cbe0d-111">String</span></span> | <span data-ttu-id="cbe0d-112">用于水印的字体颜色。</span><span class="sxs-lookup"><span data-stu-id="cbe0d-112">Color of the font to use for the watermark.</span></span>                      |
| <span data-ttu-id="cbe0d-113">fontName</span><span class="sxs-lookup"><span data-stu-id="cbe0d-113">fontName</span></span>      | <span data-ttu-id="cbe0d-114">String</span><span class="sxs-lookup"><span data-stu-id="cbe0d-114">String</span></span> | <span data-ttu-id="cbe0d-115">要用于水印的字体的名称。</span><span class="sxs-lookup"><span data-stu-id="cbe0d-115">Name of the font to use for the watermark.</span></span>                       |
| <span data-ttu-id="cbe0d-116">fontSize</span><span class="sxs-lookup"><span data-stu-id="cbe0d-116">fontSize</span></span>      | <span data-ttu-id="cbe0d-117">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe0d-117">Int32</span></span>  | <span data-ttu-id="cbe0d-118">用于水印的字号。</span><span class="sxs-lookup"><span data-stu-id="cbe0d-118">Font size to use for the watermark.</span></span>                              |
| <span data-ttu-id="cbe0d-119">布局</span><span class="sxs-lookup"><span data-stu-id="cbe0d-119">layout</span></span>        | <span data-ttu-id="cbe0d-120">String</span><span class="sxs-lookup"><span data-stu-id="cbe0d-120">String</span></span> | <span data-ttu-id="cbe0d-121">可取值为：`horizontal`、`diagonal`。</span><span class="sxs-lookup"><span data-stu-id="cbe0d-121">Possible values are: `horizontal`, `diagonal`.</span></span>                   |
| <span data-ttu-id="cbe0d-122">text</span><span class="sxs-lookup"><span data-stu-id="cbe0d-122">text</span></span>          | <span data-ttu-id="cbe0d-123">String</span><span class="sxs-lookup"><span data-stu-id="cbe0d-123">String</span></span> | <span data-ttu-id="cbe0d-124">水印本身的内容。</span><span class="sxs-lookup"><span data-stu-id="cbe0d-124">The contents of the watermark itself.</span></span>                            |
| <span data-ttu-id="cbe0d-125">uiElementName</span><span class="sxs-lookup"><span data-stu-id="cbe0d-125">uiElementName</span></span> | <span data-ttu-id="cbe0d-126">String</span><span class="sxs-lookup"><span data-stu-id="cbe0d-126">String</span></span> | <span data-ttu-id="cbe0d-127">应在其中放置水印的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="cbe0d-127">The name of the UI element where the watermark should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cbe0d-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cbe0d-128">JSON representation</span></span>

<span data-ttu-id="cbe0d-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbe0d-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addWatermarkAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "layout": "String",
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addWatermarkAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

