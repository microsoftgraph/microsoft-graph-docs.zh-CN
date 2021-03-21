---
title: addContentHeaderAction 资源类型
description: 表示一个操作，指定要添加到信息的内容标头的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 65754bffc034611fd319403cd81d931addfea9f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962132"
---
# <a name="addcontentheaderaction-resource-type"></a><span data-ttu-id="66ecd-103">addContentHeaderAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="66ecd-103">addContentHeaderAction resource type</span></span>

<span data-ttu-id="66ecd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66ecd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66ecd-105">表示一个操作，指定要添加到信息的内容标头的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="66ecd-105">Represents an action that specifies the details on the content header to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="66ecd-106">属性</span><span class="sxs-lookup"><span data-stu-id="66ecd-106">Properties</span></span>

| <span data-ttu-id="66ecd-107">属性</span><span class="sxs-lookup"><span data-stu-id="66ecd-107">Property</span></span>      | <span data-ttu-id="66ecd-108">类型</span><span class="sxs-lookup"><span data-stu-id="66ecd-108">Type</span></span>   | <span data-ttu-id="66ecd-109">说明</span><span class="sxs-lookup"><span data-stu-id="66ecd-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="66ecd-110">alignment</span><span class="sxs-lookup"><span data-stu-id="66ecd-110">alignment</span></span>     | <span data-ttu-id="66ecd-111">String</span><span class="sxs-lookup"><span data-stu-id="66ecd-111">String</span></span> | <span data-ttu-id="66ecd-112">可取值为：`left`、`right`、`center`。</span><span class="sxs-lookup"><span data-stu-id="66ecd-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="66ecd-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="66ecd-113">fontColor</span></span>     | <span data-ttu-id="66ecd-114">String</span><span class="sxs-lookup"><span data-stu-id="66ecd-114">String</span></span> | <span data-ttu-id="66ecd-115">用于标题的字体的颜色。</span><span class="sxs-lookup"><span data-stu-id="66ecd-115">Color of the font to use for the header.</span></span>                      |
| <span data-ttu-id="66ecd-116">fontName</span><span class="sxs-lookup"><span data-stu-id="66ecd-116">fontName</span></span>      | <span data-ttu-id="66ecd-117">String</span><span class="sxs-lookup"><span data-stu-id="66ecd-117">String</span></span> | <span data-ttu-id="66ecd-118">要用于标题的字体的名称。</span><span class="sxs-lookup"><span data-stu-id="66ecd-118">Name of the font to use for the header.</span></span>                       |
| <span data-ttu-id="66ecd-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="66ecd-119">fontSize</span></span>      | <span data-ttu-id="66ecd-120">Int32</span><span class="sxs-lookup"><span data-stu-id="66ecd-120">Int32</span></span>  | <span data-ttu-id="66ecd-121">用于标题的字体大小。</span><span class="sxs-lookup"><span data-stu-id="66ecd-121">Font size to use for the header.</span></span>                              |
| <span data-ttu-id="66ecd-122">margin</span><span class="sxs-lookup"><span data-stu-id="66ecd-122">margin</span></span>        | <span data-ttu-id="66ecd-123">Int32</span><span class="sxs-lookup"><span data-stu-id="66ecd-123">Int32</span></span>  | <span data-ttu-id="66ecd-124">从文档顶部开始页眉的边距。</span><span class="sxs-lookup"><span data-stu-id="66ecd-124">The margin of the header from the top of the document.</span></span>        |
| <span data-ttu-id="66ecd-125">text</span><span class="sxs-lookup"><span data-stu-id="66ecd-125">text</span></span>          | <span data-ttu-id="66ecd-126">String</span><span class="sxs-lookup"><span data-stu-id="66ecd-126">String</span></span> | <span data-ttu-id="66ecd-127">标头本身的内容。</span><span class="sxs-lookup"><span data-stu-id="66ecd-127">The contents of the header itself.</span></span>                            |
| <span data-ttu-id="66ecd-128">uiElementName</span><span class="sxs-lookup"><span data-stu-id="66ecd-128">uiElementName</span></span> | <span data-ttu-id="66ecd-129">String</span><span class="sxs-lookup"><span data-stu-id="66ecd-129">String</span></span> | <span data-ttu-id="66ecd-130">应放置标题的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="66ecd-130">The name of the UI element where the header should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66ecd-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66ecd-131">JSON representation</span></span>

<span data-ttu-id="66ecd-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66ecd-132">The following is a JSON representation of the resource.</span></span>

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

