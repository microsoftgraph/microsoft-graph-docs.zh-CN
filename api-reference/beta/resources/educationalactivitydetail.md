---
title: educationalActivityDetail 资源类型
description: educationalActivityDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ccacf02184bbf54e49949d7671d34dde93b3859f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502821"
---
# <a name="educationalactivitydetail-resource-type"></a><span data-ttu-id="615fb-103">educationalActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="615fb-103">educationalActivityDetail resource type</span></span>

<span data-ttu-id="615fb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="615fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="615fb-105">代表用户已进行并在[educationalActivity](educationalActivity.md)资源中使用的 undergraduate、毕业、postgraduate 学位或其他教学活动的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="615fb-105">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="615fb-106">属性</span><span class="sxs-lookup"><span data-stu-id="615fb-106">Properties</span></span>

| <span data-ttu-id="615fb-107">属性</span><span class="sxs-lookup"><span data-stu-id="615fb-107">Property</span></span>     | <span data-ttu-id="615fb-108">类型</span><span class="sxs-lookup"><span data-stu-id="615fb-108">Type</span></span>        | <span data-ttu-id="615fb-109">说明</span><span class="sxs-lookup"><span data-stu-id="615fb-109">Description</span></span>                                                   |
|:-------------|:------------|:--------------------------------------------------------------|
|<span data-ttu-id="615fb-110">缩写</span><span class="sxs-lookup"><span data-stu-id="615fb-110">abbreviation</span></span>  |<span data-ttu-id="615fb-111">String</span><span class="sxs-lookup"><span data-stu-id="615fb-111">String</span></span>       |<span data-ttu-id="615fb-112">缩短学位或程序的名称（示例： PhD、MBA）</span><span class="sxs-lookup"><span data-stu-id="615fb-112">Shortened name of the degree or program (example: PhD, MBA)</span></span>    |
|<span data-ttu-id="615fb-113">activities</span><span class="sxs-lookup"><span data-stu-id="615fb-113">activities</span></span>    |<span data-ttu-id="615fb-114">String</span><span class="sxs-lookup"><span data-stu-id="615fb-114">String</span></span>       |<span data-ttu-id="615fb-115">课外与程序一起开展的活动。</span><span class="sxs-lookup"><span data-stu-id="615fb-115">Extracurricular activities undertaken alongside the program.</span></span>   |
|<span data-ttu-id="615fb-116">奖励</span><span class="sxs-lookup"><span data-stu-id="615fb-116">awards</span></span>        |<span data-ttu-id="615fb-117">String</span><span class="sxs-lookup"><span data-stu-id="615fb-117">String</span></span>       |<span data-ttu-id="615fb-118">与该计划相关的任何奖项或荣誉。</span><span class="sxs-lookup"><span data-stu-id="615fb-118">Any awards or honors associated with the program.</span></span>              |
|<span data-ttu-id="615fb-119">说明</span><span class="sxs-lookup"><span data-stu-id="615fb-119">description</span></span>   |<span data-ttu-id="615fb-120">字符串</span><span class="sxs-lookup"><span data-stu-id="615fb-120">String</span></span>       |<span data-ttu-id="615fb-121">用户提供的程序的简短说明。</span><span class="sxs-lookup"><span data-stu-id="615fb-121">Short description of the program provided by the user.</span></span>         |
|<span data-ttu-id="615fb-122">displayName</span><span class="sxs-lookup"><span data-stu-id="615fb-122">displayName</span></span>   |<span data-ttu-id="615fb-123">字符串</span><span class="sxs-lookup"><span data-stu-id="615fb-123">String</span></span>       |<span data-ttu-id="615fb-124">用户提供的程序的长格式名称。</span><span class="sxs-lookup"><span data-stu-id="615fb-124">Long-form name of the program that the user has provided.</span></span>      |
|<span data-ttu-id="615fb-125">fieldsOfStudy</span><span class="sxs-lookup"><span data-stu-id="615fb-125">fieldsOfStudy</span></span> |<span data-ttu-id="615fb-126">String</span><span class="sxs-lookup"><span data-stu-id="615fb-126">String</span></span>       |<span data-ttu-id="615fb-127">与程序关联的 Majors 和未成年人。</span><span class="sxs-lookup"><span data-stu-id="615fb-127">Majors and minors associated with the program.</span></span> <span data-ttu-id="615fb-128">（如果适用）</span><span class="sxs-lookup"><span data-stu-id="615fb-128">(if applicable)</span></span> |
|<span data-ttu-id="615fb-129">grade</span><span class="sxs-lookup"><span data-stu-id="615fb-129">grade</span></span>         |<span data-ttu-id="615fb-130">String</span><span class="sxs-lookup"><span data-stu-id="615fb-130">String</span></span>       |<span data-ttu-id="615fb-131">最终成绩、类、GPA 或分数。</span><span class="sxs-lookup"><span data-stu-id="615fb-131">The final grade, class, GPA or score.</span></span>                          |
|<span data-ttu-id="615fb-132">notes</span><span class="sxs-lookup"><span data-stu-id="615fb-132">notes</span></span>         |<span data-ttu-id="615fb-133">String</span><span class="sxs-lookup"><span data-stu-id="615fb-133">String</span></span>       |<span data-ttu-id="615fb-134">用户提供的其他笔记。</span><span class="sxs-lookup"><span data-stu-id="615fb-134">Additional notes the user has provided.</span></span>                        |
|<span data-ttu-id="615fb-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="615fb-135">webUrl</span></span>        |<span data-ttu-id="615fb-136">String</span><span class="sxs-lookup"><span data-stu-id="615fb-136">String</span></span>       |<span data-ttu-id="615fb-137">指向 "度" 或 "程序" 页面的链接。</span><span class="sxs-lookup"><span data-stu-id="615fb-137">Link to the degree or program page.</span></span>                            |

## <a name="json-representation"></a><span data-ttu-id="615fb-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="615fb-138">JSON representation</span></span>

<span data-ttu-id="615fb-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="615fb-139">The following is a JSON representation of the resource.</span></span>

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