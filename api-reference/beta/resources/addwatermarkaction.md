---
title: addWatermarkAction 资源类型
description: 表示一个操作，该操作指定要添加到信息中的内容水印的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4ba3bd679d01d31aec779071a766ab804761e614
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939164"
---
# <a name="addwatermarkaction-resource-type"></a><span data-ttu-id="64f93-103">addWatermarkAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="64f93-103">addWatermarkAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64f93-104">表示一个操作，该操作指定要添加到信息中的内容水印的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="64f93-104">Represents an action that specifies the details on the content watermark to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="64f93-105">属性</span><span class="sxs-lookup"><span data-stu-id="64f93-105">Properties</span></span>

| <span data-ttu-id="64f93-106">属性</span><span class="sxs-lookup"><span data-stu-id="64f93-106">Property</span></span>      | <span data-ttu-id="64f93-107">类型</span><span class="sxs-lookup"><span data-stu-id="64f93-107">Type</span></span>   | <span data-ttu-id="64f93-108">描述</span><span class="sxs-lookup"><span data-stu-id="64f93-108">Description</span></span>                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| <span data-ttu-id="64f93-109">fontColor</span><span class="sxs-lookup"><span data-stu-id="64f93-109">fontColor</span></span>     | <span data-ttu-id="64f93-110">字符串</span><span class="sxs-lookup"><span data-stu-id="64f93-110">String</span></span> | <span data-ttu-id="64f93-111">用于水印的字体颜色。</span><span class="sxs-lookup"><span data-stu-id="64f93-111">Color of the font to use for the watermark.</span></span>                      |
| <span data-ttu-id="64f93-112">fontName</span><span class="sxs-lookup"><span data-stu-id="64f93-112">fontName</span></span>      | <span data-ttu-id="64f93-113">字符串</span><span class="sxs-lookup"><span data-stu-id="64f93-113">String</span></span> | <span data-ttu-id="64f93-114">要用于水印的字体的名称。</span><span class="sxs-lookup"><span data-stu-id="64f93-114">Name of the font to use for the watermark.</span></span>                       |
| <span data-ttu-id="64f93-115">fontSize</span><span class="sxs-lookup"><span data-stu-id="64f93-115">fontSize</span></span>      | <span data-ttu-id="64f93-116">Int32</span><span class="sxs-lookup"><span data-stu-id="64f93-116">Int32</span></span>  | <span data-ttu-id="64f93-117">用于水印的字号。</span><span class="sxs-lookup"><span data-stu-id="64f93-117">Font size to use for the watermark.</span></span>                              |
| <span data-ttu-id="64f93-118">布局</span><span class="sxs-lookup"><span data-stu-id="64f93-118">layout</span></span>        | <span data-ttu-id="64f93-119">String</span><span class="sxs-lookup"><span data-stu-id="64f93-119">String</span></span> | <span data-ttu-id="64f93-120">可取值为：`horizontal`、`diagonal`。</span><span class="sxs-lookup"><span data-stu-id="64f93-120">Possible values are: `horizontal`, `diagonal`.</span></span>                   |
| <span data-ttu-id="64f93-121">text</span><span class="sxs-lookup"><span data-stu-id="64f93-121">text</span></span>          | <span data-ttu-id="64f93-122">字符串</span><span class="sxs-lookup"><span data-stu-id="64f93-122">String</span></span> | <span data-ttu-id="64f93-123">水印本身的内容。</span><span class="sxs-lookup"><span data-stu-id="64f93-123">The contents of the watermark itself.</span></span>                            |
| <span data-ttu-id="64f93-124">uiElementName</span><span class="sxs-lookup"><span data-stu-id="64f93-124">uiElementName</span></span> | <span data-ttu-id="64f93-125">字符串</span><span class="sxs-lookup"><span data-stu-id="64f93-125">String</span></span> | <span data-ttu-id="64f93-126">应在其中放置水印的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="64f93-126">The name of the UI element where the watermark should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64f93-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64f93-127">JSON representation</span></span>

<span data-ttu-id="64f93-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64f93-128">The following is a JSON representation of the resource.</span></span>

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