---
title: " averageComparativeScore 资源类型"
description: 此资源包含基于按不同的作用域 （例如，平均通过行业垂直，平均按公司座位大小等） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 的各种不同分数。
ms.openlocfilehash: 08e4ec60788b21476d8f1491ab5548c7a4ca2e01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042774"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="2a69e-103">averageComparativeScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a69e-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="2a69e-104">此资源包含基于按不同的作用域 （例如，平均通过行业垂直，平均按公司座位大小等） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 的各种不同分数。</span><span class="sxs-lookup"><span data-stu-id="2a69e-104">This resource contains various different scores based by different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

|<span data-ttu-id="2a69e-105">属性</span><span class="sxs-lookup"><span data-stu-id="2a69e-105">Property</span></span> |<span data-ttu-id="2a69e-106">类型</span><span class="sxs-lookup"><span data-stu-id="2a69e-106">Type</span></span> |<span data-ttu-id="2a69e-107">Description</span><span class="sxs-lookup"><span data-stu-id="2a69e-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="2a69e-108">基础</span><span class="sxs-lookup"><span data-stu-id="2a69e-108">basis</span></span>   |   <span data-ttu-id="2a69e-109">字符串</span><span class="sxs-lookup"><span data-stu-id="2a69e-109">String</span></span>  |   <span data-ttu-id="2a69e-110">范围类型 (通过 AllTenants，TotalSeats，IndustryTypes)。</span><span class="sxs-lookup"><span data-stu-id="2a69e-110">Scope type (By AllTenants, TotalSeats, IndustryTypes).</span></span>  |
|   <span data-ttu-id="2a69e-111">averageScore</span><span class="sxs-lookup"><span data-stu-id="2a69e-111">averageScore</span></span>    |   <span data-ttu-id="2a69e-112">双精度数</span><span class="sxs-lookup"><span data-stu-id="2a69e-112">Double</span></span>  | <span data-ttu-id="2a69e-113">指定基础内的平均得分。</span><span class="sxs-lookup"><span data-stu-id="2a69e-113">Average score within specified basis.</span></span> |
|   <span data-ttu-id="2a69e-114">deviceScore</span><span class="sxs-lookup"><span data-stu-id="2a69e-114">deviceScore</span></span> |   <span data-ttu-id="2a69e-115">双精度数</span><span class="sxs-lookup"><span data-stu-id="2a69e-115">Double</span></span>  | <span data-ttu-id="2a69e-116">指定基础内的平均得分。</span><span class="sxs-lookup"><span data-stu-id="2a69e-116">Average score within specified basis.</span></span> |
|   <span data-ttu-id="2a69e-117">dataScore</span><span class="sxs-lookup"><span data-stu-id="2a69e-117">dataScore</span></span>   |   <span data-ttu-id="2a69e-118">双精度数</span><span class="sxs-lookup"><span data-stu-id="2a69e-118">Double</span></span>  | <span data-ttu-id="2a69e-119">指定基础内的平均得分。</span><span class="sxs-lookup"><span data-stu-id="2a69e-119">Average score within specified basis.</span></span> |
|   <span data-ttu-id="2a69e-120">identityScore</span><span class="sxs-lookup"><span data-stu-id="2a69e-120">identityScore</span></span>   |   <span data-ttu-id="2a69e-121">双精度数</span><span class="sxs-lookup"><span data-stu-id="2a69e-121">Double</span></span>  | <span data-ttu-id="2a69e-122">指定基础内的平均得分。</span><span class="sxs-lookup"><span data-stu-id="2a69e-122">Average score within specified basis.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2a69e-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a69e-123">JSON representation</span></span>

<span data-ttu-id="2a69e-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a69e-124">The following is a JSON representation of the resource.</span></span>

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
