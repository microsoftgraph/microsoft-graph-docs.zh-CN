---
title: teamsDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d398782cef79cdf92bc56502f7c6cbf1bcdee99d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979283"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="2f74d-103">teamsDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f74d-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2f74d-104">属性</span><span class="sxs-lookup"><span data-stu-id="2f74d-104">Properties</span></span>

| <span data-ttu-id="2f74d-105">属性</span><span class="sxs-lookup"><span data-stu-id="2f74d-105">Property</span></span>          | <span data-ttu-id="2f74d-106">类型</span><span class="sxs-lookup"><span data-stu-id="2f74d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2f74d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2f74d-107">reportRefreshDate</span></span> | <span data-ttu-id="2f74d-108">日期</span><span class="sxs-lookup"><span data-stu-id="2f74d-108">Date</span></span>   |
| <span data-ttu-id="2f74d-109">web</span><span class="sxs-lookup"><span data-stu-id="2f74d-109">web</span></span>               | <span data-ttu-id="2f74d-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2f74d-110">Int64</span></span>  |
| <span data-ttu-id="2f74d-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="2f74d-111">windowsPhone</span></span>      | <span data-ttu-id="2f74d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2f74d-112">Int64</span></span>  |
| <span data-ttu-id="2f74d-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="2f74d-113">androidPhone</span></span>      | <span data-ttu-id="2f74d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2f74d-114">Int64</span></span>  |
| <span data-ttu-id="2f74d-115">ios</span><span class="sxs-lookup"><span data-stu-id="2f74d-115">ios</span></span>               | <span data-ttu-id="2f74d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2f74d-116">Int64</span></span>  |
| <span data-ttu-id="2f74d-117">mac</span><span class="sxs-lookup"><span data-stu-id="2f74d-117">mac</span></span>               | <span data-ttu-id="2f74d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2f74d-118">Int64</span></span>  |
| <span data-ttu-id="2f74d-119">windows</span><span class="sxs-lookup"><span data-stu-id="2f74d-119">windows</span></span>           | <span data-ttu-id="2f74d-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2f74d-120">Int64</span></span>  |
| <span data-ttu-id="2f74d-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2f74d-121">reportPeriod</span></span>      | <span data-ttu-id="2f74d-122">String</span><span class="sxs-lookup"><span data-stu-id="2f74d-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2f74d-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f74d-123">JSON representation</span></span>

<span data-ttu-id="2f74d-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f74d-124">The following is a JSON representation of the resource.</span></span>

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
