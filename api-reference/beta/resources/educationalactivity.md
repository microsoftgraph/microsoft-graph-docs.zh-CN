---
title: educationalActivity 资源类型
description: educationalActivity 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e1f4ffd3154700f59ebdd26a2213755810b561ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502842"
---
# <a name="educationalactivity-resource-type"></a><span data-ttu-id="dc60c-103">educationalActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc60c-103">educationalActivity resource type</span></span>

<span data-ttu-id="dc60c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dc60c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc60c-105">表示用户已提供与 undergraduate、毕业、postgraduate 或其他教学活动相关的数据。</span><span class="sxs-lookup"><span data-stu-id="dc60c-105">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span>

<span data-ttu-id="dc60c-106">继承[itemFacet](itemfacet.md)中的元数据属性。</span><span class="sxs-lookup"><span data-stu-id="dc60c-106">Inherits metadata properties from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dc60c-107">方法</span><span class="sxs-lookup"><span data-stu-id="dc60c-107">Methods</span></span>

| <span data-ttu-id="dc60c-108">方法</span><span class="sxs-lookup"><span data-stu-id="dc60c-108">Method</span></span>                                                       | <span data-ttu-id="dc60c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="dc60c-109">Return Type</span></span>                                   | <span data-ttu-id="dc60c-110">说明</span><span class="sxs-lookup"><span data-stu-id="dc60c-110">Description</span></span>                                                      |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="dc60c-111">获取 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="dc60c-111">Get educationalActivity</span></span>](../api/educationalactivity-get.md) | [<span data-ttu-id="dc60c-112">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="dc60c-112">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="dc60c-113">读取 educationalActivity 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc60c-113">Read properties and relationships of educationalActivity object.</span></span> |
| [<span data-ttu-id="dc60c-114">更新</span><span class="sxs-lookup"><span data-stu-id="dc60c-114">Update</span></span>](../api/educationalactivity-update.md)               | [<span data-ttu-id="dc60c-115">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="dc60c-115">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="dc60c-116">更新 educationalActivity 对象。</span><span class="sxs-lookup"><span data-stu-id="dc60c-116">Update educationalActivity object.</span></span>                               |
| [<span data-ttu-id="dc60c-117">删除</span><span class="sxs-lookup"><span data-stu-id="dc60c-117">Delete</span></span>](../api/educationalactivity-delete.md)               | <span data-ttu-id="dc60c-118">无</span><span class="sxs-lookup"><span data-stu-id="dc60c-118">None</span></span>                                          | <span data-ttu-id="dc60c-119">删除 educationalActivity 对象。</span><span class="sxs-lookup"><span data-stu-id="dc60c-119">Delete educationalActivity object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="dc60c-120">属性</span><span class="sxs-lookup"><span data-stu-id="dc60c-120">Properties</span></span>

| <span data-ttu-id="dc60c-121">属性</span><span class="sxs-lookup"><span data-stu-id="dc60c-121">Property</span></span>           | <span data-ttu-id="dc60c-122">类型</span><span class="sxs-lookup"><span data-stu-id="dc60c-122">Type</span></span>                                                      | <span data-ttu-id="dc60c-123">说明</span><span class="sxs-lookup"><span data-stu-id="dc60c-123">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="dc60c-124">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="dc60c-124">completionMonthYear</span></span> |<span data-ttu-id="dc60c-125">日期</span><span class="sxs-lookup"><span data-stu-id="dc60c-125">Date</span></span>                                                       |<span data-ttu-id="dc60c-126">用户逐步或完成活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="dc60c-126">The month and year the user graduated or completed the activity.</span></span>            |
|<span data-ttu-id="dc60c-127">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="dc60c-127">endMonthYear</span></span>        |<span data-ttu-id="dc60c-128">日期</span><span class="sxs-lookup"><span data-stu-id="dc60c-128">Date</span></span>                                                       |<span data-ttu-id="dc60c-129">用户完成所引用的教育活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="dc60c-129">The month and year the user completed the educational activity referenced.</span></span>  |
|<span data-ttu-id="dc60c-130">机构</span><span class="sxs-lookup"><span data-stu-id="dc60c-130">institution</span></span>         |[<span data-ttu-id="dc60c-131">institutionData</span><span class="sxs-lookup"><span data-stu-id="dc60c-131">institutionData</span></span>](institutiondata.md)                      |<span data-ttu-id="dc60c-132">包含在上研究的机构的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dc60c-132">Contains details of the institution studied at.</span></span>                             |
|<span data-ttu-id="dc60c-133">主程序</span><span class="sxs-lookup"><span data-stu-id="dc60c-133">program</span></span>             |[<span data-ttu-id="dc60c-134">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="dc60c-134">educationalActivityDetail</span></span>](educationalactivitydetail.md)  |<span data-ttu-id="dc60c-135">包含有关程序或课程的扩展信息。</span><span class="sxs-lookup"><span data-stu-id="dc60c-135">Contains extended information about the program or course.</span></span>                  |
|<span data-ttu-id="dc60c-136">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="dc60c-136">startMonthYear</span></span>      |<span data-ttu-id="dc60c-137">日期</span><span class="sxs-lookup"><span data-stu-id="dc60c-137">Date</span></span>                                                       |<span data-ttu-id="dc60c-138">用户 commenced 引用的活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="dc60c-138">The month and year the user commenced the activity referenced.</span></span>              |

## <a name="relationships"></a><span data-ttu-id="dc60c-139">关系</span><span class="sxs-lookup"><span data-stu-id="dc60c-139">Relationships</span></span>

<span data-ttu-id="dc60c-140">无</span><span class="sxs-lookup"><span data-stu-id="dc60c-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc60c-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc60c-141">JSON representation</span></span>

<span data-ttu-id="dc60c-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc60c-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationalActivity",
  "baseType": ""
}-->

```json
{
  "completionMonthYear": "String (timestamp)",
  "endMonthYear": "String (timestamp)",
  "institution": {"@odata.type": "microsoft.graph.institutionData"},
  "program": {"@odata.type": "microsoft.graph.educationalActivityDetail"},
  "startMonthYear": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationalActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->