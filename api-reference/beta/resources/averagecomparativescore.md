---
title: " averageComparativeScore 资源类型"
description: 此资源包含基于不同范围的不同分数 (例如, 按行业垂直、按公司座位大小的平均值等) 和控制类别 (标识、数据、设备、应用程序、基础结构)。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3e2256e7edefd0670bb697ec6d89c9fb80a5beeb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013148"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="e86c1-103">averageComparativeScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="e86c1-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="e86c1-104">此资源包含基于不同范围的不同分数 (例如, 按行业垂直、按公司座位大小的平均值等) 和控制类别 (标识、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="e86c1-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="e86c1-105">属性</span><span class="sxs-lookup"><span data-stu-id="e86c1-105">Property</span></span> |<span data-ttu-id="e86c1-106">类型</span><span class="sxs-lookup"><span data-stu-id="e86c1-106">Type</span></span> |<span data-ttu-id="e86c1-107">说明</span><span class="sxs-lookup"><span data-stu-id="e86c1-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="e86c1-108">基本</span><span class="sxs-lookup"><span data-stu-id="e86c1-108">basis</span></span>   |   <span data-ttu-id="e86c1-109">String</span><span class="sxs-lookup"><span data-stu-id="e86c1-109">String</span></span>  |   <span data-ttu-id="e86c1-110">范围类型 (通过 AllTenants、TotalSeats、IndustryTypes)。</span><span class="sxs-lookup"><span data-stu-id="e86c1-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="e86c1-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="e86c1-111">averageScore</span></span>    |   <span data-ttu-id="e86c1-112">双精度</span><span class="sxs-lookup"><span data-stu-id="e86c1-112">Double</span></span>  | <span data-ttu-id="e86c1-113">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="e86c1-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="e86c1-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="e86c1-114">deviceScore</span></span> |   <span data-ttu-id="e86c1-115">双精度</span><span class="sxs-lookup"><span data-stu-id="e86c1-115">Double</span></span>  | <span data-ttu-id="e86c1-116">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="e86c1-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="e86c1-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="e86c1-117">dataScore</span></span>   |   <span data-ttu-id="e86c1-118">双精度</span><span class="sxs-lookup"><span data-stu-id="e86c1-118">Double</span></span>  | <span data-ttu-id="e86c1-119">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="e86c1-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="e86c1-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="e86c1-120">identityScore</span></span>   |   <span data-ttu-id="e86c1-121">双精度</span><span class="sxs-lookup"><span data-stu-id="e86c1-121">Double</span></span>  | <span data-ttu-id="e86c1-122">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="e86c1-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e86c1-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e86c1-123">JSON representation</span></span>

<span data-ttu-id="e86c1-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e86c1-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double",
  "deviceScore": "Double",
  "dataScore": "Double",
  "identityScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
