---
title: " averageComparativeScore 资源类型"
description: 此资源包含基于不同范围的不同分数（例如，按行业垂直、按公司座位大小的平均值等）和控制类别（标识、数据、设备、应用程序、基础结构）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e051ee3d1265c1dc65a5ab0cb9352d9cd536b21c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508050"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="4d9b7-103">averageComparativeScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d9b7-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="4d9b7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4d9b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4d9b7-105">此资源包含基于不同范围的不同分数（例如，按行业垂直、按公司座位大小的平均值等）和控制类别（标识、数据、设备、应用程序、基础结构）。</span><span class="sxs-lookup"><span data-stu-id="4d9b7-105">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="4d9b7-106">属性</span><span class="sxs-lookup"><span data-stu-id="4d9b7-106">Property</span></span> |<span data-ttu-id="4d9b7-107">类型</span><span class="sxs-lookup"><span data-stu-id="4d9b7-107">Type</span></span> |<span data-ttu-id="4d9b7-108">说明</span><span class="sxs-lookup"><span data-stu-id="4d9b7-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="4d9b7-109">基本</span><span class="sxs-lookup"><span data-stu-id="4d9b7-109">basis</span></span>   |   <span data-ttu-id="4d9b7-110">String</span><span class="sxs-lookup"><span data-stu-id="4d9b7-110">String</span></span>  |   <span data-ttu-id="4d9b7-111">范围类型（通过 AllTenants、TotalSeats、IndustryTypes）。</span><span class="sxs-lookup"><span data-stu-id="4d9b7-111">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="4d9b7-112">averageScore</span><span class="sxs-lookup"><span data-stu-id="4d9b7-112">averageScore</span></span>    |   <span data-ttu-id="4d9b7-113">双精度</span><span class="sxs-lookup"><span data-stu-id="4d9b7-113">Double</span></span>  | <span data-ttu-id="4d9b7-114">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="4d9b7-114">Average score within specified basis.</span></span> |
|   <span data-ttu-id="4d9b7-115">deviceScore</span><span class="sxs-lookup"><span data-stu-id="4d9b7-115">deviceScore</span></span> |   <span data-ttu-id="4d9b7-116">双精度</span><span class="sxs-lookup"><span data-stu-id="4d9b7-116">Double</span></span>  | <span data-ttu-id="4d9b7-117">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="4d9b7-117">Average score within specified basis.</span></span> |
|   <span data-ttu-id="4d9b7-118">dataScore</span><span class="sxs-lookup"><span data-stu-id="4d9b7-118">dataScore</span></span>   |   <span data-ttu-id="4d9b7-119">双精度</span><span class="sxs-lookup"><span data-stu-id="4d9b7-119">Double</span></span>  | <span data-ttu-id="4d9b7-120">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="4d9b7-120">Average score within specified basis.</span></span> |
|   <span data-ttu-id="4d9b7-121">identityScore</span><span class="sxs-lookup"><span data-stu-id="4d9b7-121">identityScore</span></span>   |   <span data-ttu-id="4d9b7-122">双精度</span><span class="sxs-lookup"><span data-stu-id="4d9b7-122">Double</span></span>  | <span data-ttu-id="4d9b7-123">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="4d9b7-123">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4d9b7-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d9b7-124">JSON representation</span></span>

<span data-ttu-id="4d9b7-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d9b7-125">The following is a JSON representation of the resource.</span></span>

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
