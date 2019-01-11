---
title: teamsDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: a02dfa5a5036d67a624656d715c0fb0d3c8194ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868696"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="c3b55-103">teamsDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3b55-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c3b55-104">属性</span><span class="sxs-lookup"><span data-stu-id="c3b55-104">Properties</span></span>

| <span data-ttu-id="c3b55-105">属性</span><span class="sxs-lookup"><span data-stu-id="c3b55-105">Property</span></span>          | <span data-ttu-id="c3b55-106">类型</span><span class="sxs-lookup"><span data-stu-id="c3b55-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c3b55-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c3b55-107">reportRefreshDate</span></span> | <span data-ttu-id="c3b55-108">日期</span><span class="sxs-lookup"><span data-stu-id="c3b55-108">Date</span></span>   |
| <span data-ttu-id="c3b55-109">web</span><span class="sxs-lookup"><span data-stu-id="c3b55-109">web</span></span>               | <span data-ttu-id="c3b55-110">Int64</span><span class="sxs-lookup"><span data-stu-id="c3b55-110">Int64</span></span>  |
| <span data-ttu-id="c3b55-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="c3b55-111">windowsPhone</span></span>      | <span data-ttu-id="c3b55-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c3b55-112">Int64</span></span>  |
| <span data-ttu-id="c3b55-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="c3b55-113">androidPhone</span></span>      | <span data-ttu-id="c3b55-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c3b55-114">Int64</span></span>  |
| <span data-ttu-id="c3b55-115">ios</span><span class="sxs-lookup"><span data-stu-id="c3b55-115">ios</span></span>               | <span data-ttu-id="c3b55-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c3b55-116">Int64</span></span>  |
| <span data-ttu-id="c3b55-117">mac</span><span class="sxs-lookup"><span data-stu-id="c3b55-117">mac</span></span>               | <span data-ttu-id="c3b55-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c3b55-118">Int64</span></span>  |
| <span data-ttu-id="c3b55-119">windows</span><span class="sxs-lookup"><span data-stu-id="c3b55-119">windows</span></span>           | <span data-ttu-id="c3b55-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c3b55-120">Int64</span></span>  |
| <span data-ttu-id="c3b55-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c3b55-121">reportPeriod</span></span>      | <span data-ttu-id="c3b55-122">String</span><span class="sxs-lookup"><span data-stu-id="c3b55-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3b55-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3b55-123">JSON representation</span></span>

<span data-ttu-id="c3b55-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3b55-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportPeriod": "String"
}
```
