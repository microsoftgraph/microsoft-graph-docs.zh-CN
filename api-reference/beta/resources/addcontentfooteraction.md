---
title: addContentFooterAction 资源类型
description: 表示一个操作，该操作指定要添加到信息中的内容页脚的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b1a2cb0f3e2ffbfb5554c4ae0323cf4fd028e0c8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939102"
---
# <a name="addcontentfooteraction-resource-type"></a><span data-ttu-id="eee84-103">addContentFooterAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="eee84-103">addContentFooterAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eee84-104">表示一个操作，该操作指定要添加到信息中的内容页脚的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="eee84-104">Represents an action that specifies the details on the content footer to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="eee84-105">属性</span><span class="sxs-lookup"><span data-stu-id="eee84-105">Properties</span></span>

| <span data-ttu-id="eee84-106">属性</span><span class="sxs-lookup"><span data-stu-id="eee84-106">Property</span></span>      | <span data-ttu-id="eee84-107">类型</span><span class="sxs-lookup"><span data-stu-id="eee84-107">Type</span></span>   | <span data-ttu-id="eee84-108">描述</span><span class="sxs-lookup"><span data-stu-id="eee84-108">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="eee84-109">alignment</span><span class="sxs-lookup"><span data-stu-id="eee84-109">alignment</span></span>     | <span data-ttu-id="eee84-110">字符串</span><span class="sxs-lookup"><span data-stu-id="eee84-110">String</span></span> | <span data-ttu-id="eee84-111">可取值为：`left`、`right`、`center`。</span><span class="sxs-lookup"><span data-stu-id="eee84-111">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="eee84-112">fontColor</span><span class="sxs-lookup"><span data-stu-id="eee84-112">fontColor</span></span>     | <span data-ttu-id="eee84-113">字符串</span><span class="sxs-lookup"><span data-stu-id="eee84-113">String</span></span> | <span data-ttu-id="eee84-114">用于页脚的字体颜色。</span><span class="sxs-lookup"><span data-stu-id="eee84-114">Color of the font to use for the footer.</span></span>                      |
| <span data-ttu-id="eee84-115">fontName</span><span class="sxs-lookup"><span data-stu-id="eee84-115">fontName</span></span>      | <span data-ttu-id="eee84-116">字符串</span><span class="sxs-lookup"><span data-stu-id="eee84-116">String</span></span> | <span data-ttu-id="eee84-117">要用于页脚的字体的名称。</span><span class="sxs-lookup"><span data-stu-id="eee84-117">Name of the font to use for the footer.</span></span>                       |
| <span data-ttu-id="eee84-118">fontSize</span><span class="sxs-lookup"><span data-stu-id="eee84-118">fontSize</span></span>      | <span data-ttu-id="eee84-119">Int32</span><span class="sxs-lookup"><span data-stu-id="eee84-119">Int32</span></span>  | <span data-ttu-id="eee84-120">用于页脚的字号。</span><span class="sxs-lookup"><span data-stu-id="eee84-120">Font size to use for the footer.</span></span>                              |
| <span data-ttu-id="eee84-121">页脚</span><span class="sxs-lookup"><span data-stu-id="eee84-121">margin</span></span>        | <span data-ttu-id="eee84-122">Int32</span><span class="sxs-lookup"><span data-stu-id="eee84-122">Int32</span></span>  | <span data-ttu-id="eee84-123">文档底部的页眉的边距。</span><span class="sxs-lookup"><span data-stu-id="eee84-123">The margin of the header from the bottom of the document.</span></span>     |
| <span data-ttu-id="eee84-124">text</span><span class="sxs-lookup"><span data-stu-id="eee84-124">text</span></span>          | <span data-ttu-id="eee84-125">字符串</span><span class="sxs-lookup"><span data-stu-id="eee84-125">String</span></span> | <span data-ttu-id="eee84-126">页脚本身的内容。</span><span class="sxs-lookup"><span data-stu-id="eee84-126">The contents of the footer itself.</span></span>                            |
| <span data-ttu-id="eee84-127">uiElementName</span><span class="sxs-lookup"><span data-stu-id="eee84-127">uiElementName</span></span> | <span data-ttu-id="eee84-128">字符串</span><span class="sxs-lookup"><span data-stu-id="eee84-128">String</span></span> | <span data-ttu-id="eee84-129">应在其中放置页脚的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="eee84-129">The name of the UI element where the footer should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eee84-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eee84-130">JSON representation</span></span>

<span data-ttu-id="eee84-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eee84-131">The following is a JSON representation of the resource.</span></span>

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