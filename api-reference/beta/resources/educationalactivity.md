---
title: educationalActivity 资源类型
description: educationalActivity 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8d060de55d765adb7e01e6b03842c569f03c8d4f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939619"
---
# <a name="educationalactivity-resource-type"></a><span data-ttu-id="5991c-103">educationalActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="5991c-103">educationalActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5991c-104">表示用户已提供与 undergraduate、毕业、postgraduate 或其他教学活动相关的数据。</span><span class="sxs-lookup"><span data-stu-id="5991c-104">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span>

<span data-ttu-id="5991c-105">继承[itemFacet](itemfacet.md)中的元数据属性。</span><span class="sxs-lookup"><span data-stu-id="5991c-105">Inherits metadata properties from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5991c-106">方法</span><span class="sxs-lookup"><span data-stu-id="5991c-106">Methods</span></span>

| <span data-ttu-id="5991c-107">方法</span><span class="sxs-lookup"><span data-stu-id="5991c-107">Method</span></span>                                                       | <span data-ttu-id="5991c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5991c-108">Return Type</span></span>                                   | <span data-ttu-id="5991c-109">说明</span><span class="sxs-lookup"><span data-stu-id="5991c-109">Description</span></span>                                                      |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="5991c-110">获取 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="5991c-110">Get educationalActivity</span></span>](../api/educationalactivity-get.md) | [<span data-ttu-id="5991c-111">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="5991c-111">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="5991c-112">读取 educationalActivity 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5991c-112">Read properties and relationships of educationalActivity object.</span></span> |
| [<span data-ttu-id="5991c-113">Update</span><span class="sxs-lookup"><span data-stu-id="5991c-113">Update</span></span>](../api/educationalactivity-update.md)               | [<span data-ttu-id="5991c-114">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="5991c-114">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="5991c-115">更新 educationalActivity 对象。</span><span class="sxs-lookup"><span data-stu-id="5991c-115">Update educationalActivity object.</span></span>                               |
| [<span data-ttu-id="5991c-116">删除</span><span class="sxs-lookup"><span data-stu-id="5991c-116">Delete</span></span>](../api/educationalactivity-delete.md)               | <span data-ttu-id="5991c-117">无</span><span class="sxs-lookup"><span data-stu-id="5991c-117">None</span></span>                                          | <span data-ttu-id="5991c-118">删除 educationalActivity 对象。</span><span class="sxs-lookup"><span data-stu-id="5991c-118">Delete educationalActivity object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="5991c-119">属性</span><span class="sxs-lookup"><span data-stu-id="5991c-119">Properties</span></span>

| <span data-ttu-id="5991c-120">属性</span><span class="sxs-lookup"><span data-stu-id="5991c-120">Property</span></span>           | <span data-ttu-id="5991c-121">类型</span><span class="sxs-lookup"><span data-stu-id="5991c-121">Type</span></span>                                                      | <span data-ttu-id="5991c-122">描述</span><span class="sxs-lookup"><span data-stu-id="5991c-122">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="5991c-123">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="5991c-123">completionMonthYear</span></span> |<span data-ttu-id="5991c-124">日期</span><span class="sxs-lookup"><span data-stu-id="5991c-124">Date</span></span>                                                       |<span data-ttu-id="5991c-125">用户逐步或完成活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="5991c-125">The month and year the user graduated or completed the activity.</span></span>            |
|<span data-ttu-id="5991c-126">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="5991c-126">endMonthYear</span></span>        |<span data-ttu-id="5991c-127">日期</span><span class="sxs-lookup"><span data-stu-id="5991c-127">Date</span></span>                                                       |<span data-ttu-id="5991c-128">用户完成所引用的教育活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="5991c-128">The month and year the user completed the educational activity referenced.</span></span>  |
|<span data-ttu-id="5991c-129">机构</span><span class="sxs-lookup"><span data-stu-id="5991c-129">institution</span></span>         |[<span data-ttu-id="5991c-130">institutionData</span><span class="sxs-lookup"><span data-stu-id="5991c-130">institutionData</span></span>](institutiondata.md)                      |<span data-ttu-id="5991c-131">包含在上研究的机构的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5991c-131">Contains details of the institution studied at.</span></span>                             |
|<span data-ttu-id="5991c-132">主程序</span><span class="sxs-lookup"><span data-stu-id="5991c-132">program</span></span>             |[<span data-ttu-id="5991c-133">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="5991c-133">educationalActivityDetail</span></span>](educationalactivitydetail.md)  |<span data-ttu-id="5991c-134">包含有关程序或课程的扩展信息。</span><span class="sxs-lookup"><span data-stu-id="5991c-134">Contains extended information about the program or course.</span></span>                  |
|<span data-ttu-id="5991c-135">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="5991c-135">startMonthYear</span></span>      |<span data-ttu-id="5991c-136">日期</span><span class="sxs-lookup"><span data-stu-id="5991c-136">Date</span></span>                                                       |<span data-ttu-id="5991c-137">用户 commenced 引用的活动的月份和年份。</span><span class="sxs-lookup"><span data-stu-id="5991c-137">The month and year the user commenced the activity referenced.</span></span>              |

## <a name="relationships"></a><span data-ttu-id="5991c-138">关系</span><span class="sxs-lookup"><span data-stu-id="5991c-138">Relationships</span></span>

<span data-ttu-id="5991c-139">无</span><span class="sxs-lookup"><span data-stu-id="5991c-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5991c-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5991c-140">JSON representation</span></span>

<span data-ttu-id="5991c-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5991c-141">The following is a JSON representation of the resource.</span></span>

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