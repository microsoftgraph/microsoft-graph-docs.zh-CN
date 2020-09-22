---
title: educationalActivityDetail 资源类型
description: educationalActivityDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2f19f5e02ae26281a5ac1b2b48498a426f976e8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055659"
---
# <a name="educationalactivitydetail-resource-type"></a><span data-ttu-id="2d0a9-103">educationalActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d0a9-103">educationalActivityDetail resource type</span></span>

<span data-ttu-id="2d0a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d0a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d0a9-105">代表用户已进行并在 [educationalActivity](educationalActivity.md) 资源中使用的 undergraduate、毕业、postgraduate 学位或其他教学活动的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="2d0a9-105">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="2d0a9-106">属性</span><span class="sxs-lookup"><span data-stu-id="2d0a9-106">Properties</span></span>

| <span data-ttu-id="2d0a9-107">属性</span><span class="sxs-lookup"><span data-stu-id="2d0a9-107">Property</span></span>     | <span data-ttu-id="2d0a9-108">类型</span><span class="sxs-lookup"><span data-stu-id="2d0a9-108">Type</span></span>        | <span data-ttu-id="2d0a9-109">说明</span><span class="sxs-lookup"><span data-stu-id="2d0a9-109">Description</span></span>                                                   |
|:-------------|:------------|:--------------------------------------------------------------|
|<span data-ttu-id="2d0a9-110">缩写</span><span class="sxs-lookup"><span data-stu-id="2d0a9-110">abbreviation</span></span>  |<span data-ttu-id="2d0a9-111">String</span><span class="sxs-lookup"><span data-stu-id="2d0a9-111">String</span></span>       |<span data-ttu-id="2d0a9-112">简短的学位或程序名称 (例如： PhD、MBA) </span><span class="sxs-lookup"><span data-stu-id="2d0a9-112">Shortened name of the degree or program (example: PhD, MBA)</span></span>    |
|<span data-ttu-id="2d0a9-113">activities</span><span class="sxs-lookup"><span data-stu-id="2d0a9-113">activities</span></span>    |<span data-ttu-id="2d0a9-114">String</span><span class="sxs-lookup"><span data-stu-id="2d0a9-114">String</span></span>       |<span data-ttu-id="2d0a9-115">课外与程序一起开展的活动。</span><span class="sxs-lookup"><span data-stu-id="2d0a9-115">Extracurricular activities undertaken alongside the program.</span></span>   |
|<span data-ttu-id="2d0a9-116">奖项</span><span class="sxs-lookup"><span data-stu-id="2d0a9-116">awards</span></span>        |<span data-ttu-id="2d0a9-117">String</span><span class="sxs-lookup"><span data-stu-id="2d0a9-117">String</span></span>       |<span data-ttu-id="2d0a9-118">与该计划相关的任何奖项或荣誉。</span><span class="sxs-lookup"><span data-stu-id="2d0a9-118">Any awards or honors associated with the program.</span></span>              |
|<span data-ttu-id="2d0a9-119">说明</span><span class="sxs-lookup"><span data-stu-id="2d0a9-119">description</span></span>   |<span data-ttu-id="2d0a9-120">String</span><span class="sxs-lookup"><span data-stu-id="2d0a9-120">String</span></span>       |<span data-ttu-id="2d0a9-121">用户提供的程序的简短说明。</span><span class="sxs-lookup"><span data-stu-id="2d0a9-121">Short description of the program provided by the user.</span></span>         |
|<span data-ttu-id="2d0a9-122">displayName</span><span class="sxs-lookup"><span data-stu-id="2d0a9-122">displayName</span></span>   |<span data-ttu-id="2d0a9-123">String</span><span class="sxs-lookup"><span data-stu-id="2d0a9-123">String</span></span>       |<span data-ttu-id="2d0a9-124">用户提供的程序的长格式名称。</span><span class="sxs-lookup"><span data-stu-id="2d0a9-124">Long-form name of the program that the user has provided.</span></span>      |
|<span data-ttu-id="2d0a9-125">fieldsOfStudy</span><span class="sxs-lookup"><span data-stu-id="2d0a9-125">fieldsOfStudy</span></span> |<span data-ttu-id="2d0a9-126">String</span><span class="sxs-lookup"><span data-stu-id="2d0a9-126">String</span></span>       |<span data-ttu-id="2d0a9-127">与程序关联的 Majors 和未成年人。</span><span class="sxs-lookup"><span data-stu-id="2d0a9-127">Majors and minors associated with the program.</span></span> <span data-ttu-id="2d0a9-128"> (（如果适用）) </span><span class="sxs-lookup"><span data-stu-id="2d0a9-128">(if applicable)</span></span> |
|<span data-ttu-id="2d0a9-129">grade</span><span class="sxs-lookup"><span data-stu-id="2d0a9-129">grade</span></span>         |<span data-ttu-id="2d0a9-130">String</span><span class="sxs-lookup"><span data-stu-id="2d0a9-130">String</span></span>       |<span data-ttu-id="2d0a9-131">最终成绩、类、GPA 或分数。</span><span class="sxs-lookup"><span data-stu-id="2d0a9-131">The final grade, class, GPA or score.</span></span>                          |
|<span data-ttu-id="2d0a9-132">notes</span><span class="sxs-lookup"><span data-stu-id="2d0a9-132">notes</span></span>         |<span data-ttu-id="2d0a9-133">String</span><span class="sxs-lookup"><span data-stu-id="2d0a9-133">String</span></span>       |<span data-ttu-id="2d0a9-134">用户提供的其他笔记。</span><span class="sxs-lookup"><span data-stu-id="2d0a9-134">Additional notes the user has provided.</span></span>                        |
|<span data-ttu-id="2d0a9-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="2d0a9-135">webUrl</span></span>        |<span data-ttu-id="2d0a9-136">String</span><span class="sxs-lookup"><span data-stu-id="2d0a9-136">String</span></span>       |<span data-ttu-id="2d0a9-137">指向 "度" 或 "程序" 页面的链接。</span><span class="sxs-lookup"><span data-stu-id="2d0a9-137">Link to the degree or program page.</span></span>                            |

## <a name="json-representation"></a><span data-ttu-id="2d0a9-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d0a9-138">JSON representation</span></span>

<span data-ttu-id="2d0a9-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d0a9-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationalActivityDetail",
  "baseType": null
}-->

```json
{
  "abbreviation": "String",
  "activities": "String",
  "awards": "String",
  "description": "String",
  "displayName": "String",
  "fieldsOfStudy": "String",
  "grade": "String",
  "notes": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationalActivityDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

