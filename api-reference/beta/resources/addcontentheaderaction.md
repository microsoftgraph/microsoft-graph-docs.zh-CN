---
title: addContentHeaderAction 资源类型
description: 表示一个操作，该操作指定要添加到信息中的内容标头的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 341af43f03d8a319c7aaec535681f21db0a7f7f4
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939101"
---
# <a name="addcontentheaderaction-resource-type"></a><span data-ttu-id="f6fdb-103">addContentHeaderAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6fdb-103">addContentHeaderAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6fdb-104">表示一个操作，该操作指定要添加到信息中的内容标头的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="f6fdb-104">Represents an action that specifies the details on the content header to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="f6fdb-105">属性</span><span class="sxs-lookup"><span data-stu-id="f6fdb-105">Properties</span></span>

| <span data-ttu-id="f6fdb-106">属性</span><span class="sxs-lookup"><span data-stu-id="f6fdb-106">Property</span></span>      | <span data-ttu-id="f6fdb-107">类型</span><span class="sxs-lookup"><span data-stu-id="f6fdb-107">Type</span></span>   | <span data-ttu-id="f6fdb-108">描述</span><span class="sxs-lookup"><span data-stu-id="f6fdb-108">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="f6fdb-109">alignment</span><span class="sxs-lookup"><span data-stu-id="f6fdb-109">alignment</span></span>     | <span data-ttu-id="f6fdb-110">字符串</span><span class="sxs-lookup"><span data-stu-id="f6fdb-110">String</span></span> | <span data-ttu-id="f6fdb-111">可取值为：`left`、`right`、`center`。</span><span class="sxs-lookup"><span data-stu-id="f6fdb-111">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="f6fdb-112">fontColor</span><span class="sxs-lookup"><span data-stu-id="f6fdb-112">fontColor</span></span>     | <span data-ttu-id="f6fdb-113">字符串</span><span class="sxs-lookup"><span data-stu-id="f6fdb-113">String</span></span> | <span data-ttu-id="f6fdb-114">标头使用的字体颜色。</span><span class="sxs-lookup"><span data-stu-id="f6fdb-114">Color of the font to use for the header.</span></span>                      |
| <span data-ttu-id="f6fdb-115">fontName</span><span class="sxs-lookup"><span data-stu-id="f6fdb-115">fontName</span></span>      | <span data-ttu-id="f6fdb-116">字符串</span><span class="sxs-lookup"><span data-stu-id="f6fdb-116">String</span></span> | <span data-ttu-id="f6fdb-117">要用于标头的字体的名称。</span><span class="sxs-lookup"><span data-stu-id="f6fdb-117">Name of the font to use for the header.</span></span>                       |
| <span data-ttu-id="f6fdb-118">fontSize</span><span class="sxs-lookup"><span data-stu-id="f6fdb-118">fontSize</span></span>      | <span data-ttu-id="f6fdb-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f6fdb-119">Int32</span></span>  | <span data-ttu-id="f6fdb-120">标头使用的字号。</span><span class="sxs-lookup"><span data-stu-id="f6fdb-120">Font size to use for the header.</span></span>                              |
| <span data-ttu-id="f6fdb-121">页脚</span><span class="sxs-lookup"><span data-stu-id="f6fdb-121">margin</span></span>        | <span data-ttu-id="f6fdb-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f6fdb-122">Int32</span></span>  | <span data-ttu-id="f6fdb-123">文档顶部的页眉的边距。</span><span class="sxs-lookup"><span data-stu-id="f6fdb-123">The margin of the header from the top of the document.</span></span>        |
| <span data-ttu-id="f6fdb-124">text</span><span class="sxs-lookup"><span data-stu-id="f6fdb-124">text</span></span>          | <span data-ttu-id="f6fdb-125">字符串</span><span class="sxs-lookup"><span data-stu-id="f6fdb-125">String</span></span> | <span data-ttu-id="f6fdb-126">标头本身的内容。</span><span class="sxs-lookup"><span data-stu-id="f6fdb-126">The contents of the header itself.</span></span>                            |
| <span data-ttu-id="f6fdb-127">uiElementName</span><span class="sxs-lookup"><span data-stu-id="f6fdb-127">uiElementName</span></span> | <span data-ttu-id="f6fdb-128">字符串</span><span class="sxs-lookup"><span data-stu-id="f6fdb-128">String</span></span> | <span data-ttu-id="f6fdb-129">应在其中放置标头的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="f6fdb-129">The name of the UI element where the header should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f6fdb-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6fdb-130">JSON representation</span></span>

<span data-ttu-id="f6fdb-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6fdb-131">The following is a JSON representation of the resource.</span></span>

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