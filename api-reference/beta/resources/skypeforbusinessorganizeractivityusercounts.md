---
title: skypeForBusinessOrganizerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 39ab5844adb9525b4e0f100892927d200609040c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858707"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a><span data-ttu-id="050e2-103">skypeForBusinessOrganizerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="050e2-103">skypeForBusinessOrganizerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="050e2-104">属性</span><span class="sxs-lookup"><span data-stu-id="050e2-104">Properties</span></span>

| <span data-ttu-id="050e2-105">属性</span><span class="sxs-lookup"><span data-stu-id="050e2-105">Property</span></span>           | <span data-ttu-id="050e2-106">类型</span><span class="sxs-lookup"><span data-stu-id="050e2-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="050e2-107">im</span><span class="sxs-lookup"><span data-stu-id="050e2-107">im</span></span>                 | <span data-ttu-id="050e2-108">Int64</span><span class="sxs-lookup"><span data-stu-id="050e2-108">Int64</span></span>  |
| <span data-ttu-id="050e2-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="050e2-109">audioVideo</span></span>         | <span data-ttu-id="050e2-110">Int64</span><span class="sxs-lookup"><span data-stu-id="050e2-110">Int64</span></span>  |
| <span data-ttu-id="050e2-111">的</span><span class="sxs-lookup"><span data-stu-id="050e2-111">appSharing</span></span>         | <span data-ttu-id="050e2-112">Int64</span><span class="sxs-lookup"><span data-stu-id="050e2-112">Int64</span></span>  |
| <span data-ttu-id="050e2-113">web</span><span class="sxs-lookup"><span data-stu-id="050e2-113">web</span></span>                | <span data-ttu-id="050e2-114">Int64</span><span class="sxs-lookup"><span data-stu-id="050e2-114">Int64</span></span>  |
| <span data-ttu-id="050e2-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="050e2-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="050e2-116">Int64</span><span class="sxs-lookup"><span data-stu-id="050e2-116">Int64</span></span>  |
| <span data-ttu-id="050e2-117">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="050e2-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="050e2-118">Int64</span><span class="sxs-lookup"><span data-stu-id="050e2-118">Int64</span></span>  |
| <span data-ttu-id="050e2-119">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="050e2-119">reportRefreshDate</span></span>  | <span data-ttu-id="050e2-120">日期</span><span class="sxs-lookup"><span data-stu-id="050e2-120">Date</span></span>   |
| <span data-ttu-id="050e2-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="050e2-121">reportDate</span></span>         | <span data-ttu-id="050e2-122">日期</span><span class="sxs-lookup"><span data-stu-id="050e2-122">Date</span></span>   |
| <span data-ttu-id="050e2-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="050e2-123">reportPeriod</span></span>       | <span data-ttu-id="050e2-124">String</span><span class="sxs-lookup"><span data-stu-id="050e2-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="050e2-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="050e2-125">JSON representation</span></span>

<span data-ttu-id="050e2-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="050e2-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "dialInOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
