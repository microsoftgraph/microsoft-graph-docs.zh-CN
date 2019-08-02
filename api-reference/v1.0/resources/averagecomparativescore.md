---
title: averageComparativeScore 资源类型
description: 包含基于不同范围的各种不同分数。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f128fd22562889a5a537f3815a4003aec9bfc8a9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030014"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="ab15d-103">averageComparativeScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab15d-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="ab15d-104">包含基于不同范围的各种不同分数 (例如, 按行业垂直、按公司座位大小的平均值等) 和控制类别 (标识、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="ab15d-104">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="ab15d-105">属性</span><span class="sxs-lookup"><span data-stu-id="ab15d-105">Properties</span></span>

|<span data-ttu-id="ab15d-106">属性</span><span class="sxs-lookup"><span data-stu-id="ab15d-106">Property</span></span> |<span data-ttu-id="ab15d-107">类型</span><span class="sxs-lookup"><span data-stu-id="ab15d-107">Type</span></span> |<span data-ttu-id="ab15d-108">说明</span><span class="sxs-lookup"><span data-stu-id="ab15d-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="ab15d-109">基本</span><span class="sxs-lookup"><span data-stu-id="ab15d-109">basis</span></span>|<span data-ttu-id="ab15d-110">String</span><span class="sxs-lookup"><span data-stu-id="ab15d-110">String</span></span>|<span data-ttu-id="ab15d-111">范围类型。</span><span class="sxs-lookup"><span data-stu-id="ab15d-111">Scope type.</span></span> <span data-ttu-id="ab15d-112">可能的值包括 `AllTenants`、`TotalSeats`、`IndustryTypes`。</span><span class="sxs-lookup"><span data-stu-id="ab15d-112">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="ab15d-113">averageScore</span><span class="sxs-lookup"><span data-stu-id="ab15d-113">averageScore</span></span>|<span data-ttu-id="ab15d-114">双精度</span><span class="sxs-lookup"><span data-stu-id="ab15d-114">Double</span></span>|<span data-ttu-id="ab15d-115">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="ab15d-115">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab15d-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab15d-116">JSON representation</span></span>

<span data-ttu-id="ab15d-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab15d-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
