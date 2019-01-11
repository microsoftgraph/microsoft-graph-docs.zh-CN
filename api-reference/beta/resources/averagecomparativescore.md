---
title: " averageComparativeScore 资源类型"
description: 此资源包含基于按不同的作用域 （例如，平均通过行业垂直，平均按公司座位大小等） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 的各种不同分数。
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834592"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="55a33-103">averageComparativeScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="55a33-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="55a33-104">此资源包含基于按不同的作用域 （例如，平均通过行业垂直，平均按公司座位大小等） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 的各种不同分数。</span><span class="sxs-lookup"><span data-stu-id="55a33-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="55a33-105">属性</span><span class="sxs-lookup"><span data-stu-id="55a33-105">Property</span></span> |<span data-ttu-id="55a33-106">类型</span><span class="sxs-lookup"><span data-stu-id="55a33-106">Type</span></span> |<span data-ttu-id="55a33-107">Description</span><span class="sxs-lookup"><span data-stu-id="55a33-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="55a33-108">基础</span><span class="sxs-lookup"><span data-stu-id="55a33-108">basis</span></span>   |   <span data-ttu-id="55a33-109">字符串</span><span class="sxs-lookup"><span data-stu-id="55a33-109">String</span></span>  |   <span data-ttu-id="55a33-110">范围类型 (通过 AllTenants，TotalSeats，IndustryTypes)。</span><span class="sxs-lookup"><span data-stu-id="55a33-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="55a33-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="55a33-111">averageScore</span></span>    |   <span data-ttu-id="55a33-112">Double</span><span class="sxs-lookup"><span data-stu-id="55a33-112">Double</span></span>  | <span data-ttu-id="55a33-113">指定基础内的平均得分。</span><span class="sxs-lookup"><span data-stu-id="55a33-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="55a33-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="55a33-114">deviceScore</span></span> |   <span data-ttu-id="55a33-115">Double</span><span class="sxs-lookup"><span data-stu-id="55a33-115">Double</span></span>  | <span data-ttu-id="55a33-116">指定基础内的平均得分。</span><span class="sxs-lookup"><span data-stu-id="55a33-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="55a33-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="55a33-117">dataScore</span></span>   |   <span data-ttu-id="55a33-118">Double</span><span class="sxs-lookup"><span data-stu-id="55a33-118">Double</span></span>  | <span data-ttu-id="55a33-119">指定基础内的平均得分。</span><span class="sxs-lookup"><span data-stu-id="55a33-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="55a33-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="55a33-120">identityScore</span></span>   |   <span data-ttu-id="55a33-121">Double</span><span class="sxs-lookup"><span data-stu-id="55a33-121">Double</span></span>  | <span data-ttu-id="55a33-122">指定基础内的平均得分。</span><span class="sxs-lookup"><span data-stu-id="55a33-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="55a33-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55a33-123">JSON representation</span></span>

<span data-ttu-id="55a33-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55a33-124">The following is a JSON representation of the resource.</span></span>

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
