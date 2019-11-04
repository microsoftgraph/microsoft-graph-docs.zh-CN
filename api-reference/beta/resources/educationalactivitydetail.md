---
title: educationalActivityDetail 资源类型
description: educationalActivityDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e8e79ac7831698bf22d5785b83ebaa71961e19df
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935266"
---
# <a name="educationalactivitydetail-resource-type"></a><span data-ttu-id="c7f13-103">educationalActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7f13-103">educationalActivityDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7f13-104">代表用户已进行并在[educationalActivity](educationalActivity.md)资源中使用的 undergraduate、毕业、postgraduate 学位或其他教学活动的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="c7f13-104">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="c7f13-105">属性</span><span class="sxs-lookup"><span data-stu-id="c7f13-105">Properties</span></span>

| <span data-ttu-id="c7f13-106">属性</span><span class="sxs-lookup"><span data-stu-id="c7f13-106">Property</span></span>     | <span data-ttu-id="c7f13-107">类型</span><span class="sxs-lookup"><span data-stu-id="c7f13-107">Type</span></span>        | <span data-ttu-id="c7f13-108">描述</span><span class="sxs-lookup"><span data-stu-id="c7f13-108">Description</span></span>                                                   |
|:-------------|:------------|:--------------------------------------------------------------|
|<span data-ttu-id="c7f13-109">缩写</span><span class="sxs-lookup"><span data-stu-id="c7f13-109">abbreviation</span></span>  |<span data-ttu-id="c7f13-110">字符串</span><span class="sxs-lookup"><span data-stu-id="c7f13-110">String</span></span>       |<span data-ttu-id="c7f13-111">缩短学位或程序的名称（示例： PhD、MBA）</span><span class="sxs-lookup"><span data-stu-id="c7f13-111">Shortened name of the degree or program (example: PhD, MBA)</span></span>    |
|<span data-ttu-id="c7f13-112">activities</span><span class="sxs-lookup"><span data-stu-id="c7f13-112">activities</span></span>    |<span data-ttu-id="c7f13-113">字符串</span><span class="sxs-lookup"><span data-stu-id="c7f13-113">String</span></span>       |<span data-ttu-id="c7f13-114">课外与程序一起开展的活动。</span><span class="sxs-lookup"><span data-stu-id="c7f13-114">Extracurricular activities undertaken alongside the program.</span></span>   |
|<span data-ttu-id="c7f13-115">奖励</span><span class="sxs-lookup"><span data-stu-id="c7f13-115">awards</span></span>        |<span data-ttu-id="c7f13-116">字符串</span><span class="sxs-lookup"><span data-stu-id="c7f13-116">String</span></span>       |<span data-ttu-id="c7f13-117">与该计划相关的任何奖项或荣誉。</span><span class="sxs-lookup"><span data-stu-id="c7f13-117">Any awards or honors associated with the program.</span></span>              |
|<span data-ttu-id="c7f13-118">description</span><span class="sxs-lookup"><span data-stu-id="c7f13-118">description</span></span>   |<span data-ttu-id="c7f13-119">字符串</span><span class="sxs-lookup"><span data-stu-id="c7f13-119">String</span></span>       |<span data-ttu-id="c7f13-120">用户提供的程序的简短说明。</span><span class="sxs-lookup"><span data-stu-id="c7f13-120">Short description of the program provided by the user.</span></span>         |
|<span data-ttu-id="c7f13-121">displayName</span><span class="sxs-lookup"><span data-stu-id="c7f13-121">displayName</span></span>   |<span data-ttu-id="c7f13-122">字符串</span><span class="sxs-lookup"><span data-stu-id="c7f13-122">String</span></span>       |<span data-ttu-id="c7f13-123">用户提供的程序的长格式名称。</span><span class="sxs-lookup"><span data-stu-id="c7f13-123">Long-form name of the program that the user has provided.</span></span>      |
|<span data-ttu-id="c7f13-124">fieldsOfStudy</span><span class="sxs-lookup"><span data-stu-id="c7f13-124">fieldsOfStudy</span></span> |<span data-ttu-id="c7f13-125">字符串</span><span class="sxs-lookup"><span data-stu-id="c7f13-125">String</span></span>       |<span data-ttu-id="c7f13-126">与程序关联的 Majors 和未成年人。</span><span class="sxs-lookup"><span data-stu-id="c7f13-126">Majors and minors associated with the program.</span></span> <span data-ttu-id="c7f13-127">（如果适用）</span><span class="sxs-lookup"><span data-stu-id="c7f13-127">(if applicable)</span></span> |
|<span data-ttu-id="c7f13-128">grade</span><span class="sxs-lookup"><span data-stu-id="c7f13-128">grade</span></span>         |<span data-ttu-id="c7f13-129">字符串</span><span class="sxs-lookup"><span data-stu-id="c7f13-129">String</span></span>       |<span data-ttu-id="c7f13-130">最终成绩、类、GPA 或分数。</span><span class="sxs-lookup"><span data-stu-id="c7f13-130">The final grade, class, GPA or score.</span></span>                          |
|<span data-ttu-id="c7f13-131">notes</span><span class="sxs-lookup"><span data-stu-id="c7f13-131">notes</span></span>         |<span data-ttu-id="c7f13-132">String</span><span class="sxs-lookup"><span data-stu-id="c7f13-132">String</span></span>       |<span data-ttu-id="c7f13-133">用户提供的其他笔记。</span><span class="sxs-lookup"><span data-stu-id="c7f13-133">Additional notes the user has provided.</span></span>                        |
|<span data-ttu-id="c7f13-134">webUrl</span><span class="sxs-lookup"><span data-stu-id="c7f13-134">webUrl</span></span>        |<span data-ttu-id="c7f13-135">String</span><span class="sxs-lookup"><span data-stu-id="c7f13-135">String</span></span>       |<span data-ttu-id="c7f13-136">指向 "度" 或 "程序" 页面的链接。</span><span class="sxs-lookup"><span data-stu-id="c7f13-136">Link to the degree or program page.</span></span>                            |

## <a name="json-representation"></a><span data-ttu-id="c7f13-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7f13-137">JSON representation</span></span>

<span data-ttu-id="c7f13-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7f13-138">The following is a JSON representation of the resource.</span></span>

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