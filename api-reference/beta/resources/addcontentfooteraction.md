---
title: addContentFooterAction 资源类型
description: 表示一个操作，该操作指定要添加到信息中的内容页脚的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 05bbd7ee4b2d4b2b9c4e772b19bd26c86d91cc69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508420"
---
# <a name="addcontentfooteraction-resource-type"></a><span data-ttu-id="ee51b-103">addContentFooterAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee51b-103">addContentFooterAction resource type</span></span>

<span data-ttu-id="ee51b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ee51b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee51b-105">表示一个操作，该操作指定要添加到信息中的内容页脚的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="ee51b-105">Represents an action that specifies the details on the content footer to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="ee51b-106">属性</span><span class="sxs-lookup"><span data-stu-id="ee51b-106">Properties</span></span>

| <span data-ttu-id="ee51b-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee51b-107">Property</span></span>      | <span data-ttu-id="ee51b-108">类型</span><span class="sxs-lookup"><span data-stu-id="ee51b-108">Type</span></span>   | <span data-ttu-id="ee51b-109">说明</span><span class="sxs-lookup"><span data-stu-id="ee51b-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="ee51b-110">alignment</span><span class="sxs-lookup"><span data-stu-id="ee51b-110">alignment</span></span>     | <span data-ttu-id="ee51b-111">String</span><span class="sxs-lookup"><span data-stu-id="ee51b-111">String</span></span> | <span data-ttu-id="ee51b-112">可取值为：`left`、`right`、`center`。</span><span class="sxs-lookup"><span data-stu-id="ee51b-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="ee51b-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="ee51b-113">fontColor</span></span>     | <span data-ttu-id="ee51b-114">String</span><span class="sxs-lookup"><span data-stu-id="ee51b-114">String</span></span> | <span data-ttu-id="ee51b-115">用于页脚的字体颜色。</span><span class="sxs-lookup"><span data-stu-id="ee51b-115">Color of the font to use for the footer.</span></span>                      |
| <span data-ttu-id="ee51b-116">fontName</span><span class="sxs-lookup"><span data-stu-id="ee51b-116">fontName</span></span>      | <span data-ttu-id="ee51b-117">String</span><span class="sxs-lookup"><span data-stu-id="ee51b-117">String</span></span> | <span data-ttu-id="ee51b-118">要用于页脚的字体的名称。</span><span class="sxs-lookup"><span data-stu-id="ee51b-118">Name of the font to use for the footer.</span></span>                       |
| <span data-ttu-id="ee51b-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="ee51b-119">fontSize</span></span>      | <span data-ttu-id="ee51b-120">Int32</span><span class="sxs-lookup"><span data-stu-id="ee51b-120">Int32</span></span>  | <span data-ttu-id="ee51b-121">用于页脚的字号。</span><span class="sxs-lookup"><span data-stu-id="ee51b-121">Font size to use for the footer.</span></span>                              |
| <span data-ttu-id="ee51b-122">页脚</span><span class="sxs-lookup"><span data-stu-id="ee51b-122">margin</span></span>        | <span data-ttu-id="ee51b-123">Int32</span><span class="sxs-lookup"><span data-stu-id="ee51b-123">Int32</span></span>  | <span data-ttu-id="ee51b-124">文档底部的页眉的边距。</span><span class="sxs-lookup"><span data-stu-id="ee51b-124">The margin of the header from the bottom of the document.</span></span>     |
| <span data-ttu-id="ee51b-125">text</span><span class="sxs-lookup"><span data-stu-id="ee51b-125">text</span></span>          | <span data-ttu-id="ee51b-126">String</span><span class="sxs-lookup"><span data-stu-id="ee51b-126">String</span></span> | <span data-ttu-id="ee51b-127">页脚本身的内容。</span><span class="sxs-lookup"><span data-stu-id="ee51b-127">The contents of the footer itself.</span></span>                            |
| <span data-ttu-id="ee51b-128">uiElementName</span><span class="sxs-lookup"><span data-stu-id="ee51b-128">uiElementName</span></span> | <span data-ttu-id="ee51b-129">String</span><span class="sxs-lookup"><span data-stu-id="ee51b-129">String</span></span> | <span data-ttu-id="ee51b-130">应在其中放置页脚的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="ee51b-130">The name of the UI element where the footer should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ee51b-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee51b-131">JSON representation</span></span>

<span data-ttu-id="ee51b-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee51b-132">The following is a JSON representation of the resource.</span></span>

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