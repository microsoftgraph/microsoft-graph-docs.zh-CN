---
title: skypeForBusinessParticipantActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: de86c49da34c9af48478a912a6ab042a354a7bf5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808188"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="94161-103">skypeForBusinessParticipantActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="94161-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="94161-104">属性</span><span class="sxs-lookup"><span data-stu-id="94161-104">Properties</span></span>

| <span data-ttu-id="94161-105">属性</span><span class="sxs-lookup"><span data-stu-id="94161-105">Property</span></span>          | <span data-ttu-id="94161-106">类型</span><span class="sxs-lookup"><span data-stu-id="94161-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="94161-107">im</span><span class="sxs-lookup"><span data-stu-id="94161-107">im</span></span>                | <span data-ttu-id="94161-108">Int64</span><span class="sxs-lookup"><span data-stu-id="94161-108">Int64</span></span>  |
| <span data-ttu-id="94161-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="94161-109">audioVideo</span></span>        | <span data-ttu-id="94161-110">Int64</span><span class="sxs-lookup"><span data-stu-id="94161-110">Int64</span></span>  |
| <span data-ttu-id="94161-111">的</span><span class="sxs-lookup"><span data-stu-id="94161-111">appSharing</span></span>        | <span data-ttu-id="94161-112">Int64</span><span class="sxs-lookup"><span data-stu-id="94161-112">Int64</span></span>  |
| <span data-ttu-id="94161-113">web</span><span class="sxs-lookup"><span data-stu-id="94161-113">web</span></span>               | <span data-ttu-id="94161-114">Int64</span><span class="sxs-lookup"><span data-stu-id="94161-114">Int64</span></span>  |
| <span data-ttu-id="94161-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="94161-115">dialInOut3rdParty</span></span> | <span data-ttu-id="94161-116">Int64</span><span class="sxs-lookup"><span data-stu-id="94161-116">Int64</span></span>  |
| <span data-ttu-id="94161-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="94161-117">reportRefreshDate</span></span> | <span data-ttu-id="94161-118">日期</span><span class="sxs-lookup"><span data-stu-id="94161-118">Date</span></span>   |
| <span data-ttu-id="94161-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="94161-119">reportDate</span></span>        | <span data-ttu-id="94161-120">日期</span><span class="sxs-lookup"><span data-stu-id="94161-120">Date</span></span>   |
| <span data-ttu-id="94161-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="94161-121">reportPeriod</span></span>      | <span data-ttu-id="94161-122">String</span><span class="sxs-lookup"><span data-stu-id="94161-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94161-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94161-123">JSON representation</span></span>

<span data-ttu-id="94161-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94161-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
