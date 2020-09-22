---
title: addContentHeaderAction 资源类型
description: 表示一个操作，该操作指定要添加到信息中的内容标头的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7e7a5675cdf150f03b283f664e248319d49c820d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024514"
---
# <a name="addcontentheaderaction-resource-type"></a><span data-ttu-id="e6722-103">addContentHeaderAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6722-103">addContentHeaderAction resource type</span></span>

<span data-ttu-id="e6722-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6722-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6722-105">表示一个操作，该操作指定要添加到信息中的内容标头的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="e6722-105">Represents an action that specifies the details on the content header to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="e6722-106">属性</span><span class="sxs-lookup"><span data-stu-id="e6722-106">Properties</span></span>

| <span data-ttu-id="e6722-107">属性</span><span class="sxs-lookup"><span data-stu-id="e6722-107">Property</span></span>      | <span data-ttu-id="e6722-108">类型</span><span class="sxs-lookup"><span data-stu-id="e6722-108">Type</span></span>   | <span data-ttu-id="e6722-109">说明</span><span class="sxs-lookup"><span data-stu-id="e6722-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="e6722-110">alignment</span><span class="sxs-lookup"><span data-stu-id="e6722-110">alignment</span></span>     | <span data-ttu-id="e6722-111">String</span><span class="sxs-lookup"><span data-stu-id="e6722-111">String</span></span> | <span data-ttu-id="e6722-112">可取值为：`left`、`right`、`center`。</span><span class="sxs-lookup"><span data-stu-id="e6722-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="e6722-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="e6722-113">fontColor</span></span>     | <span data-ttu-id="e6722-114">String</span><span class="sxs-lookup"><span data-stu-id="e6722-114">String</span></span> | <span data-ttu-id="e6722-115">标头使用的字体颜色。</span><span class="sxs-lookup"><span data-stu-id="e6722-115">Color of the font to use for the header.</span></span>                      |
| <span data-ttu-id="e6722-116">fontName</span><span class="sxs-lookup"><span data-stu-id="e6722-116">fontName</span></span>      | <span data-ttu-id="e6722-117">String</span><span class="sxs-lookup"><span data-stu-id="e6722-117">String</span></span> | <span data-ttu-id="e6722-118">要用于标头的字体的名称。</span><span class="sxs-lookup"><span data-stu-id="e6722-118">Name of the font to use for the header.</span></span>                       |
| <span data-ttu-id="e6722-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="e6722-119">fontSize</span></span>      | <span data-ttu-id="e6722-120">Int32</span><span class="sxs-lookup"><span data-stu-id="e6722-120">Int32</span></span>  | <span data-ttu-id="e6722-121">标头使用的字号。</span><span class="sxs-lookup"><span data-stu-id="e6722-121">Font size to use for the header.</span></span>                              |
| <span data-ttu-id="e6722-122">margin</span><span class="sxs-lookup"><span data-stu-id="e6722-122">margin</span></span>        | <span data-ttu-id="e6722-123">Int32</span><span class="sxs-lookup"><span data-stu-id="e6722-123">Int32</span></span>  | <span data-ttu-id="e6722-124">文档顶部的页眉的边距。</span><span class="sxs-lookup"><span data-stu-id="e6722-124">The margin of the header from the top of the document.</span></span>        |
| <span data-ttu-id="e6722-125">text</span><span class="sxs-lookup"><span data-stu-id="e6722-125">text</span></span>          | <span data-ttu-id="e6722-126">String</span><span class="sxs-lookup"><span data-stu-id="e6722-126">String</span></span> | <span data-ttu-id="e6722-127">标头本身的内容。</span><span class="sxs-lookup"><span data-stu-id="e6722-127">The contents of the header itself.</span></span>                            |
| <span data-ttu-id="e6722-128">uiElementName</span><span class="sxs-lookup"><span data-stu-id="e6722-128">uiElementName</span></span> | <span data-ttu-id="e6722-129">String</span><span class="sxs-lookup"><span data-stu-id="e6722-129">String</span></span> | <span data-ttu-id="e6722-130">应在其中放置标头的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="e6722-130">The name of the UI element where the header should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e6722-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6722-131">JSON representation</span></span>

<span data-ttu-id="e6722-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6722-132">The following is a JSON representation of the resource.</span></span>

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

