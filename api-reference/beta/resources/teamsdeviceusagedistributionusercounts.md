---
title: teamsDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d398782cef79cdf92bc56502f7c6cbf1bcdee99d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553608"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="68c62-103">teamsDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="68c62-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="68c62-104">属性</span><span class="sxs-lookup"><span data-stu-id="68c62-104">Properties</span></span>

| <span data-ttu-id="68c62-105">属性</span><span class="sxs-lookup"><span data-stu-id="68c62-105">Property</span></span>          | <span data-ttu-id="68c62-106">类型</span><span class="sxs-lookup"><span data-stu-id="68c62-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="68c62-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="68c62-107">reportRefreshDate</span></span> | <span data-ttu-id="68c62-108">Date</span><span class="sxs-lookup"><span data-stu-id="68c62-108">Date</span></span>   |
| <span data-ttu-id="68c62-109">web</span><span class="sxs-lookup"><span data-stu-id="68c62-109">web</span></span>               | <span data-ttu-id="68c62-110">Int64</span><span class="sxs-lookup"><span data-stu-id="68c62-110">Int64</span></span>  |
| <span data-ttu-id="68c62-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="68c62-111">windowsPhone</span></span>      | <span data-ttu-id="68c62-112">Int64</span><span class="sxs-lookup"><span data-stu-id="68c62-112">Int64</span></span>  |
| <span data-ttu-id="68c62-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="68c62-113">androidPhone</span></span>      | <span data-ttu-id="68c62-114">Int64</span><span class="sxs-lookup"><span data-stu-id="68c62-114">Int64</span></span>  |
| <span data-ttu-id="68c62-115">ios</span><span class="sxs-lookup"><span data-stu-id="68c62-115">ios</span></span>               | <span data-ttu-id="68c62-116">Int64</span><span class="sxs-lookup"><span data-stu-id="68c62-116">Int64</span></span>  |
| <span data-ttu-id="68c62-117">mac</span><span class="sxs-lookup"><span data-stu-id="68c62-117">mac</span></span>               | <span data-ttu-id="68c62-118">Int64</span><span class="sxs-lookup"><span data-stu-id="68c62-118">Int64</span></span>  |
| <span data-ttu-id="68c62-119">时间</span><span class="sxs-lookup"><span data-stu-id="68c62-119">windows</span></span>           | <span data-ttu-id="68c62-120">Int64</span><span class="sxs-lookup"><span data-stu-id="68c62-120">Int64</span></span>  |
| <span data-ttu-id="68c62-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="68c62-121">reportPeriod</span></span>      | <span data-ttu-id="68c62-122">String</span><span class="sxs-lookup"><span data-stu-id="68c62-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="68c62-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68c62-123">JSON representation</span></span>

<span data-ttu-id="68c62-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68c62-124">The following is a JSON representation of the resource.</span></span>

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
