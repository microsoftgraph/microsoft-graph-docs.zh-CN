---
title: add的markAction 资源类型
description: 表示指定要添加到信息的内容水印的详细信息的操作（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: db493c57d6de7c840e5f0606743392698cb475b6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962124"
---
# <a name="addwatermarkaction-resource-type"></a><span data-ttu-id="f0b57-103">add的markAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0b57-103">addWatermarkAction resource type</span></span>

<span data-ttu-id="f0b57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0b57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0b57-105">表示指定要添加到信息的内容水印的详细信息的操作（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="f0b57-105">Represents an action that specifies the details on the content watermark to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="f0b57-106">属性</span><span class="sxs-lookup"><span data-stu-id="f0b57-106">Properties</span></span>

| <span data-ttu-id="f0b57-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0b57-107">Property</span></span>      | <span data-ttu-id="f0b57-108">类型</span><span class="sxs-lookup"><span data-stu-id="f0b57-108">Type</span></span>   | <span data-ttu-id="f0b57-109">说明</span><span class="sxs-lookup"><span data-stu-id="f0b57-109">Description</span></span>                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| <span data-ttu-id="f0b57-110">fontColor</span><span class="sxs-lookup"><span data-stu-id="f0b57-110">fontColor</span></span>     | <span data-ttu-id="f0b57-111">String</span><span class="sxs-lookup"><span data-stu-id="f0b57-111">String</span></span> | <span data-ttu-id="f0b57-112">用于水印的字体的颜色。</span><span class="sxs-lookup"><span data-stu-id="f0b57-112">Color of the font to use for the watermark.</span></span>                      |
| <span data-ttu-id="f0b57-113">fontName</span><span class="sxs-lookup"><span data-stu-id="f0b57-113">fontName</span></span>      | <span data-ttu-id="f0b57-114">String</span><span class="sxs-lookup"><span data-stu-id="f0b57-114">String</span></span> | <span data-ttu-id="f0b57-115">用于水印的字体的名称。</span><span class="sxs-lookup"><span data-stu-id="f0b57-115">Name of the font to use for the watermark.</span></span>                       |
| <span data-ttu-id="f0b57-116">fontSize</span><span class="sxs-lookup"><span data-stu-id="f0b57-116">fontSize</span></span>      | <span data-ttu-id="f0b57-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f0b57-117">Int32</span></span>  | <span data-ttu-id="f0b57-118">用于水印的字体大小。</span><span class="sxs-lookup"><span data-stu-id="f0b57-118">Font size to use for the watermark.</span></span>                              |
| <span data-ttu-id="f0b57-119">layout</span><span class="sxs-lookup"><span data-stu-id="f0b57-119">layout</span></span>        | <span data-ttu-id="f0b57-120">String</span><span class="sxs-lookup"><span data-stu-id="f0b57-120">String</span></span> | <span data-ttu-id="f0b57-121">可取值为：`horizontal`、`diagonal`。</span><span class="sxs-lookup"><span data-stu-id="f0b57-121">Possible values are: `horizontal`, `diagonal`.</span></span>                   |
| <span data-ttu-id="f0b57-122">text</span><span class="sxs-lookup"><span data-stu-id="f0b57-122">text</span></span>          | <span data-ttu-id="f0b57-123">String</span><span class="sxs-lookup"><span data-stu-id="f0b57-123">String</span></span> | <span data-ttu-id="f0b57-124">水印本身的内容。</span><span class="sxs-lookup"><span data-stu-id="f0b57-124">The contents of the watermark itself.</span></span>                            |
| <span data-ttu-id="f0b57-125">uiElementName</span><span class="sxs-lookup"><span data-stu-id="f0b57-125">uiElementName</span></span> | <span data-ttu-id="f0b57-126">String</span><span class="sxs-lookup"><span data-stu-id="f0b57-126">String</span></span> | <span data-ttu-id="f0b57-127">应放置水印的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="f0b57-127">The name of the UI element where the watermark should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f0b57-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0b57-128">JSON representation</span></span>

<span data-ttu-id="f0b57-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0b57-129">The following is a JSON representation of the resource.</span></span>

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

