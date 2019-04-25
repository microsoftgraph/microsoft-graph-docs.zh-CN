---
title: " averageComparativeScore 资源类型"
description: 此资源包含基于不同范围的不同分数 (例如, 按行业垂直、按公司座位大小的平均值等) 和控制类别 (标识、数据、设备、应用程序、基础结构)。
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535436"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="a9bb6-103">averageComparativeScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9bb6-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="a9bb6-104">此资源包含基于不同范围的不同分数 (例如, 按行业垂直、按公司座位大小的平均值等) 和控制类别 (标识、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="a9bb6-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="a9bb6-105">属性</span><span class="sxs-lookup"><span data-stu-id="a9bb6-105">Property</span></span> |<span data-ttu-id="a9bb6-106">类型</span><span class="sxs-lookup"><span data-stu-id="a9bb6-106">Type</span></span> |<span data-ttu-id="a9bb6-107">说明</span><span class="sxs-lookup"><span data-stu-id="a9bb6-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="a9bb6-108">基本</span><span class="sxs-lookup"><span data-stu-id="a9bb6-108">basis</span></span>   |   <span data-ttu-id="a9bb6-109">String</span><span class="sxs-lookup"><span data-stu-id="a9bb6-109">String</span></span>  |   <span data-ttu-id="a9bb6-110">范围类型 (通过 AllTenants、TotalSeats、IndustryTypes)。</span><span class="sxs-lookup"><span data-stu-id="a9bb6-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="a9bb6-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="a9bb6-111">averageScore</span></span>    |   <span data-ttu-id="a9bb6-112">双精度</span><span class="sxs-lookup"><span data-stu-id="a9bb6-112">Double</span></span>  | <span data-ttu-id="a9bb6-113">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="a9bb6-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="a9bb6-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="a9bb6-114">deviceScore</span></span> |   <span data-ttu-id="a9bb6-115">双精度</span><span class="sxs-lookup"><span data-stu-id="a9bb6-115">Double</span></span>  | <span data-ttu-id="a9bb6-116">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="a9bb6-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="a9bb6-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="a9bb6-117">dataScore</span></span>   |   <span data-ttu-id="a9bb6-118">双精度</span><span class="sxs-lookup"><span data-stu-id="a9bb6-118">Double</span></span>  | <span data-ttu-id="a9bb6-119">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="a9bb6-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="a9bb6-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="a9bb6-120">identityScore</span></span>   |   <span data-ttu-id="a9bb6-121">双精度</span><span class="sxs-lookup"><span data-stu-id="a9bb6-121">Double</span></span>  | <span data-ttu-id="a9bb6-122">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="a9bb6-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a9bb6-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9bb6-123">JSON representation</span></span>

<span data-ttu-id="a9bb6-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9bb6-124">The following is a JSON representation of the resource.</span></span>

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
